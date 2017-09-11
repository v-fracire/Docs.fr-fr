---
title: Application de SSL dans une application ASP.NET Core
author: rick-anderson
description: "Montre comment exiger le protocole SSL dans un cœur d’ASP.NET web app"
keywords: ASP.NET Core, SSL, HTTPS, RequireHttpsAttribute, IIS Express
ms.author: riande
manager: wpickett
ms.date: 07/19/2017
ms.topic: article
ms.technology: aspnet
ms.prod: asp.net-core
uid: security/enforcing-ssl
ms.openlocfilehash: 35554939bd574b2826053004ed437bee46154c2b
ms.sourcegitcommit: 0b6c8e6d81d2b3c161cd375036eecbace46a9707
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2017
---
# <a name="enforcing-ssl-in-an-aspnet-core-app"></a>Application de SSL dans une application ASP.NET Core

Par [Rick Anderson](https://twitter.com/RickAndMSFT)

Ce document montre comment :

- Exiger le protocole SSL pour toutes les demandes (uniquement pour les requêtes HTTPS).
- Rediriger toutes les demandes HTTP vers HTTPS.

## <a name="require-ssl"></a>Exiger le protocole SSL

Le [RequireHttpsAttribute](https://docs.microsoft.com/aspnet/core/api/microsoft.aspnetcore.mvc.requirehttpsattribute) est utilisée pour exiger SSL. Vous pouvez la décorer contrôleurs ou méthodes avec cet attribut, ou vous pouvez l’appliquer globalement, comme indiqué ci-dessous :

Ajoutez le code suivant à `ConfigureServices` dans `Startup`:

[!code-csharp[Main](authentication/accconfirm/sample/WebApp1/Startup.cs?name=snippet2&highlight=4-)]

Le code en surbrillance ci-dessus nécessite l’utilisation de toutes les demandes `HTTPS`, par conséquent, les requêtes HTTP sont ignorés. Le code en surbrillance suivant redirige toutes les demandes HTTP vers HTTPS :

[!code-csharp[Main](authentication/accconfirm/sample/WebApp1/Startup.cs?name=snippet_AddRedirectToHttps&highlight=7-)]

Consultez [intergiciel (middleware) réécriture d’URL](xref:fundamentals/url-rewriting) pour plus d’informations.

Nécessitant HTTPS globalement (`options.Filters.Add(new RequireHttpsAttribute());`) est une meilleure pratique de sécurité. Appliquer le `[RequireHttps]` attribut à tous les contrôleur n’est pas considéré comme autant nécessitant HTTPS globalement. Vous ne pouvez pas garantir la sécurité ajoutées à votre application de nouveaux contrôleurs penser à appliquer le `[RequireHttps]` attribut.

## <a name="set-up-iis-express-for-sslhttps"></a>Configurer IIS Express pour SSL/HTTPS

Consultez [configuration de HTTPS pour le développement dans ASP.NET Core](xref:security/https#iisxpress).