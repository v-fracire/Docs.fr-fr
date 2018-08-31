---
title: Nouveautés d’ASP.NET Core 2.1
author: isaac2004
description: Découvrez les nouvelles fonctionnalités d’ASP.NET Core 2.1.
monikerRange: = aspnetcore-2.1
ms.author: riande
ms.custom: mvc
ms.date: 05/30/2018
uid: aspnetcore-2.1
ms.openlocfilehash: acbed75e2e894569816669e250795c95482bde2a
ms.sourcegitcommit: 5a2456cbf429069dc48aaa2823cde14100e4c438
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2018
ms.locfileid: "42908991"
---
# <a name="whats-new-in-aspnet-core-21"></a><span data-ttu-id="52540-103">Nouveautés d’ASP.NET Core 2.1</span><span class="sxs-lookup"><span data-stu-id="52540-103">What's new in ASP.NET Core 2.1</span></span>

<span data-ttu-id="52540-104">Cet article met en évidence les modifications les plus importantes dans ASP.NET 2.1 Core et fournit des liens vers la documentation appropriée.</span><span class="sxs-lookup"><span data-stu-id="52540-104">This article highlights the most significant changes in ASP.NET Core 2.1, with links to relevant documentation.</span></span>

## <a name="signalr"></a><span data-ttu-id="52540-105">SignalR</span><span class="sxs-lookup"><span data-stu-id="52540-105">SignalR</span></span>

<span data-ttu-id="52540-106">SignalR a été réécrit pour ASP.NET Core 2.1.</span><span class="sxs-lookup"><span data-stu-id="52540-106">SignalR has been rewritten for ASP.NET Core 2.1.</span></span> <span data-ttu-id="52540-107">ASP.NET Core SignalR inclut un certain nombre d’améliorations :</span><span class="sxs-lookup"><span data-stu-id="52540-107">ASP.NET Core SignalR includes a number of improvements:</span></span>

* <span data-ttu-id="52540-108">Un modèle simplifié de montée en puissance parallèle.</span><span class="sxs-lookup"><span data-stu-id="52540-108">A simplified scale-out model.</span></span>
* <span data-ttu-id="52540-109">Un nouveau client JavaScript sans dépendance de jQuery.</span><span class="sxs-lookup"><span data-stu-id="52540-109">A new JavaScript client with no jQuery dependency.</span></span>
* <span data-ttu-id="52540-110">Un nouveau protocole binaire compact basé sur MessagePack.</span><span class="sxs-lookup"><span data-stu-id="52540-110">A new compact binary protocol based on MessagePack.</span></span>
* <span data-ttu-id="52540-111">Prise en charge des protocoles personnalisés.</span><span class="sxs-lookup"><span data-stu-id="52540-111">Support for custom protocols.</span></span>
* <span data-ttu-id="52540-112">Un nouveau modèle réponse de streaming.</span><span class="sxs-lookup"><span data-stu-id="52540-112">A new streaming response model.</span></span>
* <span data-ttu-id="52540-113">Prise en charge des clients basés sur des WebSocket nus.</span><span class="sxs-lookup"><span data-stu-id="52540-113">Support for clients based on bare WebSockets.</span></span>

<span data-ttu-id="52540-114">Pour plus d’informations, consultez [ASP.NET Core SignalR](xref:signalr/index).</span><span class="sxs-lookup"><span data-stu-id="52540-114">For more information, see [ASP.NET Core SignalR](xref:signalr/index).</span></span>

## <a name="razor-class-libraries"></a><span data-ttu-id="52540-115">Bibliothèques de classes Razor</span><span class="sxs-lookup"><span data-stu-id="52540-115">Razor class libraries</span></span>

<span data-ttu-id="52540-116">Avec ASP.NET Core 2.1, il est plus facile de générer une interface utilisateur basée sur Razor, de l’inclure dans une bibliothèque et de la partager entre plusieurs projets.</span><span class="sxs-lookup"><span data-stu-id="52540-116">ASP.NET Core 2.1 makes it easier to build and include Razor-based UI in a library and share it across multiple projects.</span></span> <span data-ttu-id="52540-117">Le nouveau SDK Razor permet de générer des fichiers Razor dans un projet de bibliothèque de classes qui peut être placé dans un package NuGet.</span><span class="sxs-lookup"><span data-stu-id="52540-117">The new Razor SDK enables building Razor files into a class library project that can be packaged into a NuGet package.</span></span> <span data-ttu-id="52540-118">Les vues et les pages dans les bibliothèques sont automatiquement découvertes et peuvent être remplacées par l’application.</span><span class="sxs-lookup"><span data-stu-id="52540-118">Views and pages in libraries are automatically discovered and can be overridden by the app.</span></span> <span data-ttu-id="52540-119">Grâce à l’intégration de la compilation Razor dans la build :</span><span class="sxs-lookup"><span data-stu-id="52540-119">By integrating Razor compilation into the build:</span></span>

* <span data-ttu-id="52540-120">Le temps de démarrage de l’application est nettement plus rapide.</span><span class="sxs-lookup"><span data-stu-id="52540-120">The app startup time is significantly faster.</span></span>
* <span data-ttu-id="52540-121">Les mises à jour rapides des pages et vues Razor au moment de l’exécution sont toujours disponibles dans le cadre d’un flux de travail de développement itératif.</span><span class="sxs-lookup"><span data-stu-id="52540-121">Fast updates to Razor views and pages at runtime are still available as part of an iterative development workflow.</span></span>

<span data-ttu-id="52540-122">Pour plus d’informations, consultez [Créer une interface utilisateur réutilisable à l’aide du projet Razor Class Library](xref:razor-pages/ui-class).</span><span class="sxs-lookup"><span data-stu-id="52540-122">For more information, see [Create reusable UI using the Razor Class Library project](xref:razor-pages/ui-class).</span></span>

## <a name="identity-ui-library--scaffolding"></a><span data-ttu-id="52540-123">Bibliothèque de l’interface utilisateur d’identité et génération de modèles automatique</span><span class="sxs-lookup"><span data-stu-id="52540-123">Identity UI library & scaffolding</span></span>

<span data-ttu-id="52540-124">ASP.NET Core 2.1 fournit [l’identité ASP.NET Core](xref:security/authentication/identity) comme [bibliothèque de classes Razor](xref:razor-pages/ui-class).</span><span class="sxs-lookup"><span data-stu-id="52540-124">ASP.NET Core 2.1 provides [ASP.NET Core Identity](xref:security/authentication/identity) as a [Razor Class Library](xref:razor-pages/ui-class).</span></span> <span data-ttu-id="52540-125">Les applications qui incluent l’identité peuvent appliquer le nouveau générateur de modèles automatique d’identité de manière sélective pour ajouter le code source contenu dans la bibliothèque de classes Razor d’identité (RCL).</span><span class="sxs-lookup"><span data-stu-id="52540-125">Apps that include Identity can apply the new Identity scaffolder to selectively add the source code contained in the Identity Razor Class Library (RCL).</span></span> <span data-ttu-id="52540-126">Vous pouvez souhaiter générer le code source afin de pouvoir modifier le code et changer le comportement.</span><span class="sxs-lookup"><span data-stu-id="52540-126">You might want to generate source code so you can modify the code and change the behavior.</span></span> <span data-ttu-id="52540-127">Par exemple, vous pouvez demander au générateur de modèles automatique de générer le code utilisé dans l’inscription.</span><span class="sxs-lookup"><span data-stu-id="52540-127">For example, you could instruct the scaffolder to generate the code used in registration.</span></span> <span data-ttu-id="52540-128">Le code généré est prioritaire sur le même code dans la bibliothèque de classes Razor d’identité.</span><span class="sxs-lookup"><span data-stu-id="52540-128">Generated code takes precedence over the same code in the Identity RCL.</span></span>

<span data-ttu-id="52540-129">Les applications qui **n’incluent pas** l’authentification peuvent appliquer le générateur de modèles automatique d’identité pour ajouter le package d’identité de la bibliothèque de classes.</span><span class="sxs-lookup"><span data-stu-id="52540-129">Apps that do **not** include authentication can apply the Identity scaffolder to add the RCL Identity package.</span></span> <span data-ttu-id="52540-130">Vous pouvez sélectionner le code d’identité à générer.</span><span class="sxs-lookup"><span data-stu-id="52540-130">You have the option of selecting Identity code to be generated.</span></span>

<span data-ttu-id="52540-131">Pour plus d’informations, consultez [Identité de vue de structure dans les projets ASP.NET Core](xref:security/authentication/scaffold-identity).</span><span class="sxs-lookup"><span data-stu-id="52540-131">For more information, see [Scaffold Identity in ASP.NET Core projects](xref:security/authentication/scaffold-identity).</span></span>

## <a name="https"></a><span data-ttu-id="52540-132">HTTPS</span><span class="sxs-lookup"><span data-stu-id="52540-132">HTTPS</span></span>

<span data-ttu-id="52540-133">L’importance croissante accordée à la sécurité et à la confidentialité justifie l’activation du protocole HTTPS pour les applications web.</span><span class="sxs-lookup"><span data-stu-id="52540-133">With the increased focus on security and privacy, enabling HTTPS for web apps is important.</span></span> <span data-ttu-id="52540-134">La mise en œuvre du protocole HTTPS devient de plus en plus stricte sur le web.</span><span class="sxs-lookup"><span data-stu-id="52540-134">HTTPS enforcement is becoming increasingly strict on the web.</span></span> <span data-ttu-id="52540-135">Les sites qui n’utilisent pas le protocole HTTPS sont considérés comme non sécurisés.</span><span class="sxs-lookup"><span data-stu-id="52540-135">Sites that don’t use HTTPS are considered insecure.</span></span> <span data-ttu-id="52540-136">Les navigateurs (Chrome, Mozilla) commencent à imposer l’utilisation des fonctionnalités web dans un contexte sécurisé.</span><span class="sxs-lookup"><span data-stu-id="52540-136">Browsers (Chromium, Mozilla) are starting to enforce that web features must be used from a secure context.</span></span> <span data-ttu-id="52540-137">Le [RGPD](xref:security/gdpr) exige l’utilisation du protocole HTTPS pour protéger la confidentialité des utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="52540-137">[GDPR](xref:security/gdpr) requires the use of HTTPS to protect user privacy.</span></span> <span data-ttu-id="52540-138">L’utilisation du protocole HTTPS en production est critique et son utilisation en développement peut aider à éviter les problèmes liés au déploiement (tels que les liens non sécurisés).</span><span class="sxs-lookup"><span data-stu-id="52540-138">While using HTTPS in production is critical, using HTTPS in development can help prevent issues in deployment (for example, insecure links).</span></span> <span data-ttu-id="52540-139">ASP.NET Core 2.1 inclut un certain nombre d’améliorations qui facilitent l’utilisation du protocole HTTPS pendant le développement et sa configuration en production.</span><span class="sxs-lookup"><span data-stu-id="52540-139">ASP.NET Core 2.1 includes a number of improvements that make it easier to use HTTPS in development and to configure HTTPS in production.</span></span> <span data-ttu-id="52540-140">Pour plus d’informations, consultez [Appliquer HTTPS](xref:security/enforcing-ssl).</span><span class="sxs-lookup"><span data-stu-id="52540-140">For more information, see [Enforce HTTPS](xref:security/enforcing-ssl).</span></span>

### <a name="on-by-default"></a><span data-ttu-id="52540-141">Activé par défaut</span><span class="sxs-lookup"><span data-stu-id="52540-141">On by default</span></span>

<span data-ttu-id="52540-142">Pour faciliter le développement de sites web sécurisés, le protocole HTTPS est maintenant activé par défaut.</span><span class="sxs-lookup"><span data-stu-id="52540-142">To facilitate secure website development, HTTPS  is now enabled by default.</span></span> <span data-ttu-id="52540-143">À compter de la version 2.1, Kestrel écoute sur `https://localhost:5001` quand un certificat de développement local est présent.</span><span class="sxs-lookup"><span data-stu-id="52540-143">Starting in 2.1, Kestrel listens on `https://localhost:5001` when a local development certificate is present.</span></span> <span data-ttu-id="52540-144">Un certificat de développement est créé :</span><span class="sxs-lookup"><span data-stu-id="52540-144">A development certificate is created:</span></span>

* <span data-ttu-id="52540-145">Dans le cadre de la première exécution du kit SDK .NET Core, quand vous utilisez celui-ci pour la première fois.</span><span class="sxs-lookup"><span data-stu-id="52540-145">As part of the .NET Core SDK first-run experience, when you use the SDK for the first time.</span></span>
* <span data-ttu-id="52540-146">Manuellement à l’aide du nouvel outil `dev-certs`.</span><span class="sxs-lookup"><span data-stu-id="52540-146">Manually using the new `dev-certs` tool.</span></span>

<span data-ttu-id="52540-147">Exécutez `dotnet dev-certs https --trust` pour approuver le certificat.</span><span class="sxs-lookup"><span data-stu-id="52540-147">Run `dotnet dev-certs https --trust` to trust the certificate.</span></span>

### <a name="https-redirection-and-enforcement"></a><span data-ttu-id="52540-148">Redirection et application du protocole HTTPS</span><span class="sxs-lookup"><span data-stu-id="52540-148">HTTPS redirection and enforcement</span></span>

<span data-ttu-id="52540-149">En règle générale, les applications web doivent écouter sur les protocoles HTTP et HTTPS, mais ensuite rediriger tout le trafic HTTP vers HTTPS.</span><span class="sxs-lookup"><span data-stu-id="52540-149">Web apps typically need to listen on both HTTP and HTTPS, but then redirect all HTTP traffic to HTTPS.</span></span> <span data-ttu-id="52540-150">Dans la version 2.1 a été introduit le middleware (intergiciel) de redirection HTTPS spécialisé, qui redirige intelligemment en fonction de la présence de ports de serveur lié ou de configuration.</span><span class="sxs-lookup"><span data-stu-id="52540-150">In 2.1, specialized HTTPS redirection middleware that intelligently redirects based on the presence of configuration or bound server ports has been introduced.</span></span>

<span data-ttu-id="52540-151">Vous pouvez renforcer l’utilisation du protocole HTTPS en utilisant le protocole [HSTS (HTTP Strict Transport Security Protocol)](xref:security/enforcing-ssl#http-strict-transport-security-protocol-hsts).</span><span class="sxs-lookup"><span data-stu-id="52540-151">Use of HTTPS can be further enforced using [HTTP Strict Transport Security Protocol (HSTS)](xref:security/enforcing-ssl#http-strict-transport-security-protocol-hsts).</span></span> <span data-ttu-id="52540-152">Le protocole HSTS indique aux navigateurs de toujours accéder au site via HTTPS.</span><span class="sxs-lookup"><span data-stu-id="52540-152">HSTS instructs browsers to always access the site via HTTPS.</span></span> <span data-ttu-id="52540-153">ASP.NET Core 2.1 ajoute un middleware HSTS qui prend en charge des options pour l’âge maximal, les sous-domaines et la liste de préchargement HSTS.</span><span class="sxs-lookup"><span data-stu-id="52540-153">ASP.NET Core 2.1 adds HSTS middleware that supports options for max age, subdomains, and the HSTS preload list.</span></span>

### <a name="configuration-for-production"></a><span data-ttu-id="52540-154">Configuration pour la production</span><span class="sxs-lookup"><span data-stu-id="52540-154">Configuration for production</span></span>

<span data-ttu-id="52540-155">En production, HTTPS doit être explicitement configuré.</span><span class="sxs-lookup"><span data-stu-id="52540-155">In production, HTTPS must be explicitly configured.</span></span> <span data-ttu-id="52540-156">Dans la version 2.1, le schéma de configuration par défaut pour la configuration HTTPS pour Kestrel a été ajouté.</span><span class="sxs-lookup"><span data-stu-id="52540-156">In 2.1, default configuration schema for configuring HTTPS for Kestrel has been added.</span></span> <span data-ttu-id="52540-157">Les applications peuvent être configurées pour utiliser :</span><span class="sxs-lookup"><span data-stu-id="52540-157">Apps can be configured to use:</span></span>

* <span data-ttu-id="52540-158">Plusieurs points de terminaison, y compris les URL.</span><span class="sxs-lookup"><span data-stu-id="52540-158">Multiple endpoints including the URLs.</span></span> <span data-ttu-id="52540-159">Pour plus d’informations, consultez [Implémentation du serveur web Kestrel : configuration de point de terminaison](xref:fundamentals/servers/kestrel#endpoint-configuration).</span><span class="sxs-lookup"><span data-stu-id="52540-159">For more information, see [Kestrel web server implementation: Endpoint configuration](xref:fundamentals/servers/kestrel#endpoint-configuration).</span></span>
* <span data-ttu-id="52540-160">Le certificat à utiliser pour le protocole HTTPS à partir d’un fichier sur disque ou d’un magasin de certificats.</span><span class="sxs-lookup"><span data-stu-id="52540-160">The certificate to use for HTTPS either from a file on disk or from a certificate store.</span></span>

## <a name="gdpr"></a><span data-ttu-id="52540-161">RGPD</span><span class="sxs-lookup"><span data-stu-id="52540-161">GDPR</span></span>

<span data-ttu-id="52540-162">ASP.NET Core fournit des API et des modèles qui aident à satisfaire à certaines des exigences du [Règlement général sur la protection des données (RGPD)](https://www.eugdpr.org/).</span><span class="sxs-lookup"><span data-stu-id="52540-162">ASP.NET Core provides APIs and templates to help meet some of the [EU General Data Protection Regulation (GDPR)](https://www.eugdpr.org/) requirements.</span></span> <span data-ttu-id="52540-163">Pour plus d’informations, consultez [Prise en charge du RGPD dans ASP.NET Core](xref:security/gdpr).</span><span class="sxs-lookup"><span data-stu-id="52540-163">For more information, see [GDPR support in ASP.NET Core](xref:security/gdpr).</span></span> <span data-ttu-id="52540-164">Un [exemple d’application](https://github.com/aspnet/Docs/tree/live/aspnetcore/security/gdpr/sample) montre comment utiliser et tester la plupart des API et points d’extension RGPD ajoutés aux modèles ASP.NET Core 2.1.</span><span class="sxs-lookup"><span data-stu-id="52540-164">A [sample app](https://github.com/aspnet/Docs/tree/live/aspnetcore/security/gdpr/sample) shows how to use and lets you test most of the GDPR extension points and APIs added to the ASP.NET Core 2.1 templates.</span></span>

## <a name="integration-tests"></a><span data-ttu-id="52540-165">Tests d’intégration</span><span class="sxs-lookup"><span data-stu-id="52540-165">Integration tests</span></span>

<span data-ttu-id="52540-166">Un nouveau package est introduit qui simplifie la création et l’exécution de tests.</span><span class="sxs-lookup"><span data-stu-id="52540-166">A new package is introduced that streamlines test creation and execution.</span></span> <span data-ttu-id="52540-167">Le package [Microsoft.AspNetCore.Mvc.Testing](https://www.nuget.org/packages/Microsoft.AspNetCore.Mvc.Testing/) gère les tâches suivantes :</span><span class="sxs-lookup"><span data-stu-id="52540-167">The [Microsoft.AspNetCore.Mvc.Testing](https://www.nuget.org/packages/Microsoft.AspNetCore.Mvc.Testing/) package handles the following tasks:</span></span>

* <span data-ttu-id="52540-168">Il copie le fichier de dépendance (*\*.deps*) à partir de l’application testée dans le dossier *bin* du projet de test.</span><span class="sxs-lookup"><span data-stu-id="52540-168">Copies the dependency file (*\*.deps*) from the tested app into the test project's *bin* folder.</span></span>
* <span data-ttu-id="52540-169">Il définit la racine du contenu sur la racine du projet de l’application testée afin que soient trouvés les pages/vues et fichiers statiques quand les tests sont exécutés.</span><span class="sxs-lookup"><span data-stu-id="52540-169">Sets the content root to the tested app's project root so that static files and pages/views are found when the tests are executed.</span></span>
* <span data-ttu-id="52540-170">Il fournit la classe [WebApplicationFactory](/dotnet/api/microsoft.aspnetcore.mvc.testing.webapplicationfactory-1) afin de simplifier l’amorçage de l’application testée avec [TestServer](/dotnet/api/microsoft.aspnetcore.testhost.testserver).</span><span class="sxs-lookup"><span data-stu-id="52540-170">Provides the [WebApplicationFactory](/dotnet/api/microsoft.aspnetcore.mvc.testing.webapplicationfactory-1) class to streamline bootstrapping the tested app with [TestServer](/dotnet/api/microsoft.aspnetcore.testhost.testserver).</span></span>

<span data-ttu-id="52540-171">Le test suivant utilise [xUnit](https://xunit.github.io/) pour vérifier que la page Index se charge avec un code d’état de réussite et avec l’en-tête Content-Type correct :</span><span class="sxs-lookup"><span data-stu-id="52540-171">The following test uses [xUnit](https://xunit.github.io/) to check that the Index page loads with a success status code and with the correct Content-Type header:</span></span>

```csharp
public class BasicTests
    : IClassFixture<WebApplicationFactory<RazorPagesProject.Startup>>
{
    private readonly HttpClient _client;

    public BasicTests(WebApplicationFactory<RazorPagesProject.Startup> factory)
    {
        _client = factory.CreateClient();
    }

    [Fact]
    public async Task GetHomePage()
    {
        // Act
        var response = await _client.GetAsync("/");

        // Assert
        response.EnsureSuccessStatusCode(); // Status Code 200-299
        Assert.Equal("text/html; charset=utf-8",
            response.Content.Headers.ContentType.ToString());
    }
}
```

<span data-ttu-id="52540-172">Pour plus d’informations, consultez la rubrique [Tests d’intégration](xref:test/integration-tests).</span><span class="sxs-lookup"><span data-stu-id="52540-172">For more information, see the [Integration tests](xref:test/integration-tests) topic.</span></span>

## <a name="apicontroller-actionresultt"></a><span data-ttu-id="52540-173">[ApiController], ActionResult\<T></span><span class="sxs-lookup"><span data-stu-id="52540-173">[ApiController], ActionResult\<T></span></span>

<span data-ttu-id="52540-174">ASP.NET Core 2.1 ajoute de nouvelles conventions de programmation qui facilitent la génération d’API web propres et descriptives.</span><span class="sxs-lookup"><span data-stu-id="52540-174">ASP.NET Core 2.1 adds new programming conventions that make it easier to build clean and descriptive web APIs.</span></span> <span data-ttu-id="52540-175">`ActionResult<T>` est un nouveau type qui permet à une application de retourner soit un type de réponse, soit tout autre résultat d’action (à l’image d’IActionResult) tout en indiquant toujours le type de réponse.</span><span class="sxs-lookup"><span data-stu-id="52540-175">`ActionResult<T>` is a new type added to allow an app to return either a response type or any other action result (similar to IActionResult), while still indicating the response type.</span></span> <span data-ttu-id="52540-176">L’attribut `[ApiController]` a également été ajouté comme moyen d’accepter des comportements et des conventions propres aux API web.</span><span class="sxs-lookup"><span data-stu-id="52540-176">The `[ApiController]` attribute has also been added as the way to opt in to Web API-specific conventions and behaviors.</span></span>

<span data-ttu-id="52540-177">Pour plus d’informations, consultez [Créer des API web avec ASP.NET Core](xref:web-api/index).</span><span class="sxs-lookup"><span data-stu-id="52540-177">For more information, see [Build Web APIs with ASP.NET Core](xref:web-api/index).</span></span>

## <a name="ihttpclientfactory"></a><span data-ttu-id="52540-178">IHttpClientFactory</span><span class="sxs-lookup"><span data-stu-id="52540-178">IHttpClientFactory</span></span>

<span data-ttu-id="52540-179">ASP.NET Core 2.1 inclut un nouveau service `IHttpClientFactory` qui facilite la configuration et l’utilisation d’instances de `HttpClient` dans les applications.</span><span class="sxs-lookup"><span data-stu-id="52540-179">ASP.NET Core 2.1 includes a new `IHttpClientFactory` service that makes it easier to configure and consume instances of `HttpClient` in apps.</span></span> <span data-ttu-id="52540-180">`HttpClient` intègre déjà le concept de délégation des gestionnaires qui pourraient être liés ensemble pour les requêtes HTTP sortantes.</span><span class="sxs-lookup"><span data-stu-id="52540-180">`HttpClient` already has the concept of delegating handlers that could be linked together for outgoing HTTP requests.</span></span> <span data-ttu-id="52540-181">La fabrique :</span><span class="sxs-lookup"><span data-stu-id="52540-181">The factory:</span></span>

* <span data-ttu-id="52540-182">Rend plus intuitive l’inscription des instances de `HttpClient` par client nommé.</span><span class="sxs-lookup"><span data-stu-id="52540-182">Makes registering of instances of `HttpClient` per named client more intuitive.</span></span>
* <span data-ttu-id="52540-183">Implémente un gestionnaire Polly qui permet d’utiliser des stratégies Polly pour des fonctionnalités telles que Retry (nouvelle tentative) ou CircuitBreaker (disjoncteur).</span><span class="sxs-lookup"><span data-stu-id="52540-183">Implements a Polly handler that allows Polly policies to be used for Retry, CircuitBreakers, etc.</span></span>

<span data-ttu-id="52540-184">Pour plus d’informations, consultez [Lancer des requêtes HTTP](xref:fundamentals/http-requests).</span><span class="sxs-lookup"><span data-stu-id="52540-184">For more information, see [Initiate HTTP Requests](xref:fundamentals/http-requests).</span></span>

## <a name="kestrel-transport-configuration"></a><span data-ttu-id="52540-185">Configuration du transport Kestrel</span><span class="sxs-lookup"><span data-stu-id="52540-185">Kestrel transport configuration</span></span>

<span data-ttu-id="52540-186">Dans ASP.NET Core 2.1, le transport par défaut de Kestrel n’est plus basé sur Libuv, mais sur des sockets managés.</span><span class="sxs-lookup"><span data-stu-id="52540-186">With the release of ASP.NET Core 2.1, Kestrel's default transport is no longer based on Libuv but instead based on managed sockets.</span></span> <span data-ttu-id="52540-187">Pour plus d’informations, consultez [Implémentation du serveur web Kestrel : configuration du transport](xref:fundamentals/servers/kestrel#transport-configuration).</span><span class="sxs-lookup"><span data-stu-id="52540-187">For more information, see [Kestrel web server implementation: Transport configuration](xref:fundamentals/servers/kestrel#transport-configuration).</span></span>

## <a name="generic-host-builder"></a><span data-ttu-id="52540-188">Générateur d’hôte générique</span><span class="sxs-lookup"><span data-stu-id="52540-188">Generic host builder</span></span>

<span data-ttu-id="52540-189">Le générateur d’hôte générique (`HostBuilder`) a été introduit.</span><span class="sxs-lookup"><span data-stu-id="52540-189">The Generic Host Builder (`HostBuilder`) has been introduced.</span></span> <span data-ttu-id="52540-190">Ce générateur peut être utilisé pour les applications qui ne traitent pas les requêtes HTTP (messagerie, les tâches en arrière-plan, etc.).</span><span class="sxs-lookup"><span data-stu-id="52540-190">This builder can be used for apps that don't process HTTP requests (Messaging, background tasks, etc.).</span></span>

<span data-ttu-id="52540-191">Pour plus d’informations, consultez [Hôte générique .NET](xref:fundamentals/host/generic-host).</span><span class="sxs-lookup"><span data-stu-id="52540-191">For more information, see [.NET Generic Host](xref:fundamentals/host/generic-host).</span></span>

## <a name="updated-spa-templates"></a><span data-ttu-id="52540-192">Modèles SPA mis à jour</span><span class="sxs-lookup"><span data-stu-id="52540-192">Updated SPA templates</span></span>

<span data-ttu-id="52540-193">Les modèles d’applications monopages pour Angular, React et React avec Redux sont mis à jour pour utiliser les systèmes de génération et les structures de projet standard pour chaque framework.</span><span class="sxs-lookup"><span data-stu-id="52540-193">The Single Page Application templates for Angular, React, and React with Redux are updated to use the standard project structures and build systems for each framework.</span></span>

<span data-ttu-id="52540-194">Le modèle Angular est basé sur l’interface CLI Angular, tandis que les modèles React sont basés sur create-react-app.</span><span class="sxs-lookup"><span data-stu-id="52540-194">The Angular template is based on the Angular CLI, and the React templates are based on create-react-app.</span></span>
<span data-ttu-id="52540-195">Pour plus d’informations, consultez [Utiliser les modèles d’applications monopages avec ASP.NET Core](xref:spa/index).</span><span class="sxs-lookup"><span data-stu-id="52540-195">For more information, see [Use the Single Page Application templates with ASP.NET Core](xref:spa/index).</span></span>

## <a name="razor-pages-search-for-razor-assets"></a><span data-ttu-id="52540-196">Recherche Razor Pages de ressources Razor</span><span class="sxs-lookup"><span data-stu-id="52540-196">Razor Pages search for Razor assets</span></span>

<span data-ttu-id="52540-197">Dans la version 2.1, Razor Pages recherche les ressources Razor (par exemple, les dispositions et pages partielles) dans les répertoires suivants dans l’ordre indiqué :</span><span class="sxs-lookup"><span data-stu-id="52540-197">In 2.1, Razor Pages search for Razor assets (such as layouts and partials) in the following directories in the listed order:</span></span>

1. <span data-ttu-id="52540-198">Dossier Pages en cours.</span><span class="sxs-lookup"><span data-stu-id="52540-198">Current Pages folder.</span></span>
1. <span data-ttu-id="52540-199">*/Pages/Shared/*</span><span class="sxs-lookup"><span data-stu-id="52540-199">*/Pages/Shared/*</span></span>
1. <span data-ttu-id="52540-200">*/Views/Shared/*</span><span class="sxs-lookup"><span data-stu-id="52540-200">*/Views/Shared/*</span></span>

## <a name="razor-pages-in-an-area"></a><span data-ttu-id="52540-201">Razor Pages dans une zone</span><span class="sxs-lookup"><span data-stu-id="52540-201">Razor Pages in an area</span></span>

<span data-ttu-id="52540-202">Razor Pages prend désormais en charge les [zones](xref:mvc/controllers/areas).</span><span class="sxs-lookup"><span data-stu-id="52540-202">Razor Pages now support [areas](xref:mvc/controllers/areas).</span></span> <span data-ttu-id="52540-203">Pour obtenir un exemple de zones, créez une application web Razor Pages avec des comptes d’utilisateur individuels.</span><span class="sxs-lookup"><span data-stu-id="52540-203">To see an example of areas, create a new Razor Pages web app with individual user accounts.</span></span> <span data-ttu-id="52540-204">Une application web Razor Pages avec des comptes d’utilisateur individuels inclut */Areas/Identity/Pages*.</span><span class="sxs-lookup"><span data-stu-id="52540-204">A Razor Pages web app with individual user accounts includes */Areas/Identity/Pages*.</span></span>

## <a name="mvc-compatibility-version"></a><span data-ttu-id="52540-205">Version de compatibilité MVC</span><span class="sxs-lookup"><span data-stu-id="52540-205">MVC compatibility version</span></span>

<span data-ttu-id="52540-206">La méthode <xref:Microsoft.Extensions.DependencyInjection.MvcCoreMvcBuilderExtensions.SetCompatibilityVersion*> permet à une application d’accepter ou de refuser les changements de comportement potentiellement cassants introduits dans ASP.NET Core MVC 2.1 ou version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="52540-206">The <xref:Microsoft.Extensions.DependencyInjection.MvcCoreMvcBuilderExtensions.SetCompatibilityVersion*> method allows an app to opt-in or opt-out of potentially breaking behavior changes introduced in ASP.NET Core MVC 2.1 or later.</span></span>

<span data-ttu-id="52540-207">Pour plus d'informations, consultez <xref:mvc/compatibility-version>.</span><span class="sxs-lookup"><span data-stu-id="52540-207">For more information, see <xref:mvc/compatibility-version>.</span></span>

## <a name="migrate-from-20-to-21"></a><span data-ttu-id="52540-208">Migrer depuis la version 2.0 vers la version 2.1</span><span class="sxs-lookup"><span data-stu-id="52540-208">Migrate from 2.0 to 2.1</span></span>

<span data-ttu-id="52540-209">Consultez [Migrer depuis ASP.NET Core 2.0 vers 2.1](xref:migration/20_21).</span><span class="sxs-lookup"><span data-stu-id="52540-209">See [Migrate from ASP.NET Core 2.0 to 2.1](xref:migration/20_21).</span></span>

## <a name="additional-information"></a><span data-ttu-id="52540-210">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="52540-210">Additional information</span></span>

<span data-ttu-id="52540-211">Pour obtenir la liste complète des modifications, consultez les [Notes de publication d’ASP.NET Core 2.1 ](https://github.com/aspnet/Home/releases/tag/2.1.0).</span><span class="sxs-lookup"><span data-stu-id="52540-211">For the complete list of changes, see the [ASP.NET Core 2.1 Release Notes](https://github.com/aspnet/Home/releases/tag/2.1.0).</span></span>