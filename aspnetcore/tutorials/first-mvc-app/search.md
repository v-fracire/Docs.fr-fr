---
title: Ajouter une fonction de recherche à une application ASP.NET Core MVC
author: rick-anderson
description: Montre comment ajouter une fonction de recherche à une application ASP.NET MVC simple
ms.author: riande
ms.date: 03/07/2017
uid: tutorials/first-mvc-app/search
ms.openlocfilehash: d0581142b505323385feba441b707d29b3f6db5d
ms.sourcegitcommit: b8a2f14bf8dd346d7592977642b610bbcb0b0757
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38216194"
---
[!INCLUDE [adding-model](~/includes/mvc-intro/search1.md)]

Vous pouvez renommer rapidement le paramètre`searchString` en `id` à l’aide de la commande **Renommer**. Cliquez avec le bouton droit sur `searchString` **> Renommer**.

![Menu contextuel](search/_static/rename.png)

Les cibles de renommage sont mises en surbrillance.

![Éditeur de code présentant la variable mise en surbrillance à l’aide de la méthode Index ActionResult](search/_static/rename2.png)

Remplacez le paramètre par `id` et toutes les occurrences de `searchString` par `id`.

![Éditeur de code montrant que la variable a été remplacée par id](search/_static/rename3.png)

[!INCLUDE [adding-model](~/includes/mvc-intro/search2.md)]

Notez comment IntelliSense nous permet de mettre à jour la balise.

![Menu contextuel IntelliSense avec « method » sélectionné dans la liste des attributs de l’élément form](search/_static/int_m.png)

![Menu contextuel IntelliSense avec « get » sélectionné dans la liste des valeurs d’attribut de « method »](search/_static/int_get.png)

Notez la police distinctive dans la balise `<form>`. Cette police distinctive indique que la balise est prise en charge par les [Tag Helpers](~/mvc/views/tag-helpers/intro.md).

![balise form avec du texte en violet](search/_static/th_font.png)

[!INCLUDE [adding-model](~/includes/mvc-intro/search3.md)]

> [!div class="step-by-step"]
> [Précédent](controller-methods-views.md)
> [Suivant](new-field.md)  
