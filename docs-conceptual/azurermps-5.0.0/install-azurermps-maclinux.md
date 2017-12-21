---
title: "Installer et configurer Azure PowerShell sur macOS et Linux │ Microsoft Docs"
description: "Comment installer et configurer Azure PowerShell pour la première utilisation sur macOS et Linux."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: 94b39c18acaca7a4b17b5207feed025442665acc
ms.sourcegitcommit: 358d260a867c6ee2e8700b91f776ba4f1b0e24a5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/11/2017
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a><span data-ttu-id="433ba-103">Installer et configurer Azure PowerShell sur macOS et Linux</span><span class="sxs-lookup"><span data-stu-id="433ba-103">Install and configure Azure PowerShell on macOS and Linux</span></span>

<span data-ttu-id="433ba-104">Il est désormais possible d’installer PowerShell 6 (bêta) et Azure PowerShell sur des plateformes non-Windows.</span><span class="sxs-lookup"><span data-stu-id="433ba-104">It is now possible to install PowerShell 6 (beta) and Azure PowerShell on non-Windows platforms.</span></span>
<span data-ttu-id="433ba-105">Le processus d’installation d’Azure PowerShell sur macOS et Linux est presque le même que sur Windows, sauf que vous devez d’abord installer PowerShell 6 (bêta).</span><span class="sxs-lookup"><span data-stu-id="433ba-105">The process of installing Azure PowerShell on macOS and Linux is not that different from Windows, however, you must first install PowerShell 6 (beta).</span></span>

> [!NOTE]

> <span data-ttu-id="433ba-106">Actuellement, PowerShell 6 (bêta) et Azure PowerShell pour .NET Core sont toujours en version bêta.</span><span class="sxs-lookup"><span data-stu-id="433ba-106">At this time, both PowerShell 6 (beta) and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="433ba-107">La prise en charge de ces produits est limitée.</span><span class="sxs-lookup"><span data-stu-id="433ba-107">Support for these products is limited.</span></span> <span data-ttu-id="433ba-108">Si vous rencontrez des problèmes ou que vous découvrez des bogues, vous pouvez nous les signaler dans GitHub.</span><span class="sxs-lookup"><span data-stu-id="433ba-108">If you have problems or discover bugs, please file Issues in GitHub.</span></span>
>
> * [<span data-ttu-id="433ba-109">Problèmes pour PowerShell 6 (bêta)</span><span class="sxs-lookup"><span data-stu-id="433ba-109">Issues for PowerShell 6 (beta)</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="433ba-110">Problèmes pour Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="433ba-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-6-beta"></a><span data-ttu-id="433ba-111">Étape 1 : Installer PowerShell 6 (bêta)</span><span class="sxs-lookup"><span data-stu-id="433ba-111">Step 1: Install PowerShell 6 (beta)</span></span>

<span data-ttu-id="433ba-112">Le processus d’installation de PowerShell 6 (bêta) varie selon le système d’exploitation cible.</span><span class="sxs-lookup"><span data-stu-id="433ba-112">The process of installing PowerShell 6 (beta) on varies depending on the target operating system.</span></span>
<span data-ttu-id="433ba-113">S’il est possible d’installer PowerShell 6 (bêta) sur Windows, cet article est néanmoins centré sur macOS et Linux.</span><span class="sxs-lookup"><span data-stu-id="433ba-113">While it is possible to install PowerShell 6 (beta) on Windows, this article focuses on macOS and Linux.</span></span> <span data-ttu-id="433ba-114">Si vous voulez utiliser Azure PowerShell sur Windows, consultez l’article sur [l’installation](./install-azurerm-ps.md) pour Windows.</span><span class="sxs-lookup"><span data-stu-id="433ba-114">If you want to use Azure PowerShell on Windows, see the [install](./install-azurerm-ps.md) article for Windows.</span></span>

<span data-ttu-id="433ba-115">Pour installer **PowerShell 6** (bêta) sur Linux ou macOS, vous devez :</span><span class="sxs-lookup"><span data-stu-id="433ba-115">To install **PowerShell 6** (beta) on Linux or macOS, you need to:</span></span>

1. <span data-ttu-id="433ba-116">Obtenir PowerShell pour le système d’exploitation et la version spécifiques auprès de [GitHub](https://github.com/powershell/powershell#get-powershell)</span><span class="sxs-lookup"><span data-stu-id="433ba-116">Get PowerShell for the specific OS and version, from [GitHub](https://github.com/powershell/powershell#get-powershell)</span></span>
2. <span data-ttu-id="433ba-117">Suivre les instructions d’installation</span><span class="sxs-lookup"><span data-stu-id="433ba-117">Follow the installation instructions</span></span>
   - [<span data-ttu-id="433ba-118">Linux</span><span class="sxs-lookup"><span data-stu-id="433ba-118">Linux</span></span>](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md)
   - [<span data-ttu-id="433ba-119">macOS</span><span class="sxs-lookup"><span data-stu-id="433ba-119">macOS</span></span>](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md#macos-1012)

## <a name="step-2-install-azure-powershell-for-net-core"></a><span data-ttu-id="433ba-120">Étape 2 : Installer Azure PowerShell pour .NET Core</span><span class="sxs-lookup"><span data-stu-id="433ba-120">Step 2: Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="433ba-121">PowerShell 6 (bêta) est fourni avec le module PowerShellGet déjà installé.</span><span class="sxs-lookup"><span data-stu-id="433ba-121">PowerShell 6 (beta) comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="433ba-122">Ceci facilite l’installation de n’importe quel module publié dans PowerShell Gallery.</span><span class="sxs-lookup"><span data-stu-id="433ba-122">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="433ba-123">Pour installer Azure PowerShell, ouvrez une nouvelle session PowerShell et exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="433ba-123">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a><span data-ttu-id="433ba-124">Étape 3 : Charger le module AzureRM.Netcore</span><span class="sxs-lookup"><span data-stu-id="433ba-124">Step 3: Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="433ba-125">Une fois le module installé, vous devez le charger dans votre session PowerShell.</span><span class="sxs-lookup"><span data-stu-id="433ba-125">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="433ba-126">Les modules sont chargés à l’aide de l’applet de commande `Import-Module`, comme suit :</span><span class="sxs-lookup"><span data-stu-id="433ba-126">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
```

<span data-ttu-id="433ba-127">Une fois l’importation terminée, vous pouvez tester votre module nouvellement installé en essayant de vous connecter à Azure avec la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="433ba-127">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Login-AzureRMAccount
```

<span data-ttu-id="433ba-128">La commande ci-dessus vous invite à accéder à `https://aka.ms/devicelogin` et à entrer le code fourni.</span><span class="sxs-lookup"><span data-stu-id="433ba-128">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="433ba-129">Applets de commande disponibles</span><span class="sxs-lookup"><span data-stu-id="433ba-129">Available cmdlets</span></span>

<span data-ttu-id="433ba-130">Les modules Azure PowerShell pour .NET Standard sont en cours de développement.</span><span class="sxs-lookup"><span data-stu-id="433ba-130">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="433ba-131">Ces modules ne fournissent pas l’ensemble des applets de commande qui sont disponibles pour la version Windows des modules.</span><span class="sxs-lookup"><span data-stu-id="433ba-131">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="433ba-132">Les fonctions suivantes sont implémentées dans les modules AzureRM.Netcore :</span><span class="sxs-lookup"><span data-stu-id="433ba-132">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="433ba-133">Account Management</span><span class="sxs-lookup"><span data-stu-id="433ba-133">Account management</span></span>
  - <span data-ttu-id="433ba-134">Se connecter avec un compte Microsoft, un compte d’organisation ou un principal du service via Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="433ba-134">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="433ba-135">Enregistrer les informations d’identification sur disque avec Save-AzureRmContext et charger les informations d’identification enregistrées avec Import-AzureRmContext</span><span class="sxs-lookup"><span data-stu-id="433ba-135">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="433ba-136">Environnement</span><span class="sxs-lookup"><span data-stu-id="433ba-136">Environment</span></span>
  - <span data-ttu-id="433ba-137">Obtenir les différents environnements Microsoft Azure prédéfinis</span><span class="sxs-lookup"><span data-stu-id="433ba-137">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="433ba-138">Ajouter/définir/supprimer des environnements personnalisés (comme vos environnements Azure Stack ou Windows Azure Pack)</span><span class="sxs-lookup"><span data-stu-id="433ba-138">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="433ba-139">Applets de commande de plan de gestion pour les services Azure avec les interfaces Resource Manager et Gestion des services.</span><span class="sxs-lookup"><span data-stu-id="433ba-139">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="433ba-140">Machine virtuelle</span><span class="sxs-lookup"><span data-stu-id="433ba-140">Virtual Machine</span></span>
  - <span data-ttu-id="433ba-141">App Service (sites web)</span><span class="sxs-lookup"><span data-stu-id="433ba-141">App Service (Websites)</span></span>
  - <span data-ttu-id="433ba-142">Base de données SQL</span><span class="sxs-lookup"><span data-stu-id="433ba-142">SQL Database</span></span>
  - <span data-ttu-id="433ba-143">Storage</span><span class="sxs-lookup"><span data-stu-id="433ba-143">Storage</span></span>
  - <span data-ttu-id="433ba-144">Réseau</span><span class="sxs-lookup"><span data-stu-id="433ba-144">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="433ba-145">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="433ba-145">Next Steps</span></span>

<span data-ttu-id="433ba-146">Pour plus d’informations sur l’utilisation d’Azure PowerShell, consultez l’article [Bien démarrer avec Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="433ba-146">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>