---
title: Installer et configurer Azure PowerShell | Microsoft Docs
description: Comment installer et configurer Azure PowerShell pour la première utilisation.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/27/2018
ms.openlocfilehash: 3acae0cc03e5af34fdf005ea644e0932278d471a
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2018
ms.locfileid: "52258466"
---
# <a name="install-and-configure-azure-powershell"></a>Installation et configuration d'Azure PowerShell

La méthode recommandée est d’installer Azure PowerShell à partir de PowerShell Gallery.

## <a name="step-1-install-powershellget"></a>Étape 1 : Installer PowerShellGet

Pour installer des éléments à partir de PowerShell Gallery, vous avez besoin du module PowerShellGet. Vérifiez que votre système a la version appropriée de PowerShellGet et qu’il présente toute la configuration requise. Exécutez la commande suivante pour vérifier que PowerShellGet est installé sur votre système.

```powershell-interactive
Get-Module -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

Vous devez obtenir un graphique similaire à la sortie suivante :

```Output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

Vous avez besoin de PowerShellGet version 1.1.2.0 ou versions ultérieures. Pour mettre à jour PowerShellGet, utilisez la commande suivante :

```powershell-interactive
Install-Module PowerShellGet -Force
```

Si PowerShellGet n’est pas installé, consultez la section [Comment obtenir PowerShellGet](#how-to-get-powershellget) dans cet article.

> [!NOTE]
> L’utilisation de PowerShellGet nécessite une stratégie d’exécution pour exécuter les scripts. Pour plus d’informations sur la stratégie d’exécution de PowerShell, consultez [About Execution Policy](/powershell/module/microsoft.powershell.core/about/about_execution_policies) (À propos des stratégies d’exécution).

## <a name="step-2-install-azure-powershell"></a>Étape 2 : Installer Azure PowerShell

L’installation d’Azure PowerShell à partir de PowerShell Gallery nécessite des privilèges élevés. Exécutez la commande suivante à partir d’une session PowerShell avec élévation de privilèges :

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

Par défaut, la galerie PowerShell n’est pas configurée comme un référentiel de confiance pour PowerShellGet. La première fois que vous utilisez PSGallery, le message suivant s’affiche :

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

Répondez « Oui » ou « Oui pour tous » pour poursuivre l’installation.

> [!NOTE]
> Si votre version de NuGet est antérieure à 2.8.5.201, vous êtes invité à télécharger et installer la dernière version de NuGet.

Le module AzureRM est un module cumulatif pour les applets de commande Azure Resource Manager. Quand vous installez le module AzureRM, les autres modules Azure qui n’ont pas encore été installés sont téléchargés et installés à partir de PowerShell Gallery.

Si vous disposez d’une version précédente d’Azure PowerShell, vous pourriez recevoir une erreur. Pour résoudre ce problème, consultez la section [Mise à jour vers une nouvelle version d’Azure PowerShell](#update-azps) de cet article.

## <a name="step-3-load-the-azurerm-module"></a>Étape 3 : Charger le module AzureRM

Une fois le module installé, vous devez le charger dans votre session PowerShell. Vous devez le faire dans une session PowerShell normale (sans élévation de privilèges). Les modules sont chargés à l’aide de l’applet de commande `Import-Module`, comme suit :

```powershell-interactive
Import-Module -Name AzureRM
```

## <a name="next-steps"></a>Étapes suivantes

Pour plus d’informations sur l’utilisation d’Azure PowerShell, consultez les articles suivants :

* [Prise en main d’Azure PowerShell](get-started-azureps.md)

## <a name="frequently-asked-questions"></a>Questions fréquentes (FAQ)

### <a name="how-to-get-powershellget"></a>Comment obtenir PowerShellGet

|Version du SE|Instructions d’installation|
|---|---|
|J’ai Windows 10 ou Windows Server 2016|Intégré à Windows Management Framework (WMF) 5.0 inclus dans le système d’exploitation|
|Je veux effectuer la mise à niveau vers PowerShell 5|[Installer la dernière version de WMF](https://www.microsoft.com/en-us/download/details.aspx?id=54616)|
|Mon ordinateur exécute une version de Windows avec PowerShell 3 ou 4|[Obtenir les modules PackageManagement](http://go.microsoft.com/fwlink/?LinkID=746217)|

### <a name="div-idhelpmechoosechecking-the-version-of-azure-powershell"></a><div id="helpmechoose"/>Vérification de la version d’Azure PowerShell

Bien que nous vous encouragions à effectuer la mise à niveau vers la version la plus récente dès que possible, plusieurs versions d’Azure PowerShell sont prises en charge. Pour déterminer la version d’Azure PowerShell installée, exécutez `Get-Module AzureRM` à partir de la ligne de commande.

```powershell-interactive
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a>Prise en charge des méthodes de déploiement classiques

Si vous avez des déploiements qui utilisent le modèle de déploiement Classic, vous pouvez installer la version Service Management d’Azure PowerShell. Pour plus d’informations, consultez [Installer le module Azure PowerShell Service Management](/powershell/azure/servicemanagement/install-azure-ps). Les modules Azure et AzureRM partagent des dépendances communes. Si vous utilisez des modules Azure et AzureRM, vous devez installer la même version de chaque package.

### <a name="div-idupdate-azpsupdating-to-a-new-version-of-azure-powershell"></a><div id="update-azps"/>Mise à jour vers une nouvelle version d’Azure PowerShell

Si vous avez une version précédente d’Azure PowerShell installée qui inclut le module Gestion des services, vous pourriez recevoir l’erreur suivante :

```Output
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

Comme le message d’erreur l’indique, vous devez utiliser le paramètre -AllowClobber pour installer le module. Utilisez la commande suivante :

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

Pour plus d’informations, consultez la rubrique pour [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).

### <a name="installing-module-versions-side-by-side"></a>Installation de versions de modules côte à côte

La méthode d’installation avec PowerShellGet est la seule qui prend en charge l’installation de plusieurs versions. Utilisez-la, par exemple, si vous avez des scripts écrits à l’aide d’une version précédente d’Azure PowerShell et que vous n’avez pas le temps ou les ressources pour les mettre à jour. Les commandes suivantes illustrent l’installation de plusieurs versions d’Azure PowerShell :

```powershell-interactive
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

Une seule version du module peut être chargée dans une session PowerShell. Vous devez ouvrir une nouvelle fenêtre PowerShell et utiliser `Import-Module` pour importer une version spécifique des applets de commande AzureRM :

```powershell-interactive
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> Les versions 2.1.0 et 1.2.6 sont les premières versions de module conçues pour être installées et utilisées côte à côte. Lors du chargement d’une version antérieure d’Azure PowerShell, des versions incompatibles du module **AzureRM.Profile** sont chargées. Ainsi, les applets de commande vous invitent à vous connecter chaque fois que vous exécutez une applet de commande.

### <a name="other-installation-methods"></a>Autres méthodes d’installation

Pour plus d’informations sur l’installation à l’aide de Web Platform Installer ou du package MSI, consultez [Autres méthodes d’installation](other-install.md)
