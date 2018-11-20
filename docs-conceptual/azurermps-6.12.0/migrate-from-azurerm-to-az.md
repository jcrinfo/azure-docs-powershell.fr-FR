---
title: Migrer des scripts Azure PowerShell depuis AzureRM vers Az
description: Découvrez les étapes et les outils pour effectuer une migration des scripts à partir du module AzureRM vers le nouveau module Az.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 0c73e7ac1d47a2a97b6136fa481d0adce8de33db
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574411"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a><span data-ttu-id="5001c-103">Migrer de AzureRM vers Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="5001c-103">Migrate from AzureRM to Azure PowerShell Az</span></span>

<span data-ttu-id="5001c-104">Le module Az a la même parité des fonctionnalités que AzureRM, mais il utilise des noms de cmdlets plus courts et plus cohérents.</span><span class="sxs-lookup"><span data-stu-id="5001c-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="5001c-105">Les scripts écrits pour les cmdlets AzureRM ne fonctionnent pas automatiquement avec le nouveau module.</span><span class="sxs-lookup"><span data-stu-id="5001c-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="5001c-106">Pour faciliter la transition, Az propose des outils qui vous permettent d’exécuter vos scripts existants à l’aide d’AzureRM.</span><span class="sxs-lookup"><span data-stu-id="5001c-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="5001c-107">Il n’existe pas une migration vers un nouveau jeu de commandes qui soit pratique, mais cet article vous aide à bien démarrer la transition vers le nouveau module.</span><span class="sxs-lookup"><span data-stu-id="5001c-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="5001c-108">Assurez-vous que vos scripts existants fonctionnent avec la dernière version d’AzureRM</span><span class="sxs-lookup"><span data-stu-id="5001c-108">Ensure your existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="5001c-109">Il s’agit de l’étape la plus importante.</span><span class="sxs-lookup"><span data-stu-id="5001c-109">This is the most important step!</span></span> <span data-ttu-id="5001c-110">Exécutez vos scripts existants et assurez-vous qu’ils fonctionnent avec la _dernière_ version d’AzureRM (__6.12.0__).</span><span class="sxs-lookup"><span data-stu-id="5001c-110">Run your existing scripts, and make sure that they work with the _latest_ release of AzureRM (__6.12.0__).</span></span> <span data-ttu-id="5001c-111">Si vos scripts ne fonctionnent pas, veuillez lire le [guide de migration AzureRM](migration-guide.6.0.0.md).</span><span class="sxs-lookup"><span data-stu-id="5001c-111">If your scripts don't work, make sure to read the [AzureRM migration guide](migration-guide.6.0.0.md).</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="5001c-112">Installer le module Azure PowerShell Az</span><span class="sxs-lookup"><span data-stu-id="5001c-112">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="5001c-113">La première étape consiste à installer le module Az sur votre plateforme.</span><span class="sxs-lookup"><span data-stu-id="5001c-113">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="5001c-114">Pour installer Az, vous devez désinstaller AzureRM.</span><span class="sxs-lookup"><span data-stu-id="5001c-114">To install Az, you need to uninstall AzureRM.</span></span>
<span data-ttu-id="5001c-115">Dans les étapes suivantes, vous découvrez comment poursuivre l’exécution de vos scripts existants et activer la compatibilité pour les anciens noms de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5001c-115">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="5001c-116">Pour installer le module Azure PowerShell Az, suivez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="5001c-116">To install the Azure PowerShell Az module, follow these steps:</span></span>

* <span data-ttu-id="5001c-117">[Désinstaller le module AzureRM](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="5001c-117">[Uninstall the AzureRM module](uninstall-azurerm-ps.md).</span></span> <span data-ttu-id="5001c-118">Assurez-vous de supprimer _toutes les_ versions installées d’AzureRM, et non pas simplement la plus récente.</span><span class="sxs-lookup"><span data-stu-id="5001c-118">Make sure that you remove _all_ installed versions of AzureRM, not just the most recent version.</span></span>
* [<span data-ttu-id="5001c-119">Installer le module Az</span><span class="sxs-lookup"><span data-stu-id="5001c-119">Install the Az module</span></span>](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><span data-ttu-id="5001c-120"><a name="aliases"/>Activer le mode alias d’AzureRM</span><span class="sxs-lookup"><span data-stu-id="5001c-120"><a name="aliases"/>Enable AzureRM alias mode</span></span>

<span data-ttu-id="5001c-121">Une fois AzureRM désinstallé et vos scripts compatibles avec la dernière version d’AzureRM, vous pouvez procéder à l’activation du mode de compatibilité pour le module Az.</span><span class="sxs-lookup"><span data-stu-id="5001c-121">With AzureRM uninstalled and your scripts working with the latest AzureRM version, now is the time to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="5001c-122">La compatibilité est activée à l’aide de la commande :</span><span class="sxs-lookup"><span data-stu-id="5001c-122">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="5001c-123">Les alias rendent possible l’utilisation des anciens noms de cmdlets avec le module `Az` installé.</span><span class="sxs-lookup"><span data-stu-id="5001c-123">Aliases enable the ability to use old cmdlet names with the `Az` module installed.</span></span> <span data-ttu-id="5001c-124">Ces alias sont écrits dans le profil utilisateur pour l’étendue sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="5001c-124">These aliases are written to the user profile for the selected scope.</span></span> <span data-ttu-id="5001c-125">S’il n’en existe aucun, un profil utilisateur est créé.</span><span class="sxs-lookup"><span data-stu-id="5001c-125">If no user profile exists, one is created.</span></span>

> [!WARNING]
>
> <span data-ttu-id="5001c-126">Vous pouvez utiliser une autre `-Scope` pour cette commande, mais ce n’est pas conseillé !</span><span class="sxs-lookup"><span data-stu-id="5001c-126">You can use a different `-Scope` for this command, but it's not recommended!</span></span> <span data-ttu-id="5001c-127">Les alias sont écrits dans le profil utilisateur pour l’étendue sélectionnée. Ainsi, poursuivez leur activation pour une étendue aussi limitée que possible.</span><span class="sxs-lookup"><span data-stu-id="5001c-127">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="5001c-128">L’activation des alias à l’échelle du système peut également entraîner des problèmes pour d’autres utilisateurs qui ont installé `AzureRM` dans leur étendue locale.</span><span class="sxs-lookup"><span data-stu-id="5001c-128">Enabling aliases system-wide could also cause issues for other users which have `AzureRM` installed in their local scope.</span></span>

<span data-ttu-id="5001c-129">Une fois le mode alias activé, exécutez une nouvelle fois les scripts pour confirmer qu’ils fonctionnent toujours comme prévu.</span><span class="sxs-lookup"><span data-stu-id="5001c-129">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span> 

## <a name="change-module-imports-and-cmdlet-names"></a><span data-ttu-id="5001c-130">Modifier les importations de modules et les noms de cmdlets</span><span class="sxs-lookup"><span data-stu-id="5001c-130">Change module imports and cmdlet names</span></span>

<span data-ttu-id="5001c-131">En règle générale, les noms de module ont été modifiés pour que `AzureRM` et `Azure` deviennent `Az`et il en va de même pour les cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5001c-131">In general, the module names have been changed so that `AzureRM` and `Azure` become `Az`, and the same for cmdlets.</span></span>
<span data-ttu-id="5001c-132">Par exemple, le module `AzureRM.Compute` a été renommé `Az.Compute`.</span><span class="sxs-lookup"><span data-stu-id="5001c-132">For example, the `AzureRM.Compute` module has been renamed to `Az.Compute`.</span></span> <span data-ttu-id="5001c-133">`New-AzureRmVM` est devenu `New-AzVM` et `Get-AzureStorageBlob` est désormais `Get-AzStorageBlob`.</span><span class="sxs-lookup"><span data-stu-id="5001c-133">`New-AzureRmVM` has become `New-AzVM`, and `Get-AzureStorageBlob` is now `Get-AzStorageBlob`.</span></span>

<span data-ttu-id="5001c-134">Il existe des exceptions à cette modification de dénomination que vous devez connaître avant de renommer quoi que ce soit :</span><span class="sxs-lookup"><span data-stu-id="5001c-134">There are exceptions to this naming change that you should be aware of before doing any renaming:</span></span>

| <span data-ttu-id="5001c-135">Module AzureRM</span><span class="sxs-lookup"><span data-stu-id="5001c-135">AzureRM module</span></span> | <span data-ttu-id="5001c-136">Module Az</span><span class="sxs-lookup"><span data-stu-id="5001c-136">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="5001c-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="5001c-137">AzureRM.DataFactories</span></span> | <span data-ttu-id="5001c-138">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5001c-138">Az.DataFactory</span></span> |
| <span data-ttu-id="5001c-139">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5001c-139">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="5001c-140">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="5001c-140">Az.DataFactory</span></span> |
| <span data-ttu-id="5001c-141">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5001c-141">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="5001c-142">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5001c-142">Az.RecoveryServices</span></span> |
| <span data-ttu-id="5001c-143">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="5001c-143">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="5001c-144">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5001c-144">Az.RecoveryServices</span></span> |

## <a name="summary"></a><span data-ttu-id="5001c-145">Résumé</span><span class="sxs-lookup"><span data-stu-id="5001c-145">Summary</span></span>

<span data-ttu-id="5001c-146">Suivez les étapes suivantes pour mettre à jour tous vos scripts existants et utiliser le nouveau module.</span><span class="sxs-lookup"><span data-stu-id="5001c-146">By following these steps, you can update all of your existing scripts to use the new module.</span></span> <span data-ttu-id="5001c-147">Si vous avez des questions concernant ces étapes ou rencontrez des problèmes rendant la migration difficile, veuillez laisser un commentaire sur cet article afin que nous puissions améliorer les instructions.</span><span class="sxs-lookup"><span data-stu-id="5001c-147">If you have any questions or problems with these steps that made your migration difficult, please comment on this article so that we can improve the instructions.</span></span>