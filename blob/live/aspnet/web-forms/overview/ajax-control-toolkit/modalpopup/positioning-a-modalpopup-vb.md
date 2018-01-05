---
uid: web-forms/overview/ajax-control-toolkit/modalpopup/positioning-a-modalpopup-vb
title: "Positionnement d’un ModalPopup (VB) | Documents Microsoft"
author: wenz
description: "Le contrôle ModalPopup dans la boîte à outils de contrôle AJAX offre un moyen simple de créer une fenêtre modale, à l’aide des moyens de côté client. Toutefois le contrôle n’offre pas un..."
ms.author: aspnetcontent
manager: wpickett
ms.date: 06/02/2008
ms.topic: article
ms.assetid: 8a07210c-eb0e-485e-9ee8-82a101520e65
ms.technology: dotnet-webforms
ms.prod: .net-framework
msc.legacyurl: /web-forms/overview/ajax-control-toolkit/modalpopup/positioning-a-modalpopup-vb
msc.type: authoredcontent
ms.openlocfilehash: 4b9c0790d1696bcf478bcdea089d4d3d92450369
ms.sourcegitcommit: 9a9483aceb34591c97451997036a9120c3fe2baf
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/10/2017
---
<a name="positioning-a-modalpopup-vb"></a><span data-ttu-id="39598-104">Positionnement d’un ModalPopup (VB)</span><span class="sxs-lookup"><span data-stu-id="39598-104">Positioning a ModalPopup (VB)</span></span>
====================
<span data-ttu-id="39598-105">par [Christian Wenz](https://github.com/wenz)</span><span class="sxs-lookup"><span data-stu-id="39598-105">by [Christian Wenz](https://github.com/wenz)</span></span>

<span data-ttu-id="39598-106">[Télécharger le Code](http://download.microsoft.com/download/2/4/0/24052038-f942-4336-905b-b60ae56f0dd5/ModalPopup4.vb.zip) ou [télécharger le PDF](http://download.microsoft.com/download/b/6/a/b6ae89ee-df69-4c87-9bfb-ad1eb2b23373/modalpopup4VB.pdf)</span><span class="sxs-lookup"><span data-stu-id="39598-106">[Download Code](http://download.microsoft.com/download/2/4/0/24052038-f942-4336-905b-b60ae56f0dd5/ModalPopup4.vb.zip) or [Download PDF](http://download.microsoft.com/download/b/6/a/b6ae89ee-df69-4c87-9bfb-ad1eb2b23373/modalpopup4VB.pdf)</span></span>

> <span data-ttu-id="39598-107">Le contrôle ModalPopup dans la boîte à outils de contrôle AJAX offre un moyen simple de créer une fenêtre modale, à l’aide des moyens de côté client.</span><span class="sxs-lookup"><span data-stu-id="39598-107">The ModalPopup control in the AJAX Control Toolkit offers a simple way to create a modal popup using client-side means.</span></span> <span data-ttu-id="39598-108">Toutefois le contrôle n’offre pas une fonctionnalité intégrée pour positionner le menu contextuel.</span><span class="sxs-lookup"><span data-stu-id="39598-108">However the control does not offer a built-in functionality to position the popup.</span></span>


## <a name="overview"></a><span data-ttu-id="39598-109">Vue d'ensemble</span><span class="sxs-lookup"><span data-stu-id="39598-109">Overview</span></span>

<span data-ttu-id="39598-110">Le contrôle ModalPopup dans la boîte à outils de contrôle AJAX offre un moyen simple de créer une fenêtre modale, à l’aide des moyens de côté client.</span><span class="sxs-lookup"><span data-stu-id="39598-110">The ModalPopup control in the AJAX Control Toolkit offers a simple way to create a modal popup using client-side means.</span></span> <span data-ttu-id="39598-111">Toutefois le contrôle n’offre pas une fonctionnalité intégrée pour positionner le menu contextuel.</span><span class="sxs-lookup"><span data-stu-id="39598-111">However the control does not offer a built-in functionality to position the popup.</span></span>

## <a name="steps"></a><span data-ttu-id="39598-112">Étapes</span><span class="sxs-lookup"><span data-stu-id="39598-112">Steps</span></span>

<span data-ttu-id="39598-113">Pour activer la fonctionnalité d’ASP.NET AJAX et les outils de contrôle, le `ScriptManager`.</span><span class="sxs-lookup"><span data-stu-id="39598-113">In order to activate the functionality of ASP.NET AJAX and the Control Toolkit, the `ScriptManager`.</span></span> <span data-ttu-id="39598-114">contrôle doit être placé n’importe où sur la page (mais dans les limites du `<form>` élément) :</span><span class="sxs-lookup"><span data-stu-id="39598-114">control must be put anywhere on the page (but within the `<form>` element):</span></span>

[!code-aspx[Main](positioning-a-modalpopup-vb/samples/sample1.aspx)]

<span data-ttu-id="39598-115">Ensuite, ajoutez un panneau qui sert de la fenêtre contextuelle modale.</span><span class="sxs-lookup"><span data-stu-id="39598-115">Next, add a panel which serves as the modal popup.</span></span> <span data-ttu-id="39598-116">Un bouton est utilisé pour fermer la fenêtre contextuelle :</span><span class="sxs-lookup"><span data-stu-id="39598-116">A button is used to close the popup:</span></span>

[!code-aspx[Main](positioning-a-modalpopup-vb/samples/sample2.aspx)]

<span data-ttu-id="39598-117">Chaque fois que la fenêtre contextuelle s’affiche, il doit être situé à un lieu donné dans la page.</span><span class="sxs-lookup"><span data-stu-id="39598-117">Whenever the popup is shown, it shall be positioned at a certain place in the page.</span></span> <span data-ttu-id="39598-118">Pour cette tâche, une fonction de JavaScript côté client est créée.</span><span class="sxs-lookup"><span data-stu-id="39598-118">For this task, a client-side JavaScript function is created.</span></span> <span data-ttu-id="39598-119">Il tente d’abord d’accéder au panneau.</span><span class="sxs-lookup"><span data-stu-id="39598-119">It first tries to access the panel.</span></span> <span data-ttu-id="39598-120">Si elle réussit, la position du panneau est définie à l’aide de CSS et JavaScript (modifier la position de la fenêtre contextuelle à sera).</span><span class="sxs-lookup"><span data-stu-id="39598-120">If it succeeds, the panel's position is set using CSS and JavaScript (change the position of the popup at will).</span></span> <span data-ttu-id="39598-121">Toutefois, le `ModalPopupExtender` contrôle essaie également de positionner la fenêtre contextuelle.</span><span class="sxs-lookup"><span data-stu-id="39598-121">However the `ModalPopupExtender` control also tries to position the popup.</span></span> <span data-ttu-id="39598-122">Par conséquent, le code JavaScript positionne à plusieurs reprises de la fenêtre contextuelle, dixième de seconde.</span><span class="sxs-lookup"><span data-stu-id="39598-122">Therefore, the JavaScript code repeatedly positions the popup, every tenth of a second.</span></span>

[!code-html[Main](positioning-a-modalpopup-vb/samples/sample3.html)]

<span data-ttu-id="39598-123">Comme vous pouvez le voir, la valeur de retour de la `setTimeout()` méthode JavaScript est enregistrée dans une variable globale.</span><span class="sxs-lookup"><span data-stu-id="39598-123">As you can see, the return value of the `setTimeout()` JavaScript method is saved in a global variable.</span></span> <span data-ttu-id="39598-124">Cela permet d’arrêter le positionnement répétées de la fenêtre contextuelle à la demande, à l’aide de la `clearTimeout()` méthode :</span><span class="sxs-lookup"><span data-stu-id="39598-124">This allows to stop the repeated positioning of the popup on demand, using the `clearTimeout()` method:</span></span>

[!code-javascript[Main](positioning-a-modalpopup-vb/samples/sample4.js)]

<span data-ttu-id="39598-125">Maintenant, tout ce qui reste à faire consiste à appeler ces fonctions chaque fois qu’appropriée du navigateur.</span><span class="sxs-lookup"><span data-stu-id="39598-125">Now all that is left to do is to make the browser call these functions whenever appropriate.</span></span> <span data-ttu-id="39598-126">Le `movePanel()` fonction JavaScript doit être appelée lorsque le bouton qui déclenche le panneau de configuration :</span><span class="sxs-lookup"><span data-stu-id="39598-126">The `movePanel()` JavaScript function must be called when the button is clicked that triggers the panel:</span></span>

[!code-aspx[Main](positioning-a-modalpopup-vb/samples/sample5.aspx)]

<span data-ttu-id="39598-127">Et le `stopMoving()` fonction entre en jeu, la fermeture de la fenêtre contextuelle peut être déclenchée dans la `ModalPopupExtender` contrôle :</span><span class="sxs-lookup"><span data-stu-id="39598-127">And the `stopMoving()` function comes into play when the popup is closed this can be triggered in the `ModalPopupExtender` control:</span></span>

[!code-aspx[Main](positioning-a-modalpopup-vb/samples/sample6.aspx)]


<span data-ttu-id="39598-128">[![La fenêtre contextuelle modale s’affiche à la position désignée](positioning-a-modalpopup-vb/_static/image2.png)](positioning-a-modalpopup-vb/_static/image1.png)</span><span class="sxs-lookup"><span data-stu-id="39598-128">[![The modal popup appears at the designated position](positioning-a-modalpopup-vb/_static/image2.png)](positioning-a-modalpopup-vb/_static/image1.png)</span></span>

<span data-ttu-id="39598-129">La fenêtre contextuelle modale s’affiche à la position désignée ([cliquez pour afficher l’image en taille réelle](positioning-a-modalpopup-vb/_static/image3.png))</span><span class="sxs-lookup"><span data-stu-id="39598-129">The modal popup appears at the designated position ([Click to view full-size image](positioning-a-modalpopup-vb/_static/image3.png))</span></span>

>[!div class="step-by-step"]
[<span data-ttu-id="39598-130">Précédent</span><span class="sxs-lookup"><span data-stu-id="39598-130">Previous</span></span>](handling-postbacks-from-a-modalpopup-vb.md)