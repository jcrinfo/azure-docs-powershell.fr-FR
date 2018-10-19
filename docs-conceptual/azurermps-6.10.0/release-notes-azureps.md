---
title: Journal de modifications Azure PowerShell | Microsoft Docs
description: Il s’agit d’un historique des modifications apportées à Azure PowerShell dans la dernière version.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: 6a33d1a85fc61d0281bf1183163185b0dc4d3a12
ms.sourcegitcommit: f6f5e256143aa6c097de3e57e930d8badea49f30
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2018
ms.locfileid: "49399057"
---
# <a name="release-notes"></a><span data-ttu-id="0be91-103">Notes de publication</span><span class="sxs-lookup"><span data-stu-id="0be91-103">Release notes</span></span>

<span data-ttu-id="0be91-104">Il s’agit de la liste des modifications apportées à Azure PowerShell dans cette version.</span><span class="sxs-lookup"><span data-stu-id="0be91-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6100---october-2018"></a><span data-ttu-id="0be91-105">6.10.0 - Octobre 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-105">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="0be91-106">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-106">Azure.Storage</span></span>
* <span data-ttu-id="0be91-107">Correction d’un problème où le fichier/objet blob de copie ne copie pas les métadonnées lorsque la destination contient des problèmes de métadonnées</span><span class="sxs-lookup"><span data-stu-id="0be91-107">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="0be91-108">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="0be91-108">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="0be91-109">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="0be91-109">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="0be91-110">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0be91-110">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="0be91-111">Prise en charge de Get-AzureRmCognitiveServicesAccountSkus sans compte existant.</span><span class="sxs-lookup"><span data-stu-id="0be91-111">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-112">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-112">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-113">Correction de Get-AzureRmVM -ResourceGroupName <rg> pour retourner plus de 50 résultats si besoin</span><span class="sxs-lookup"><span data-stu-id="0be91-113">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="0be91-114">Ajout d’un exemple de la commande « SimpleParameterSet » à l’aide de cmdlet New-AzureRmVmss.</span><span class="sxs-lookup"><span data-stu-id="0be91-114">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="0be91-115">Correction d’une faute de frappe dans le message de progression d’Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="0be91-115">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="0be91-116">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="0be91-116">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="0be91-117">Mise à jour de la version du Kit de développement logiciel (SDK) ADF .Net vers la version 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="0be91-117">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-118">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-118">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-119">Ajout de la fonctionnalité NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="0be91-119">Added NetworkProfile functionality.</span></span> <span data-ttu-id="0be91-120">nouvelles cmdlets ajoutées</span><span class="sxs-lookup"><span data-stu-id="0be91-120">new cmdlets added</span></span>
    - <span data-ttu-id="0be91-121">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0be91-121">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="0be91-122">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0be91-122">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="0be91-123">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0be91-123">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="0be91-124">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0be91-124">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="0be91-125">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-125">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="0be91-126">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-126">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="0be91-127">Ajout d’un lien d’association de service sur le modèle de sous-réseau</span><span class="sxs-lookup"><span data-stu-id="0be91-127">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="0be91-128">Ajout des cmdlets New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="0be91-128">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="0be91-129">Ajout des cmdlets Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-129">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="0be91-130">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="0be91-130">AzureRM.RedisCache</span></span>
* <span data-ttu-id="0be91-131">Autorisez toutes les chaînes en tant que Paramètre de taille à progresser.</span><span class="sxs-lookup"><span data-stu-id="0be91-131">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="0be91-132">Ajout de P5 dans la fenêtre contextuelle PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="0be91-132">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-133">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-133">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-134">Ajout du paramètre manquant -Mode à Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0be91-134">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="0be91-135">Correction d’un bug de la cmdlet Get-AzureRmProviderOperation pour les opérations avec Origin comprenant un utilisateur</span><span class="sxs-lookup"><span data-stu-id="0be91-135">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="0be91-136">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-136">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-137">Correction d’un problème où certaines cmdlets ne reconnaissaient pas l’abonnement Azure actuel</span><span class="sxs-lookup"><span data-stu-id="0be91-137">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="0be91-138">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-138">AzureRM.Storage</span></span>
* <span data-ttu-id="0be91-139">Prise en charge de l’obtention de l’utilisation d’une ressource de stockage d’un emplacement spécifique, et de l’ajout de message d'avertissement où l’obtention de l’utilisation d’une ressource de stockage globale est obsolète.</span><span class="sxs-lookup"><span data-stu-id="0be91-139">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="0be91-140">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="0be91-140">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="0be91-141">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="0be91-141">AzureRM.Websites</span></span>
* <span data-ttu-id="0be91-142">Nouvelle cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl : obtient l’URL du webhook de déploiement continu de conteneur</span><span class="sxs-lookup"><span data-stu-id="0be91-142">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="0be91-143">Nouvelles cmdlets New-AzureRMWebAppContainerPSSession et Enter-WebAppContainerPSSession - démarrent une session PowerShell à distance dans une application de conteneur Windows</span><span class="sxs-lookup"><span data-stu-id="0be91-143">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="0be91-144">6.9.0 - septembre 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-144">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="0be91-145">Généralités</span><span class="sxs-lookup"><span data-stu-id="0be91-145">General</span></span>
* <span data-ttu-id="0be91-146">AzureRM.SignalR a été ajouté au module Rollup AzureRM</span><span class="sxs-lookup"><span data-stu-id="0be91-146">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="0be91-147">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-147">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-148">Modifications mineures du code commun de stockage</span><span class="sxs-lookup"><span data-stu-id="0be91-148">Minor changes to the storage common code</span></span>
* <span data-ttu-id="0be91-149">Mise à jour des fichiers d’aide pour inclure des types de paramètre complet.</span><span class="sxs-lookup"><span data-stu-id="0be91-149">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="0be91-150">Modification de -ServicePrincipal en non obligatoire dans l’ensemble de paramètres ServicePrincipalCertificateWithSubscriptionId</span><span class="sxs-lookup"><span data-stu-id="0be91-150">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="0be91-151">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-151">Azure.Storage</span></span>
* <span data-ttu-id="0be91-152">Prise en charge du contexte de stockage avec OAuth.</span><span class="sxs-lookup"><span data-stu-id="0be91-152">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="0be91-153">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="0be91-153">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="0be91-154">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="0be91-154">AzureRM.Cdn</span></span>
* <span data-ttu-id="0be91-155">Ajout de Standard_Microsoft dans la référence SKU de tarification d’un CDN.</span><span class="sxs-lookup"><span data-stu-id="0be91-155">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-156">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-156">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-157">Déplacement des dépendances du coffre de clés et du stockage vers les dépendances communes</span><span class="sxs-lookup"><span data-stu-id="0be91-157">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="0be91-158">Ajout de la prise en charge de plus de tailles de machine virtuelle aux cmdlets AEM</span><span class="sxs-lookup"><span data-stu-id="0be91-158">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="0be91-159">Ajout du paramètre PublicIPPrefix à New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-159">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="0be91-160">Ajout du paramètre ResourceId à la cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="0be91-160">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="0be91-161">Ajout de la cmdlet Invoke-AzureRmVmssVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="0be91-161">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="0be91-162">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="0be91-162">AzureRM.Dns</span></span>
* <span data-ttu-id="0be91-163">Prise en charge de l’enregistrement d’alias pendant la création d’enregistrements DNS</span><span class="sxs-lookup"><span data-stu-id="0be91-163">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="0be91-164">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="0be91-164">AzureRM.Insights</span></span>
* <span data-ttu-id="0be91-165">Résolution des problèmes #6833 et #7102 (zone Paramètres de diagnostic)</span><span class="sxs-lookup"><span data-stu-id="0be91-165">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="0be91-166">Problèmes avec un nom par défaut, par exemple « service », lors de la création et l’obtention/le référencement des paramètres de diagnostic</span><span class="sxs-lookup"><span data-stu-id="0be91-166">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="0be91-167">Problèmes créant des paramètres de diagnostic avec des catégories</span><span class="sxs-lookup"><span data-stu-id="0be91-167">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="0be91-168">Ajout de message de désapprobation pour les paramètres de fragments de temps de métriques</span><span class="sxs-lookup"><span data-stu-id="0be91-168">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="0be91-169">Les paramètres Timegrains sont toujours acceptés (il s’agit d’une modification sans rupture,), mais ils sont ignorés dans le serveur principal dans la mesure où seul PT1M est valide</span><span class="sxs-lookup"><span data-stu-id="0be91-169">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-170">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-170">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-171">Modifications apportées aux cmdlets LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="0be91-171">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="0be91-172">LoadBalancerInboundNatPoolConfig : ajout des paramètres IdleTimeoutInMinutes, EnableFloatingIp et EnableTcpReset</span><span class="sxs-lookup"><span data-stu-id="0be91-172">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="0be91-173">LoadBalancerInboundNatRuleConfig : ajout du paramètre EnableTcpReset</span><span class="sxs-lookup"><span data-stu-id="0be91-173">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="0be91-174">LoadBalancerRuleConfig : ajout du paramètre EnableTcpReset</span><span class="sxs-lookup"><span data-stu-id="0be91-174">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="0be91-175">LoadBalancerProbeConfig : ajout d’une prise en charge de la valeur « Https » pour le paramètre Protocole</span><span class="sxs-lookup"><span data-stu-id="0be91-175">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="0be91-176">Ajout de nouvelles commandes pour la sous-ressource OutboundRule du nouveau LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="0be91-176">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="0be91-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="0be91-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="0be91-179">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-179">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="0be91-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="0be91-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="0be91-182">Ajout d’une nouvelle propriété HostedWorkloads pour PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="0be91-182">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="0be91-183">Ajouté de nouvelles cmdlets pour la fonctionnalité : Pare-feu Azure via ARM</span><span class="sxs-lookup"><span data-stu-id="0be91-183">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="0be91-184">Ajout de Get-AzureRmFirewall</span><span class="sxs-lookup"><span data-stu-id="0be91-184">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="0be91-185">Ajout de Set-AzureRmFirewall</span><span class="sxs-lookup"><span data-stu-id="0be91-185">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="0be91-186">Ajout de New-AzureRmFirewall</span><span class="sxs-lookup"><span data-stu-id="0be91-186">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="0be91-187">Ajout de Remove-AzureRmFirewall</span><span class="sxs-lookup"><span data-stu-id="0be91-187">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="0be91-188">Ajout de New-AzureRmFirewallApplicationRuleCollection</span><span class="sxs-lookup"><span data-stu-id="0be91-188">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="0be91-189">Ajout de New-AzureRmFirewallApplicationRule</span><span class="sxs-lookup"><span data-stu-id="0be91-189">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="0be91-190">Ajout de New-AzureRmFirewallNatRuleCollection</span><span class="sxs-lookup"><span data-stu-id="0be91-190">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="0be91-191">Ajout de New-AzureRmFirewallNatRule</span><span class="sxs-lookup"><span data-stu-id="0be91-191">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="0be91-192">Ajout de New-AzureRmFirewallNetworkRuleCollection</span><span class="sxs-lookup"><span data-stu-id="0be91-192">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="0be91-193">Ajout de New-AzureRmFirewallNetworkRule</span><span class="sxs-lookup"><span data-stu-id="0be91-193">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="0be91-194">Ajout de la prise en charge du certificat racine approuvé et de la configuration de mise à l’échelle automatique dans Application Gateway</span><span class="sxs-lookup"><span data-stu-id="0be91-194">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="0be91-195">Nouvelles cmdlets ajoutées :</span><span class="sxs-lookup"><span data-stu-id="0be91-195">New Cmdlets added:</span></span>
      - <span data-ttu-id="0be91-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="0be91-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="0be91-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="0be91-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="0be91-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="0be91-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="0be91-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="0be91-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="0be91-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="0be91-205">Cmdlets mises à jour avec le paramètre facultatif -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-205">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="0be91-206">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="0be91-206">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="0be91-207">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="0be91-207">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="0be91-208">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="0be91-208">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="0be91-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="0be91-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="0be91-210">Cmdlets mises à jour avec le paramètre facultatif -AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-210">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="0be91-211">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="0be91-211">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="0be91-212">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="0be91-212">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="0be91-213">Ajout d’une cmdlet pour le point de terminaison d’interface Get-AzureInterfaceEndpoint</span><span class="sxs-lookup"><span data-stu-id="0be91-213">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="0be91-214">Ajout de la prise en charge de plusieurs préfixes d’adresse dans un sous-réseau.</span><span class="sxs-lookup"><span data-stu-id="0be91-214">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="0be91-215">Cmdlets mises à jour :</span><span class="sxs-lookup"><span data-stu-id="0be91-215">Updated cmdlets:</span></span>
  - <span data-ttu-id="0be91-216">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-216">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="0be91-217">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-217">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="0be91-218">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-218">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="0be91-219">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-219">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="0be91-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="0be91-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="0be91-222">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-222">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="0be91-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="0be91-224">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-224">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="0be91-225">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-225">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="0be91-226">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-226">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="0be91-227">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-227">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="0be91-228">New-AzureRmNetworkInterfaceIpConfig - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="0be91-229">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-229">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="0be91-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="0be91-231">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-231">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="0be91-232">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-232">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="0be91-233">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-233">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="0be91-234">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="0be91-234">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="0be91-235">Ajout de cmdlets pour la délégation de sous-réseau.</span><span class="sxs-lookup"><span data-stu-id="0be91-235">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="0be91-236">New-AzureRmDelegation : crée une nouvelle délégation, celle-ci peut être ajoutée à un sous-réseau</span><span class="sxs-lookup"><span data-stu-id="0be91-236">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="0be91-237">Remove-AzureRmDelegation : accepte un sous-réseau et supprime le nom de délégation fourni de ce sous-réseau</span><span class="sxs-lookup"><span data-stu-id="0be91-237">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="0be91-238">Add-AzureRmDelegation : accepte un sous-réseau et ajoute le nom de service fourni en tant que délégation à ce sous-réseau</span><span class="sxs-lookup"><span data-stu-id="0be91-238">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="0be91-239">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="0be91-239">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="0be91-240">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="0be91-240">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="0be91-241">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="0be91-241">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="0be91-242">Prise en charge de la gestion de disque managé</span><span class="sxs-lookup"><span data-stu-id="0be91-242">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="0be91-243">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="0be91-243">AzureRM.RedisCache</span></span>
* <span data-ttu-id="0be91-244">Mise à jour de la dépendance Insights.</span><span class="sxs-lookup"><span data-stu-id="0be91-244">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-245">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-246">Mise à jour de New-AzureRmResourceGroupDeployment avec le nouveau paramètre RollbackAction</span><span class="sxs-lookup"><span data-stu-id="0be91-246">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="0be91-247">Ajout de la prise en charge d’OnErrorDeployment avec le nouveau paramètre.</span><span class="sxs-lookup"><span data-stu-id="0be91-247">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="0be91-248">Prise en charge des identités managées sur les affectations de stratégies.</span><span class="sxs-lookup"><span data-stu-id="0be91-248">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="0be91-249">Des paramètres avec des valeurs par défaut ne sont plus requis lors de l’affectation d’une stratégie avec « New-AzureRmPolicyAssignment »</span><span class="sxs-lookup"><span data-stu-id="0be91-249">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="0be91-250">Ajout de la nouvelle cmdlet Get-AzureRmPolicyAlias pour récupérer les alias de stratégie</span><span class="sxs-lookup"><span data-stu-id="0be91-250">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="0be91-251">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0be91-251">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="0be91-252">Résolution du problème #7161</span><span class="sxs-lookup"><span data-stu-id="0be91-252">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="0be91-253">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="0be91-253">AzureRM.SignalR</span></span>
* <span data-ttu-id="0be91-254">Mise à jour des noms de référence SKU en Free_F1 et Standard_S1</span><span class="sxs-lookup"><span data-stu-id="0be91-254">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="0be91-255">Ajout d’un champ de version à l’objet PSSignalRResource et d’une chaîne de connexion à l’objet PSSignalRKeys.</span><span class="sxs-lookup"><span data-stu-id="0be91-255">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="0be91-256">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-256">AzureRM.Storage</span></span>
* <span data-ttu-id="0be91-257">Prise en charge de la stratégie d’immuabilité dans AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-257">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="0be91-258">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="0be91-258">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="0be91-259">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="0be91-259">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="0be91-260">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="0be91-260">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="0be91-261">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="0be91-261">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="0be91-262">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="0be91-262">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="0be91-263">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="0be91-263">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="0be91-264">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="0be91-264">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="0be91-265">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="0be91-265">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="0be91-266">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="0be91-266">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="0be91-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="0be91-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="0be91-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="0be91-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="0be91-269">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="0be91-269">AzureRM.Websites</span></span>
* <span data-ttu-id="0be91-270">Ajout de deux nouvelles cmdlets : Get-AzureRmDeletedWebApp et Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="0be91-270">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="0be91-271">New-AzureRmAppServicePlan : le commutateur HyperV est ajouté pour créer un plan App Service avec conteneur Windows</span><span class="sxs-lookup"><span data-stu-id="0be91-271">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="0be91-272">New-AzureRmWebApp/New-AzureRmWebAppSlot/Set-AzureRmWebApp/Set-AzureRmWebAppSlot : les nouveaux paramètres (la chaîne -ContainerRegistryUser -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) ajoutés pour créer et gérer l’application de conteneur Windows</span><span class="sxs-lookup"><span data-stu-id="0be91-272">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="0be91-273">6.8.1 - Août 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-273">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="0be91-274">Généralités</span><span class="sxs-lookup"><span data-stu-id="0be91-274">General</span></span>
* <span data-ttu-id="0be91-275">Résolution du problème relatif aux groupes de ressources par défaut non définis.</span><span class="sxs-lookup"><span data-stu-id="0be91-275">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="0be91-276">Mise à jour des assemblys de runtime courants</span><span class="sxs-lookup"><span data-stu-id="0be91-276">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="0be91-277">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0be91-277">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="0be91-278">Résolution du problème relatif aux groupes de ressources par défaut non définis.</span><span class="sxs-lookup"><span data-stu-id="0be91-278">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="0be91-279">Problème résolu https://github.com/Azure/azure-powershell/issues/6603</span><span class="sxs-lookup"><span data-stu-id="0be91-279">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="0be91-280">Les cmdlets Import-AzureRmApiManagementApi et \*-AzureRmApiManagementCertificate peuvent maintenant gérer les chemins d’accès relatifs</span><span class="sxs-lookup"><span data-stu-id="0be91-280">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="0be91-281">Problème résolu https://github.com/Azure/azure-powershell/issues/6879</span><span class="sxs-lookup"><span data-stu-id="0be91-281">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="0be91-282">CertificateInformation est une propriété définissable permettant à la cmdlet Set-AzureRmApiManagement de fonctionner correctement.</span><span class="sxs-lookup"><span data-stu-id="0be91-282">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="0be91-283">Résolu en passant au nuget 4.0.4-preview</span><span class="sxs-lookup"><span data-stu-id="0be91-283">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="0be91-284">Problème résolu https://github.com/Azure/azure-powershell/issues/6853</span><span class="sxs-lookup"><span data-stu-id="0be91-284">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="0be91-285">Recherche par nom sur produit du filtre Odata résolue</span><span class="sxs-lookup"><span data-stu-id="0be91-285">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="0be91-286">Problème résolu https://github.com/Azure/azure-powershell/issues/6814</span><span class="sxs-lookup"><span data-stu-id="0be91-286">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="0be91-287">Recherche par nom sur Api du filtre Odata résolue</span><span class="sxs-lookup"><span data-stu-id="0be91-287">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="0be91-288">Ajout de la prise en charge de l’enregistreur d'événements AzureMonitor</span><span class="sxs-lookup"><span data-stu-id="0be91-288">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="0be91-289">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-289">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-290">Résolution du problème signalant que la cible est manquante dans la sortie d’erreur.</span><span class="sxs-lookup"><span data-stu-id="0be91-290">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="0be91-291">Résolution du problème relatif au type de compte de stockage pour les machines virtuelles dotées d’un disque managé</span><span class="sxs-lookup"><span data-stu-id="0be91-291">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="0be91-292">Résolution du problème relatif aux groupes de ressources par défaut non définis.</span><span class="sxs-lookup"><span data-stu-id="0be91-292">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="0be91-293">Correction des applets de commande AEM Extension pour d’autres environnements, par exemple Azure Chine</span><span class="sxs-lookup"><span data-stu-id="0be91-293">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-294">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-295">Modification de la présentation d’une sortie de cmdlet par défaut en affichage sous forme de table</span><span class="sxs-lookup"><span data-stu-id="0be91-295">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="0be91-296">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="0be91-296">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="0be91-297">Correction de l’erreur dans Update-AzureRmPowerBIEmbeddedCapacity lors d’une tentative de redimensionnement de la capacité mise en pause</span><span class="sxs-lookup"><span data-stu-id="0be91-297">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="0be91-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-298">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-299">Résolution du problème de création d’applications managées depuis le Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0be91-299">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="0be91-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0be91-300">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="0be91-301">Problèmes résolus</span><span class="sxs-lookup"><span data-stu-id="0be91-301">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="0be91-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="0be91-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="0be91-303">Ajout de la prise en charge de la méthode de routage MultiValue</span><span class="sxs-lookup"><span data-stu-id="0be91-303">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="0be91-304">Nouveau paramètre « MaxReturn » pour le routage MultiValue</span><span class="sxs-lookup"><span data-stu-id="0be91-304">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="0be91-305">Ajout de la prise en charge de la méthode de routage Subnet</span><span class="sxs-lookup"><span data-stu-id="0be91-305">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="0be91-306">Prise en charge des plages d’adresses IP (sous-réseaux) dans les points de terminaison</span><span class="sxs-lookup"><span data-stu-id="0be91-306">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="0be91-307">Ajout de la prise en charge des en-têtes personnalisés dans les profils</span><span class="sxs-lookup"><span data-stu-id="0be91-307">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="0be91-308">Ajout de la prise en charge des plages de codes avec l’état Attendu dans les profils</span><span class="sxs-lookup"><span data-stu-id="0be91-308">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="0be91-309">Ajout de la prise en charge des en-têtes personnalisés dans les points de terminaison</span><span class="sxs-lookup"><span data-stu-id="0be91-309">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="0be91-310">6.8.0 - Août 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-310">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="0be91-311">Généralités</span><span class="sxs-lookup"><span data-stu-id="0be91-311">General</span></span>
* <span data-ttu-id="0be91-312">Résolution du problème relatif aux groupes de ressources par défaut non définis.</span><span class="sxs-lookup"><span data-stu-id="0be91-312">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="0be91-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-313">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-314">Ajout d’une propriété d’expiration aux jetons renvoyés lors de la phase Connect-AzureRmAccount.</span><span class="sxs-lookup"><span data-stu-id="0be91-314">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-315">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-315">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-316">Résolution du problème signalant que la cible est manquante dans la sortie d’erreur.</span><span class="sxs-lookup"><span data-stu-id="0be91-316">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="0be91-317">Résolution du problème relatif au type de compte de stockage pour les machines virtuelles dotées d’un disque managé</span><span class="sxs-lookup"><span data-stu-id="0be91-317">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="0be91-318">Correction des applets de commande AEM Extension pour d’autres environnements, par exemple Azure Chine</span><span class="sxs-lookup"><span data-stu-id="0be91-318">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="0be91-319">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="0be91-319">AzureRM.IotHub</span></span>
* <span data-ttu-id="0be91-320">Correction des exemples pour New-AzureRmIotHubExportDevices et New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="0be91-320">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-321">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-321">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-322">Modification de la représentation sous forme de modèles par défaut en affichage sous forme de table</span><span class="sxs-lookup"><span data-stu-id="0be91-322">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="0be91-323">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="0be91-323">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="0be91-324">Correction de l’erreur dans Update-AzureRmPowerBIEmbeddedCapacity lors d’une tentative de redimensionnement de la capacité mise en pause</span><span class="sxs-lookup"><span data-stu-id="0be91-324">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-325">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-325">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-326">Résolution du problème de création d’application managée depuis le Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0be91-326">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="0be91-327">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0be91-327">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="0be91-328">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="0be91-328">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="0be91-329">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="0be91-329">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="0be91-330">Prise en charge de la méthode de routage MultiValue</span><span class="sxs-lookup"><span data-stu-id="0be91-330">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="0be91-331">Nouveau paramètre « MaxReturn » pour le routage MultiValue</span><span class="sxs-lookup"><span data-stu-id="0be91-331">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="0be91-332">Prise en charge de la méthode de routage Subnet</span><span class="sxs-lookup"><span data-stu-id="0be91-332">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="0be91-333">Prise en charge des plages d’adresses IP (sous-réseaux) dans les points de terminaison</span><span class="sxs-lookup"><span data-stu-id="0be91-333">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="0be91-334">Prise en charge des en-têtes personnalisés dans les profils</span><span class="sxs-lookup"><span data-stu-id="0be91-334">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="0be91-335">Prise en charge des plages de codes avec l’état Attendu dans les profils</span><span class="sxs-lookup"><span data-stu-id="0be91-335">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="0be91-336">Prise en charge des en-têtes personnalisés dans les points de terminaison</span><span class="sxs-lookup"><span data-stu-id="0be91-336">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="0be91-337">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="0be91-337">AzureRM.Websites</span></span>
* <span data-ttu-id="0be91-338">Résolution du problème relatif aux groupes de ressources par défaut mal définis.</span><span class="sxs-lookup"><span data-stu-id="0be91-338">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="0be91-339">6.7.0 : août 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-339">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="0be91-340">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-340">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-341">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-341">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="0be91-342">Ajout d’un identifiant utilisateur au nom de contexte par défaut afin d’éviter un conflit de contextes.</span><span class="sxs-lookup"><span data-stu-id="0be91-342">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="0be91-343">Résolution des problèmes liés à Clear-AzureRmContext avec la sélection d’un contexte 6398.</span><span class="sxs-lookup"><span data-stu-id="0be91-343">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="0be91-344">Possibilité de transmettre le domaine du locataire au paramètre « -TenantId » pour la cmdlet Connect-AzureRmAccount.</span><span class="sxs-lookup"><span data-stu-id="0be91-344">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="0be91-345">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-345">Azure.Storage</span></span>
* <span data-ttu-id="0be91-346">Suppression de la limite de 5 To pour le quota de partage de fichiers Azure.</span><span class="sxs-lookup"><span data-stu-id="0be91-346">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="0be91-347">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="0be91-347">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="0be91-348">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0be91-348">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="0be91-349">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-349">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="0be91-350">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0be91-350">Azure.AnalysisServices</span></span>
* <span data-ttu-id="0be91-351">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-351">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="0be91-352">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0be91-352">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="0be91-353">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="0be91-354">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="0be91-354">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="0be91-355">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="0be91-356">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="0be91-356">AzureRM.Automation</span></span>
* <span data-ttu-id="0be91-357">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="0be91-358">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="0be91-358">AzureRM.Backup</span></span>
* <span data-ttu-id="0be91-359">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="0be91-360">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="0be91-360">AzureRM.Batch</span></span>
* <span data-ttu-id="0be91-361">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="0be91-362">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="0be91-362">AzureRM.Billing</span></span>
* <span data-ttu-id="0be91-363">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="0be91-364">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="0be91-364">AzureRM.Cdn</span></span>
* <span data-ttu-id="0be91-365">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="0be91-366">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0be91-366">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="0be91-367">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-368">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-368">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-369">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-369">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="0be91-370">Ajout du paramètre EvictionPolicy à la cmdlet New-AzureRmVmssConfig.</span><span class="sxs-lookup"><span data-stu-id="0be91-370">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="0be91-371">Utilisation de l’emplacement par défaut dans le paramètre DiskFileParameterSet de la cmdlet New-AzureRmVm si aucun emplacement n’est spécifié.</span><span class="sxs-lookup"><span data-stu-id="0be91-371">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="0be91-372">Correction de la description de paramètre dans la cmdlet Save-AzureRmVMImage.</span><span class="sxs-lookup"><span data-stu-id="0be91-372">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="0be91-373">Correction de la cmdlet Get-AzureRmVMDiskEncryptionStatus pour certains scénarios liés à un passage unique.</span><span class="sxs-lookup"><span data-stu-id="0be91-373">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="0be91-374">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="0be91-374">AzureRM.Consumption</span></span>
* <span data-ttu-id="0be91-375">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="0be91-376">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="0be91-376">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="0be91-377">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="0be91-378">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="0be91-378">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="0be91-379">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-379">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="0be91-380">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="0be91-380">AzureRM.DataFactories</span></span>
* <span data-ttu-id="0be91-381">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-381">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="0be91-382">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="0be91-382">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="0be91-383">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-383">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="0be91-384">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="0be91-384">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="0be91-385">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-385">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="0be91-386">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0be91-386">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="0be91-387">Correction du débogage lorsque le paramètre DebugPreference est défini à partir de la ligne de commande PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0be91-387">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="0be91-388">Mise à jour de l’exemple pour la cmdlet Set-AzureRmDataLakeStoreItemAcl.</span><span class="sxs-lookup"><span data-stu-id="0be91-388">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="0be91-389">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-389">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="0be91-390">Mise à jour de l’exemple pour la cmdlet Set-AzureRmDataLakeStoreItemAclEntry.</span><span class="sxs-lookup"><span data-stu-id="0be91-390">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="0be91-391">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="0be91-391">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="0be91-392">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="0be91-393">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="0be91-393">AzureRM.Dns</span></span>
* <span data-ttu-id="0be91-394">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="0be91-395">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="0be91-395">AzureRM.EventGrid</span></span>
* <span data-ttu-id="0be91-396">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="0be91-397">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="0be91-397">AzureRM.EventHub</span></span>
* <span data-ttu-id="0be91-398">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="0be91-399">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0be91-399">AzureRM.HDInsight</span></span>
* <span data-ttu-id="0be91-400">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="0be91-401">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="0be91-401">AzureRM.Insights</span></span>
* <span data-ttu-id="0be91-402">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="0be91-403">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="0be91-403">AzureRM.IotHub</span></span>
* <span data-ttu-id="0be91-404">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="0be91-405">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0be91-405">AzureRM.KeyVault</span></span>
* <span data-ttu-id="0be91-406">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="0be91-407">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="0be91-407">AzureRM.LogicApp</span></span>
* <span data-ttu-id="0be91-408">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="0be91-409">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="0be91-409">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="0be91-410">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="0be91-411">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="0be91-411">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="0be91-412">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-412">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="0be91-413">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="0be91-413">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="0be91-414">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-414">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="0be91-415">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="0be91-415">AzureRM.Media</span></span>
* <span data-ttu-id="0be91-416">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-416">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-417">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-417">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-418">Ajout d’un exemple pour la cmdlet Set-AzureRmLocalNetworkGateway.</span><span class="sxs-lookup"><span data-stu-id="0be91-418">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="0be91-419">Ajout d’exemples et de descriptions pour les cmdlets Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey et New-AzureRmVirtualNetworkGatewayConnection.</span><span class="sxs-lookup"><span data-stu-id="0be91-419">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="0be91-420">Ajout d’exemples pour les cmdlets Remove-AzureRmVirtualNetworkGatewayIpConfig et Reset-AzureRmVirtualNetworkGateway.</span><span class="sxs-lookup"><span data-stu-id="0be91-420">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="0be91-421">Ajout d’un exemple pour la cmdlet Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey.</span><span class="sxs-lookup"><span data-stu-id="0be91-421">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="0be91-422">Ajout d’un exemple pour la cmdlet Set-AzureRmVirtualNetworkGatewayConnectionSharedKey.</span><span class="sxs-lookup"><span data-stu-id="0be91-422">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="0be91-423">Ajout d’un exemple pour la cmdlet Set-AzureRmVirtualNetworkGatewayConnection.</span><span class="sxs-lookup"><span data-stu-id="0be91-423">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="0be91-424">Régénération des cmdlets pour ApplicationSecurityGroup, RouteTable et Usage à l’aide du tout dernier générateur de code.</span><span class="sxs-lookup"><span data-stu-id="0be91-424">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="0be91-425">Clarification du message d’erreur pour la cmdlet Get-AzureRmVirtualNetworkSubnetConfig lors de la tentative d’obtention d’un sous-réseau qui n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="0be91-425">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="0be91-426">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="0be91-426">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="0be91-427">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="0be91-428">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0be91-428">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="0be91-429">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="0be91-430">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0be91-430">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="0be91-431">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="0be91-432">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="0be91-432">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="0be91-433">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="0be91-434">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0be91-434">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="0be91-435">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="0be91-436">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="0be91-436">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="0be91-437">Ajout d’un filtre de stratégie pour la cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="0be91-437">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="0be91-438">La commande retourne la liste des éléments de sauvegarde protégés par l’ID de stratégie donnée.</span><span class="sxs-lookup"><span data-stu-id="0be91-438">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="0be91-439">Mise à jour de Microsoft.Azure.Management.RecoveryServices.Backup vers la préversion 3.0.0.</span><span class="sxs-lookup"><span data-stu-id="0be91-439">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="0be91-440">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-440">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="0be91-441">Ajout du paramètre TargetResourceGroupName à la cmdlet Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="0be91-441">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="0be91-442">Groupe de ressources vers lequel les disques managés sont restaurés.</span><span class="sxs-lookup"><span data-stu-id="0be91-442">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="0be91-443">S’applique à la sauvegarde des machines virtuelles avec disques managés.</span><span class="sxs-lookup"><span data-stu-id="0be91-443">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="0be91-444">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="0be91-444">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="0be91-445">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-445">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="0be91-446">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="0be91-446">AzureRM.RedisCache</span></span>
* <span data-ttu-id="0be91-447">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-447">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="0be91-448">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="0be91-448">AzureRM.Relay</span></span>
* <span data-ttu-id="0be91-449">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-449">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-450">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-450">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-451">Prise en charge du déploiement de modèle à l’étendue de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="0be91-451">Support template deployment at subscription scope.</span></span> <span data-ttu-id="0be91-452">Ajout de nouvelles cmdlets :</span><span class="sxs-lookup"><span data-stu-id="0be91-452">Add new Cmdlets:</span></span>
    - <span data-ttu-id="0be91-453">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="0be91-453">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="0be91-454">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="0be91-454">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="0be91-455">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="0be91-455">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="0be91-456">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="0be91-456">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="0be91-457">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="0be91-457">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="0be91-458">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="0be91-458">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="0be91-459">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="0be91-459">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="0be91-460">Résolution du problème entraînant une erreur lors de la transmission d’un contexte à la cmdlet Set-AzureRmResource.</span><span class="sxs-lookup"><span data-stu-id="0be91-460">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="0be91-461">Correction de l’exemple indiqué pour la cmdlet New-AzureRmResourceGroupDeployment.</span><span class="sxs-lookup"><span data-stu-id="0be91-461">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="0be91-462">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-462">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="0be91-463">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="0be91-463">AzureRM.Scheduler</span></span>
* <span data-ttu-id="0be91-464">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-464">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="0be91-465">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0be91-465">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="0be91-466">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="0be91-467">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0be91-467">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="0be91-468">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="0be91-469">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-469">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-470">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="0be91-471">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-471">AzureRM.Storage</span></span>
* <span data-ttu-id="0be91-472">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-472">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="0be91-473">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="0be91-473">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="0be91-474">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-474">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="0be91-475">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="0be91-475">AzureRM.Tags</span></span>
* <span data-ttu-id="0be91-476">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-476">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="0be91-477">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="0be91-477">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="0be91-478">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-478">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="0be91-479">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="0be91-479">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="0be91-480">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-480">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="0be91-481">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="0be91-481">AzureRM.Websites</span></span>
* <span data-ttu-id="0be91-482">Mise à jour vers la dernière version d’Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-482">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="0be91-483">6.6.0 - juillet 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-483">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="0be91-484">Généralités</span><span class="sxs-lookup"><span data-stu-id="0be91-484">General</span></span>
* <span data-ttu-id="0be91-485">Mise à jour de tous les fichiers d’aide pour inclure les types de paramètre complet et les types d’entrée/sortie corrects.</span><span class="sxs-lookup"><span data-stu-id="0be91-485">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="0be91-486">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-486">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-487">Mise à jour de la bibliothèque Common.Strategy pour être en mesure de valider que la configuration actuelle pour une ressource est compatible avec la ressource cible.</span><span class="sxs-lookup"><span data-stu-id="0be91-487">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="0be91-488">Ajout des types ps1xml à Common.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-488">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="0be91-489">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-489">Azure.Storage</span></span>
* <span data-ttu-id="0be91-490">Ajout de la prise en charge de l’obtention du contexte de stockage à partir de DefaultProfile.</span><span class="sxs-lookup"><span data-stu-id="0be91-490">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="0be91-491">Ajout de Ps1XmlAttribute aux propriétés de types de sortie des cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0be91-491">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="0be91-492">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0be91-492">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="0be91-493">Problème résolu https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="0be91-493">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="0be91-494">Correction du bogue dans Automapper pour traduire PsApiManagementApi à ApiContract</span><span class="sxs-lookup"><span data-stu-id="0be91-494">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="0be91-495">Problème résolu https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="0be91-495">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="0be91-496">Correction du bogue dans File.Save pour ne pas surcharger avec le Type d’encodage</span><span class="sxs-lookup"><span data-stu-id="0be91-496">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="0be91-497">Problème résolu https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="0be91-497">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="0be91-498">Mise à jour vers la version 4.0.3 de Nuget qui corrige l’exception du modèle sur apiId</span><span class="sxs-lookup"><span data-stu-id="0be91-498">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-499">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-499">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-500">Correction du problème d’échec de création d’une machine virtuelle à l’aide de DiskFileParameterSet dans New-AzureRmVm en raison du changement de nom du type de compte de stockage PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="0be91-500">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="0be91-501">Correction de la cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="0be91-501">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="0be91-502">Mise à jour de Get-AzureRmAvailabilitySet pour activer la liste de tous les groupes à haute disponibilité dans un abonnement.</span><span class="sxs-lookup"><span data-stu-id="0be91-502">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="0be91-503">(La paramètre ResouceGroupName est désormais facultatif.)</span><span class="sxs-lookup"><span data-stu-id="0be91-503">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="0be91-504">Mise à jour de SimpleParameterSet pour « New-AzureRmVm » pour activer le réseau accéléré sur les machines virtuelles admissibles.</span><span class="sxs-lookup"><span data-stu-id="0be91-504">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="0be91-505">Mise à jour du jeu de paramètres simple de New-AzureRmVmss qui échoue à créer les groupes de machines virtuelles identiques lorsqu’un équilibreur de charge spécifié par un utilisateur existe déjà.</span><span class="sxs-lookup"><span data-stu-id="0be91-505">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="0be91-506">Mise à jour de l’exemple pour New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="0be91-506">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="0be91-507">Ajout d’un exemple pour « New-AzureRmVM »</span><span class="sxs-lookup"><span data-stu-id="0be91-507">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="0be91-508">Mise à jour de la description pour Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="0be91-508">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="0be91-509">Mise à jour de l’exemple 1 pour Set-AzureRmVMBginfoExtension pour corriger l’orthographe et le préfixe.</span><span class="sxs-lookup"><span data-stu-id="0be91-509">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="0be91-510">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="0be91-510">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="0be91-511">Mise à jour de la version du Kit de développement logiciel (SDK) ADF .Net vers la version 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="0be91-511">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="0be91-512">Prise en charge du runtime d’intégration auto-hébergé en partageant entre les fabriques de données.</span><span class="sxs-lookup"><span data-stu-id="0be91-512">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="0be91-513">Ajout d’un nouveau paramètre -SharedIntegrationRuntimeResourceId à la cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-513">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="0be91-514">Ajout d’un nouveau paramètre facultatif -LinkedDataFactoryName à la cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="0be91-514">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="0be91-515">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0be91-515">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="0be91-516">Mise à jour de la version du Kit de développement logiciel (SDK) DataPlane (Microsoft.Azure.DataLake.Store) vers la version 1.1.9</span><span class="sxs-lookup"><span data-stu-id="0be91-516">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="0be91-517">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="0be91-517">AzureRM.EventHub</span></span>
* <span data-ttu-id="0be91-518">Mise à jour de la redirection pour InputObject et ResourceId dans les cmdlets de suppression</span><span class="sxs-lookup"><span data-stu-id="0be91-518">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="0be91-519">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="0be91-519">AzureRM.Insights</span></span>
* <span data-ttu-id="0be91-520">Correction de mise en forme de OutputType dans les fichiers d’aide</span><span class="sxs-lookup"><span data-stu-id="0be91-520">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="0be91-521">À l’aide de la préversion 0.19.1 du Kit de développement logiciel Microsoft.Azure.Management.Monitor</span><span class="sxs-lookup"><span data-stu-id="0be91-521">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="0be91-522">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0be91-522">AzureRM.KeyVault</span></span>
* <span data-ttu-id="0be91-523">Correction des problèmes de redirection dans Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0be91-523">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-524">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-524">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-525">Ajout d’exemples pour les cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="0be91-525">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-526">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-526">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-527">Correction du problème lorsque vous fournissez le nom de la balise et la valeur pour « Get-AzureRmResource »</span><span class="sxs-lookup"><span data-stu-id="0be91-527">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="0be91-528">Correction du scénario de redirection avec « Set-AzureRmResource »</span><span class="sxs-lookup"><span data-stu-id="0be91-528">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="0be91-529">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0be91-529">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="0be91-530">Mise à jour de la redirection pour InputObject et ResourceId dans les cmdlets de suppression</span><span class="sxs-lookup"><span data-stu-id="0be91-530">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="0be91-531">quelques problèmes résolus</span><span class="sxs-lookup"><span data-stu-id="0be91-531">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="0be91-532">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-532">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-533">Ajout d’un support de serveur de protection avancée contre les menaces avec les cmdlets suivantes :</span><span class="sxs-lookup"><span data-stu-id="0be91-533">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="0be91-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="0be91-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="0be91-535">Ajout d’un support d’évaluation des vulnérabilités avec les cmdlets suivantes :</span><span class="sxs-lookup"><span data-stu-id="0be91-535">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="0be91-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="0be91-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="0be91-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="0be91-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="0be91-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="0be91-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="0be91-539">Correction de l’exemple dans Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="0be91-539">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="0be91-540">Correction de la manipulation incorrecte de la DateHeure pour les cultures non-américaines dans Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="0be91-540">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="0be91-541">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-541">AzureRM.Storage</span></span>
* <span data-ttu-id="0be91-542">Ajout de Ps1XmlAttribute aux propriétés de types de sortie des cmdlets</span><span class="sxs-lookup"><span data-stu-id="0be91-542">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="0be91-543">Affichage de la sortie de la cmdlet StorageAccount dans l’affichage du tableau</span><span class="sxs-lookup"><span data-stu-id="0be91-543">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="0be91-544">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0be91-544">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="0be91-545">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0be91-545">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="0be91-546">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0be91-546">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="0be91-547">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="0be91-547">AzureRM.Tags</span></span>
* <span data-ttu-id="0be91-548">Suppression de l’instruction incorrecte de l’aide de la cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="0be91-548">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="0be91-549">6.5.0 - Juillet 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-549">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="0be91-550">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-550">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-551">Mise à jour de l’aide pour « Get-AzureRmContextAutosaveSetting »</span><span class="sxs-lookup"><span data-stu-id="0be91-551">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="0be91-552">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-552">Azure.Storage</span></span>
* <span data-ttu-id="0be91-553">Prise en charge du chargement de l’objet blob ou du fichier avec un jeton SAS en écriture seule</span><span class="sxs-lookup"><span data-stu-id="0be91-553">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="0be91-554">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="0be91-554">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="0be91-555">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="0be91-555">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="0be91-556">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0be91-556">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="0be91-557">Ajout de la propriété ResourceGroupName requise au système autonome.</span><span class="sxs-lookup"><span data-stu-id="0be91-557">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="0be91-558">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="0be91-558">AzureRM.Automation</span></span>
* <span data-ttu-id="0be91-559">Mise à jour de l’aide et ajout d’un exemple pour « New-AzureRMAutomationSchedule »</span><span class="sxs-lookup"><span data-stu-id="0be91-559">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-560">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-560">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-561">Ajout du paramètre de balise à Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="0be91-561">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="0be91-562">Ajout d’un exemple pour « Add-AzureRmVmssExtension »</span><span class="sxs-lookup"><span data-stu-id="0be91-562">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="0be91-563">Ajout d’exemples pour « Remove-AzureRmVmssExtension »</span><span class="sxs-lookup"><span data-stu-id="0be91-563">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="0be91-564">Mise à jour de l’aide pour « Set-AzureRmVMAccessExtension »</span><span class="sxs-lookup"><span data-stu-id="0be91-564">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="0be91-565">Mettez à jour SimpleParameterSet pour New-AzureRmVmss pour définir SinglePlacementGroup sur false par défaut, et ajoutez le paramètre de commutateur « SinglePlacementGroup » qui permet à l’utilisateur de créer le groupe de machines virtuelles identiques dans un seul groupe de placement.</span><span class="sxs-lookup"><span data-stu-id="0be91-565">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="0be91-566">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="0be91-566">AzureRM.EventHub</span></span>
* <span data-ttu-id="0be91-567">Ajout d’une propriété en lecture seule « PendingReplicationOperationsCount » à la classe PSEventHubDRConfigurationAttributes, ce qui donne le nombre d’opérations de réplication en attente pendant l’exécution de la réplication</span><span class="sxs-lookup"><span data-stu-id="0be91-567">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="0be91-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0be91-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="0be91-569">Mise à jour du message d’erreur pour Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0be91-569">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="0be91-570">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="0be91-570">AzureRM.LogicApp</span></span>
* <span data-ttu-id="0be91-571">Correction de l’erreur « impossible de résoudre le jeu de paramètres » dans New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="0be91-571">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-572">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-572">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-573">Activer l’homologation entre des réseaux virtuels dans plusieurs locataires pour Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="0be91-573">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="0be91-574">Mise à jour des applets de commande ci-dessous pour Application Gateway</span><span class="sxs-lookup"><span data-stu-id="0be91-574">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="0be91-575">New-AzureRmApplicationGateway : ajout de la prise en charge des zones et de l’indicateur EnableFIPS</span><span class="sxs-lookup"><span data-stu-id="0be91-575">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="0be91-576">New-AzureRmApplicationGatewaySku : ajout des nouvelles références (SKU) Standard_v2 et WAF_v2</span><span class="sxs-lookup"><span data-stu-id="0be91-576">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="0be91-577">Set-AzureRmApplicationGatewaySku : ajout des nouvelles références (SKU) Standard_v2 et WAF_v2</span><span class="sxs-lookup"><span data-stu-id="0be91-577">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="0be91-578">Régénération des applets de commande RouteTable avec la dernière version du Générateur</span><span class="sxs-lookup"><span data-stu-id="0be91-578">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="0be91-579">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="0be91-579">AzureRM.Relay</span></span>
* <span data-ttu-id="0be91-580">Mise à jour des fichiers Markdown, correction du problème relatif au nom du paramètre dans l’exemple</span><span class="sxs-lookup"><span data-stu-id="0be91-580">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-581">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-581">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-582">Mise à jour des applets de commande Roleassignment et Roledefinition :</span><span class="sxs-lookup"><span data-stu-id="0be91-582">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="0be91-583">Supprimez les appels Roledefinition supplémentaires dans le cadre de la pagination.</span><span class="sxs-lookup"><span data-stu-id="0be91-583">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="0be91-584">Correction de l’applet de commande Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0be91-584">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="0be91-585">Correction de la fonctionnalité du paramètre de commande -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="0be91-585">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="0be91-586">Résolution du problème avec « Get-AzureRmResource » où le paramètre « -ResourceType » était sensible à la casse</span><span class="sxs-lookup"><span data-stu-id="0be91-586">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="0be91-587">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0be91-587">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="0be91-588">Ajout des paramètres Top et Skip à la liste des applets de commande</span><span class="sxs-lookup"><span data-stu-id="0be91-588">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="0be91-589">Ajout des applets de commande de migration de l’espace de noms Standard vers l’espace de noms Premium :</span><span class="sxs-lookup"><span data-stu-id="0be91-589">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="0be91-590">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="0be91-590">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="0be91-591">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="0be91-591">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="0be91-592">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="0be91-592">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="0be91-593">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="0be91-593">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="0be91-594">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="0be91-594">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="0be91-595">Ajout d’une propriété en lecture seule « PendingReplicationOperationsCount » à la classe PSServiceBusDRConfigurationAttributes, ce qui donne le nombre d’opérations de réplication en attente pendant l’exécution de la réplication</span><span class="sxs-lookup"><span data-stu-id="0be91-595">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="0be91-596">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0be91-596">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="0be91-597">Mise à jour de l’exemple pour « New-AzureRmServiceFabricCluster »</span><span class="sxs-lookup"><span data-stu-id="0be91-597">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="0be91-598">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-598">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-599">Ajout de nouvelles applets de commande pour Management.Sql pour permettre aux clients d’ajouter le certificat TDE à l’instance SQL Server ou à une instance gérée</span><span class="sxs-lookup"><span data-stu-id="0be91-599">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="0be91-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="0be91-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="0be91-602">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="0be91-602">AzureRM.Websites</span></span>
* <span data-ttu-id="0be91-603">Lorsque `Set-AzureRmWebApp -AssignIdentity` et `Set-AzureRmWebAppSlot -AssignIdentity` sont définis sur false, cela supprime également la propriété d’identité de la balise d’aperçu du site object.Removing.</span><span class="sxs-lookup"><span data-stu-id="0be91-603">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="0be91-604">Exemples `Get-AzureRmWebAppMetrics` et `Get-AzureRmAppServicePlanMetrics` mis à jour</span><span class="sxs-lookup"><span data-stu-id="0be91-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="0be91-605">`Set-AzureRmWebApp -PhpVersion` prend en charge hors connexion en tant que version PHP valide</span><span class="sxs-lookup"><span data-stu-id="0be91-605">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="0be91-606">6.4.0 - Juillet 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-606">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="0be91-607">Généralités</span><span class="sxs-lookup"><span data-stu-id="0be91-607">General</span></span>
* <span data-ttu-id="0be91-608">Correction de mise en forme de OutputType dans les fichiers d’aide pour la plupart des modules</span><span class="sxs-lookup"><span data-stu-id="0be91-608">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="0be91-609">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-609">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-610">Ajout de l’attribut Ps1Xml aux types de sortie de base</span><span class="sxs-lookup"><span data-stu-id="0be91-610">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-611">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-611">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-612">Fonctionnalité IP Tag pour VMSS</span><span class="sxs-lookup"><span data-stu-id="0be91-612">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="0be91-613">La cmdlet New-AzureRmVmssIpTagConfig est ajoutée</span><span class="sxs-lookup"><span data-stu-id="0be91-613">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="0be91-614">Ajout du paramètre IpTag à New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-614">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="0be91-615">Fonctionnalité de restauration du système d’exploitation automatique pour VMSS</span><span class="sxs-lookup"><span data-stu-id="0be91-615">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="0be91-616">Les paramètres DisableAutoRollback sont ajoutés à New-AzureRmVmssConfig et Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="0be91-616">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="0be91-617">Fonctionnalité OS Upgrade History pour Vmss</span><span class="sxs-lookup"><span data-stu-id="0be91-617">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="0be91-618">Le paramètre de commutateur OSUpgradeHistory est ajouté à Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="0be91-618">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="0be91-619">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="0be91-619">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="0be91-620">Ajout de la prise en charge des listes de contrôle d’accès de catalogue avec les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="0be91-620">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="0be91-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="0be91-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="0be91-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="0be91-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="0be91-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="0be91-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="0be91-624">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0be91-624">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="0be91-625">Ajout de la prise en charge de l’annulation et du suivi de la progression pour Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="0be91-625">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="0be91-626">Ajout de la prise en charge de l’annulation pour Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="0be91-626">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="0be91-627">Correction du vidage des messages de débogage pour les cmdlets qui effectuent des opérations récursives</span><span class="sxs-lookup"><span data-stu-id="0be91-627">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="0be91-628">Correction de l’emplacement du test des applets de commande DataLake</span><span class="sxs-lookup"><span data-stu-id="0be91-628">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="0be91-629">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="0be91-629">AzureRM.EventHub</span></span>
* <span data-ttu-id="0be91-630">Ajout du paramètre MaxCount facultatif à la cmdlet Répertorier les opérations Get-AzureRmEventHub et Get-AzureRmEventHubConsumerGroup</span><span class="sxs-lookup"><span data-stu-id="0be91-630">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="0be91-631">Résolution du problème dans la cmdlet New-AzureRmEventHub où au moins un paramètre est nécessaire lors de la création du nouveau EventHub.</span><span class="sxs-lookup"><span data-stu-id="0be91-631">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="0be91-632">Jeu de paramètres par défaut fourni.</span><span class="sxs-lookup"><span data-stu-id="0be91-632">Provided Default Parameter set.</span></span>
* <span data-ttu-id="0be91-633">Ajout du Parameter -KeyValue facultatif à la cmdlet New-AzureRmEventHubKey, qui permet à l’utilisateur de fournir KeyValue.</span><span class="sxs-lookup"><span data-stu-id="0be91-633">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="0be91-634">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0be91-634">AzureRM.KeyVault</span></span>
* <span data-ttu-id="0be91-635">Résolution d’un problème où toutes les ressources sont renvoyées par Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="0be91-635">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-636">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-636">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-637">Exposer les nouvelles références SKU pour Zone-Redundant VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="0be91-637">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="0be91-638">Ajout de nouvelles commandes pour la fonctionnalité : API de partenaire ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="0be91-638">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="0be91-639">Ajout de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="0be91-639">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="0be91-640">Ajout de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="0be91-640">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="0be91-641">Ajout de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="0be91-641">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="0be91-642">Ajout de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="0be91-642">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="0be91-643">Ajout de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="0be91-643">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="0be91-644">Ajout de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="0be91-644">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="0be91-645">Ajout de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="0be91-645">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="0be91-646">Ajout de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="0be91-646">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="0be91-647">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="0be91-647">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="0be91-648">Ajout de la cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="0be91-648">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="0be91-649">Cette cmdlet prend un ID de machine virtuelle et vérifie si la machine virtuelle est protégée par un coffre dans l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="0be91-649">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="0be91-650">Si un tel coffre existe, la cmdlet sort les informations du coffre.</span><span class="sxs-lookup"><span data-stu-id="0be91-650">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-651">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-651">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-652">Mettre à jour les cmdlets Get-AzureRmPolicyAssignment :</span><span class="sxs-lookup"><span data-stu-id="0be91-652">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="0be91-653">Ajouter la prise de l’énumération des valeurs -Scope values au niveau du groupe de gestion</span><span class="sxs-lookup"><span data-stu-id="0be91-653">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="0be91-654">Ajouter la prise en charge de la récupération des affectations individuelles avec les valeurs -Scope au niveau du groupe de gestion</span><span class="sxs-lookup"><span data-stu-id="0be91-654">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="0be91-655">Ajouter les commutateurs -Effective et -All au paramètre de contrôle</span><span class="sxs-lookup"><span data-stu-id="0be91-655">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="0be91-656">Mettre à jour les cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0be91-656">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="0be91-657">Ajouter le paramètre - ManagementGroupName pour appliquer des opérations à un groupe de gestion donné</span><span class="sxs-lookup"><span data-stu-id="0be91-657">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="0be91-658">Ajouter le paramètre -SubscriptionId pour appliquer des opérations à un abonnement donné</span><span class="sxs-lookup"><span data-stu-id="0be91-658">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="0be91-659">Mettre à jour les cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="0be91-659">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="0be91-660">Ajouter le paramètre - ManagementGroupName pour appliquer des opérations à un groupe de gestion donné</span><span class="sxs-lookup"><span data-stu-id="0be91-660">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="0be91-661">Ajouter le paramètre -SubscriptionId pour appliquer des opérations à un abonnement donné</span><span class="sxs-lookup"><span data-stu-id="0be91-661">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="0be91-662">Ajouter la prise en charge des références secrètes des coffres de clés dans les paramètres lors de l’utilisation de TemplateParameterObject dans New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="0be91-662">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="0be91-663">Correction du problème où le paramètre EndDatea été ignoré pour New-AzureRmADAppCredential</span><span class="sxs-lookup"><span data-stu-id="0be91-663">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="0be91-664">Correction du problème où Add-AzureRmADGroupMember a utilisé une URL pour effectuer la demande</span><span class="sxs-lookup"><span data-stu-id="0be91-664">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="0be91-665">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0be91-665">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="0be91-666">Ajout du Parameter -KeyValue facultatif à la cmdlet New-AzureRmServiceBusKey, qui permet à l’utilisateur de fournir KeyValue.</span><span class="sxs-lookup"><span data-stu-id="0be91-666">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="0be91-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-667">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-668">Clarification des points de restauration définis par l’utilisateur pour SQLDW dans l’aide de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="0be91-668">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="0be91-669">Mise à jour de la documentation du paramètre - ComputeGeneration dans plusieurs cmdlets</span><span class="sxs-lookup"><span data-stu-id="0be91-669">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="0be91-670">6.3.0 - juin 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-670">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="0be91-671">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-671">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-672">Mise à jour des messages d’erreur pour la commande Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="0be91-672">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="0be91-673">Création d’un contexte pour chaque abonnement lors de l’exécution de la commande Connect-AzureRmAccount sans contexte précédent</span><span class="sxs-lookup"><span data-stu-id="0be91-673">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="0be91-674">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="0be91-674">Azure.Storage</span></span>
* <span data-ttu-id="0be91-675">Ajout d’informations supplémentaires sur le paramètre -Permissions dans les fichiers d’aide.</span><span class="sxs-lookup"><span data-stu-id="0be91-675">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-676">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-676">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-677">Get-AzureRmVmDiskEncryptionStatus résout un problème rencontré sur les machines virtuelles sans disques de données</span><span class="sxs-lookup"><span data-stu-id="0be91-677">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="0be91-678">Mise à jour de la version de la bibliothèque de client Compute pour résoudre les cmdlets suivantes</span><span class="sxs-lookup"><span data-stu-id="0be91-678">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="0be91-679">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="0be91-679">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="0be91-680">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="0be91-680">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="0be91-681">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="0be91-681">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="0be91-682">Problème relatif aux cmdlets suivantes résolu afin d’afficher « ID d’opération » et « État d’opération » correctement :</span><span class="sxs-lookup"><span data-stu-id="0be91-682">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="0be91-683">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="0be91-683">Start-AzureRmVM</span></span>
    - <span data-ttu-id="0be91-684">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="0be91-684">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="0be91-685">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="0be91-685">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="0be91-686">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="0be91-686">Set-AzureRmVM</span></span>
    - <span data-ttu-id="0be91-687">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="0be91-687">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="0be91-688">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="0be91-688">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="0be91-689">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="0be91-689">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="0be91-690">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="0be91-690">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="0be91-691">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="0be91-691">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="0be91-692">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="0be91-692">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="0be91-693">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="0be91-693">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="0be91-694">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="0be91-694">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="0be91-695">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="0be91-695">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="0be91-696">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="0be91-696">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="0be91-697">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="0be91-697">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="0be91-698">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="0be91-698">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="0be91-699">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="0be91-699">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="0be91-700">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="0be91-700">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="0be91-701">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="0be91-701">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="0be91-702">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="0be91-702">AzureRM.EventGrid</span></span>
* <span data-ttu-id="0be91-703">Suppression des conditions de validation de ValidateNotNullOrEmpty pour SubjectBeginsWith/SubjectEndsWith dans la cmdlet Update-AzureRmEventGridSubscription afin de changer ces paramètres pour vider la chaîne, si nécessaire.</span><span class="sxs-lookup"><span data-stu-id="0be91-703">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="0be91-704">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0be91-704">AzureRM.KeyVault</span></span>
* <span data-ttu-id="0be91-705">Résolution d’un problème où les balises sont retournées lorsque la commande Get-AzureRmKeyVault est exécutée</span><span class="sxs-lookup"><span data-stu-id="0be91-705">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="0be91-706">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0be91-706">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="0be91-707">Version publique des cmdlets Policy Insights</span><span class="sxs-lookup"><span data-stu-id="0be91-707">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="0be91-708">Utiliser l’API de version du 04/04/2018</span><span class="sxs-lookup"><span data-stu-id="0be91-708">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="0be91-709">Ajout de PolicyDefinitionReferenceId aux résultats de la commande Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="0be91-709">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="0be91-710">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="0be91-710">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="0be91-711">Ajout du paramètre -Vault aux cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="0be91-711">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="0be91-712">Une fois envoyé, il écrasera la cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="0be91-712">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="0be91-713">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-713">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-714">Mise à jour d’un exemple dans le fichier d’aide de la commande Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="0be91-714">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="0be91-715">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="0be91-715">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="0be91-716">Mise à jour du fichier d’aide de la commande Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-716">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="0be91-717">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="0be91-717">AzureRM.Websites</span></span>
* <span data-ttu-id="0be91-718">Mise à jour de la commande Set-AzureRMWebApp afin qu’elle n’écrase pas le paramètre AppSettings lors de l’exécution de -AssignIdentity</span><span class="sxs-lookup"><span data-stu-id="0be91-718">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="0be91-719">Mise à jour de la commande New-AzureRMWebAppSlot pour rendre optionnel le paramètre AppServicePlan</span><span class="sxs-lookup"><span data-stu-id="0be91-719">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="0be91-720">6.2.1 - juin 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-720">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="0be91-721">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0be91-721">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="0be91-722">Mise à jour du modèle PSWorkspace pour permettre à Network d’utiliser le type en paramètre</span><span class="sxs-lookup"><span data-stu-id="0be91-722">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="0be91-723">6.2.0 - Juin 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-723">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="0be91-724">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-724">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-725">Correction d’un problème où la version 10.0.3 de Newtonsoft.Json n’était pas chargée lors de l’importation du module</span><span class="sxs-lookup"><span data-stu-id="0be91-725">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="0be91-726">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="0be91-726">AzureRM.Compute</span></span>
* <span data-ttu-id="0be91-727">Fonctionnalité de mise à jour de machine virtuelle de groupe de machines virtuelles identiques (VMSS)</span><span class="sxs-lookup"><span data-stu-id="0be91-727">VMSS VM Update feature</span></span>
    - <span data-ttu-id="0be91-728">Ajout des cmdlet « Update-AzureRmVmssVM » et « New-AzureRmVMDataDisk »</span><span class="sxs-lookup"><span data-stu-id="0be91-728">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="0be91-729">Ajout du paramètre VirtualMachineScaleSetVM à la cmdlet « Add-AzureRmVMDataDisk » pour prendre en charge l’ajout d’un disque de données à un groupe de machines virtuelles identiques (VMSS).</span><span class="sxs-lookup"><span data-stu-id="0be91-729">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="0be91-730">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="0be91-730">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="0be91-731">Mise à jour du Kit de développement logiciel (SDK) .Net ADF vers la version 0.8.0 - préversion , qui contient les modifications suivantes :</span><span class="sxs-lookup"><span data-stu-id="0be91-731">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="0be91-732">Ajout de l’opération de référentiel de configuration de fabrique</span><span class="sxs-lookup"><span data-stu-id="0be91-732">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="0be91-733">Mise à jour des QuickBooks LinkedService pour exposer les propriétés consumerKey et consumerSecret</span><span class="sxs-lookup"><span data-stu-id="0be91-733">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="0be91-734">Mise à jour de plusieurs types de modèle de SecretBase à l’objet</span><span class="sxs-lookup"><span data-stu-id="0be91-734">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="0be91-735">Ajout d’un déclencheur d’événements d’objet Blob</span><span class="sxs-lookup"><span data-stu-id="0be91-735">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="0be91-736">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0be91-736">AzureRM.KeyVault</span></span>
* <span data-ttu-id="0be91-737">Mise à jour de la documentation avec l’exemple de sortie</span><span class="sxs-lookup"><span data-stu-id="0be91-737">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="0be91-738">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-738">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-739">Activation des paramètres Traffic Analytics sur les cmdlet Network Watcher</span><span class="sxs-lookup"><span data-stu-id="0be91-739">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="0be91-740">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="0be91-740">AzureRM.Resources</span></span>
* <span data-ttu-id="0be91-741">Résolution d’un problème où la propriété « Properties » des objets « PSResource » était retournée à partir de « Get-AzureRmResource »</span><span class="sxs-lookup"><span data-stu-id="0be91-741">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="0be91-742">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="0be91-742">AzureRM.Scheduler</span></span>
* <span data-ttu-id="0be91-743">Correction d’un problème de mise à jour où ServiceBusQueueJob ne définissait pas de nouvelles valeurs d’authentification</span><span class="sxs-lookup"><span data-stu-id="0be91-743">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="0be91-744">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-744">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-745">Mise à jour des cmdlet suivantes avec le paramètre facultatif LicenseType</span><span class="sxs-lookup"><span data-stu-id="0be91-745">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="0be91-746">New-AzureRmSqlDatabase ; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="0be91-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="0be91-747">New-AzureRmSqlElasticPool ; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="0be91-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="0be91-748">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="0be91-748">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="0be91-749">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="0be91-749">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="0be91-750">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="0be91-750">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="0be91-751">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="0be91-751">AzureRM.Websites</span></span>
* <span data-ttu-id="0be91-752">« New-AzureRMWebApp » est mis à jour pour utiliser des algorithmes communs à partir de la bibliothèque de stratégies.</span><span class="sxs-lookup"><span data-stu-id="0be91-752">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="0be91-753">6.1.0 - Mai 2018</span><span class="sxs-lookup"><span data-stu-id="0be91-753">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="0be91-754">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="0be91-754">AzureRM.Profile</span></span>
* <span data-ttu-id="0be91-755">Correction d’un problème où un contexte vide avec le nom du contexte par défaut précédent était conservé lors de l’exécution de « Clear-AzureRmContext », ce qui empêchait l’utilisateur de créer un nouveau contexte avec l’ancien nom</span><span class="sxs-lookup"><span data-stu-id="0be91-755">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="0be91-756">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0be91-756">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="0be91-757">Activation des opérations d’association/dissociation de passerelle sur les systèmes autonomes</span><span class="sxs-lookup"><span data-stu-id="0be91-757">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="0be91-758">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0be91-758">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="0be91-759">Ajout de la prise en charge des éléments ApiVersions, ApiReleases et ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="0be91-759">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="0be91-760">Ajout de la prise en charge du principal ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0be91-760">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="0be91-761">Ajout de la prise en charge de l’enregistreur d’événements Application Insights</span><span class="sxs-lookup"><span data-stu-id="0be91-761">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="0be91-762">Ajout de la reconnaissance de la référence « De base » comme une référence valide du service Gestion des Api</span><span class="sxs-lookup"><span data-stu-id="0be91-762">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="0be91-763">Ajout de la prise en charge de l’installation des certificats émis par une autorité de certification privée en tant que certificats racine ou d’autorité de certification</span><span class="sxs-lookup"><span data-stu-id="0be91-763">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="0be91-764">Ajout de la prise en charge des certificats SSL personnalisés via KeyVault et de plusieurs noms d’hôte de proxy</span><span class="sxs-lookup"><span data-stu-id="0be91-764">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="0be91-765">Ajout de la prise en charge de l’identité MSI</span><span class="sxs-lookup"><span data-stu-id="0be91-765">Added support for MSI identity</span></span>
* <span data-ttu-id="0be91-766">Ajout de la prise en charge des stratégies via une URL. REMARQUE : les cmdlet suivantes seront déconseillées dans une version ultérieure :</span><span class="sxs-lookup"><span data-stu-id="0be91-766">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="0be91-767">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="0be91-767">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="0be91-768">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-768">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="0be91-769">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="0be91-769">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="0be91-770">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="0be91-770">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="0be91-771">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="0be91-771">AzureRM.Batch</span></span>
* <span data-ttu-id="0be91-772">Ajout de la nouvelle cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="0be91-772">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="0be91-773">Ajout de la nouvelle cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="0be91-773">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="0be91-774">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="0be91-774">AzureRM.Consumption</span></span>
* <span data-ttu-id="0be91-775">Ajout des nouveaux paramètres Expand, ResourceGroup, InstanceName, InstanceId, Tags et Top pour la cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="0be91-775">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="0be91-776">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0be91-776">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="0be91-777">Correction de l’exemple pour Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="0be91-777">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="0be91-778">Correction de l’exception de paramètre Null pour le cas Recurse dans Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="0be91-778">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="0be91-779">Correction des fichiers d’aide pour Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl et Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="0be91-779">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="0be91-780">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="0be91-780">AzureRM.Network</span></span>
* <span data-ttu-id="0be91-781">Passage de la version du Kit de développement logiciel (SDK) Network de 18.0.0-preview à 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="0be91-781">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="0be91-782">Ajout d’une cmdlet pour créer une configuration de protocole :</span><span class="sxs-lookup"><span data-stu-id="0be91-782">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="0be91-783">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="0be91-783">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="0be91-784">Ajout d’une cmdlet pour ajouter une nouvelle connexion de circuit à un circuit ExpressRoute existant :</span><span class="sxs-lookup"><span data-stu-id="0be91-784">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="0be91-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="0be91-786">Ajout d’une cmdlet pour supprimer une connexion de circuit d’un circuit ExpressRoute existant :</span><span class="sxs-lookup"><span data-stu-id="0be91-786">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="0be91-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="0be91-788">Ajout d’une cmdlet pour récupérer une connexion de circuit :</span><span class="sxs-lookup"><span data-stu-id="0be91-788">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="0be91-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="0be91-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="0be91-790">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0be91-790">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="0be91-791">Correction de l’utilisation de l’authentification serveur avec les certificats générés (problème nº 5998)</span><span class="sxs-lookup"><span data-stu-id="0be91-791">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="0be91-792">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="0be91-792">AzureRM.Sql</span></span>
* <span data-ttu-id="0be91-793">Mise à jour des cmdlets d’audit pour permettre la suppression des éléments AuditAction ou AuditActionGroup</span><span class="sxs-lookup"><span data-stu-id="0be91-793">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="0be91-794">Correction d’un problème concernant Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy lors de la définition d’une nouvelle stratégie de rétention flexible, où la commande échouait avec le message d’erreur « Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="0be91-794">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="0be91-795">Please submit request with the new flexible retention policy » (La configuration d’une stratégie de rétention à long terme avec un coffre et une stratégie Azure Recovery Services n’est plus prise en charge. Veuillez soumettre une demande avec la nouvelle stratégie de rétention flexible.).</span><span class="sxs-lookup"><span data-stu-id="0be91-795">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="0be91-796">Mise à jour de toutes les cmdlets liées à la création/mise à jour de bases de données/pools élastiques Azure SQL pour utiliser la nouvelle API Base de données, qui prend en charge la propriété Sku pour les propriétés liées à la mise à l’échelle et au niveau.</span><span class="sxs-lookup"><span data-stu-id="0be91-796">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="0be91-797">Les cmdlets mises à jour incluent :</span><span class="sxs-lookup"><span data-stu-id="0be91-797">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="0be91-798">New-AzureRmSqlDatabase ; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="0be91-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="0be91-799">New-AzureRmSqlElasticPool ; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="0be91-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="0be91-800">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="0be91-800">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="0be91-801">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="0be91-801">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="0be91-802">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="0be91-802">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="0be91-803">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="0be91-803">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="0be91-804">Mise à jour des paramètres pour « Get-AzureRmTrafficManagerProfile » afin que le paramètre -ResourceGroupName soit requis lors de l’utilisation du paramètre -name</span><span class="sxs-lookup"><span data-stu-id="0be91-804">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>