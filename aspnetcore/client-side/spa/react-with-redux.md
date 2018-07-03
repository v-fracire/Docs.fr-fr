---
title: Utiliser le modèle de projet React-with-Redux avec ASP.NET Core
author: SteveSandersonMS
description: Découvrez comment démarrer avec le modèle de projet d’application monopage ASP.NET Core pour React-with-Redux et create-react-app.
monikerRange: '>= aspnetcore-2.0'
ms.author: scaddie
ms.custom: mvc
ms.date: 02/21/2018
uid: spa/react-with-redux
ms.openlocfilehash: dab3d20865250aae548bff4614e631dd7c73b46f
ms.sourcegitcommit: a1afd04758e663d7062a5bfa8a0d4dca38f42afc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/20/2018
ms.locfileid: "36291482"
---
# <a name="use-the-react-with-redux-project-template-with-aspnet-core"></a><span data-ttu-id="28ebb-103">Utiliser le modèle de projet React-with-Redux avec ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="28ebb-103">Use the React-with-Redux project template with ASP.NET Core</span></span>

::: moniker range="= aspnetcore-2.0"

> [!NOTE]
> <span data-ttu-id="28ebb-104">Cette documentation ne concerne pas le modèle de projet React-with-Redux inclus dans ASP.NET Core 2.0.</span><span class="sxs-lookup"><span data-stu-id="28ebb-104">This documentation isn't about the React-with-Redux project template included in ASP.NET Core 2.0.</span></span> <span data-ttu-id="28ebb-105">Elle traite du nouveau modèle React-with-Redux vers lequel vous pouvez effectuer une mise à jour manuellement.</span><span class="sxs-lookup"><span data-stu-id="28ebb-105">It's about the newer React-with-Redux template to which you can update manually.</span></span> <span data-ttu-id="28ebb-106">Par défaut, le modèle est inclus dans ASP.NET Core 2.1.</span><span class="sxs-lookup"><span data-stu-id="28ebb-106">The template is included in ASP.NET Core 2.1 by default.</span></span>

::: moniker-end

<span data-ttu-id="28ebb-107">Le modèle de projet React-with-Redux mis à jour fournit un point de départ pratique pour les applications ASP.NET Core utilisant les conventions React, Redux et [create-react-app](https://github.com/facebookincubator/create-react-app) (CRA) pour implémenter une interface utilisateur (IU) côté client enrichie.</span><span class="sxs-lookup"><span data-stu-id="28ebb-107">The updated React-with-Redux project template provides a convenient starting point for ASP.NET Core apps using React, Redux, and [create-react-app](https://github.com/facebookincubator/create-react-app) (CRA) conventions to implement a rich, client-side user interface (UI).</span></span>

<span data-ttu-id="28ebb-108">À l’exception de la commande de création de projet, toutes les informations sur le modèle React-with-Redux sont les mêmes que celles relatives au modèle React.</span><span class="sxs-lookup"><span data-stu-id="28ebb-108">With the exception of the project creation command, all information about the React-with-Redux template is the same as the React template.</span></span> <span data-ttu-id="28ebb-109">Pour créer ce type de projet, exécutez `dotnet new reactredux` au lieu de `dotnet new react`.</span><span class="sxs-lookup"><span data-stu-id="28ebb-109">To create this project type, run `dotnet new reactredux` instead of `dotnet new react`.</span></span> <span data-ttu-id="28ebb-110">Pour plus d’informations sur les fonctionnalités communes aux deux modèles basés sur React, consultez la [documentation relative aux modèles React](xref:spa/react).</span><span class="sxs-lookup"><span data-stu-id="28ebb-110">For more information about the functionality common to both React-based templates, see [React template documentation](xref:spa/react).</span></span>