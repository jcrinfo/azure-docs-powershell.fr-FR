<span data-ttu-id="6bcb3-101">Programme d’installation d’Azure PowerShell 4.3.1 : [lien](https://github.com/Azure/azure-powershell/releases/download/v4.3.1-August2017/azure-powershell.4.3.1.msi)</span><span class="sxs-lookup"><span data-stu-id="6bcb3-101">Azure PowerShell 4.3.1 Installer: [link](https://github.com/Azure/azure-powershell/releases/download/v4.3.1-August2017/azure-powershell.4.3.1.msi)</span></span>

<span data-ttu-id="6bcb3-102">Module de la galerie pour les applets de commande ARM : [lien](https://www.powershellgallery.com/packages/AzureRM/4.3.1)</span><span class="sxs-lookup"><span data-stu-id="6bcb3-102">Gallery Module for ARM Cmdlets: [link](https://www.powershellgallery.com/packages/AzureRM/4.3.1)</span></span>

<span data-ttu-id="6bcb3-103">Module de la galerie pour les applets de commande héritées pour la gestion du Service (RDFE) : [lien](https://www.powershellgallery.com/packages/Azure/4.3.1)</span><span class="sxs-lookup"><span data-stu-id="6bcb3-103">Gallery Module for Legacy Cmdlets for Service Management (RDFE): [link](https://www.powershellgallery.com/packages/Azure/4.3.1)</span></span>

## <a name="changes-in-431"></a><span data-ttu-id="6bcb3-104">Changements dans 4.3.1</span><span class="sxs-lookup"><span data-stu-id="6bcb3-104">Changes in 4.3.1</span></span>

- <span data-ttu-id="6bcb3-105">Problème résolu avec certains assemblys non signés qui entraînaient une erreur `could not load file or assembly` à l’importation des modules</span><span class="sxs-lookup"><span data-stu-id="6bcb3-105">Fixed issue with certain assemblies not being signed, resulting in an `could not load file or assembly` error when modules were imported</span></span>

## <a name="changes-in-430"></a><span data-ttu-id="6bcb3-106">Changements dans 4.3.0</span><span class="sxs-lookup"><span data-stu-id="6bcb3-106">Changes in 4.3.0</span></span>

* <span data-ttu-id="6bcb3-107">AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6bcb3-107">AnalysisServices</span></span>
    * <span data-ttu-id="6bcb3-108">Résolution du bogue dans Set-AzureRmAnalysisServciesServer</span><span class="sxs-lookup"><span data-stu-id="6bcb3-108">Fixed bug in Set-AzureRmAnalysisServciesServer</span></span>
        - <span data-ttu-id="6bcb3-109">Lorsque l’administrateur n’est pas fourni, il est supprimé.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-109">When admin was not provided, the admin will be removed.</span></span>
    * <span data-ttu-id="6bcb3-110">Ajout de BackupBlobContainerUri dans New-AzureRmAnalysisServicesServer et Set-AzureRmAnalysisServicesServer</span><span class="sxs-lookup"><span data-stu-id="6bcb3-110">Added BackupBlobContainerUri in New-AzureRmAnalysisServicesServer and Set-AzureRmAnalysisServicesServer</span></span>
        - <span data-ttu-id="6bcb3-111">Activer pour définir/désactiver le conteneur d’objets blob de sauvegarde pour la sauvegarde/restauration du serveur Azure Analysis Services</span><span class="sxs-lookup"><span data-stu-id="6bcb3-111">Enable to set/disable backup blob container for backup/restore Azure Analysis Services Server</span></span>
    * <span data-ttu-id="6bcb3-112">Mise à jour de la recherche de référence SKU dans New-AzureRmAnalysisServicesServer et Set-AzureRmAnalysisServicesServer</span><span class="sxs-lookup"><span data-stu-id="6bcb3-112">Updated Sku lookup in New-AzureRmAnalysisServicesServer and Set-AzureRmAnalysisServicesServer</span></span>
        - <span data-ttu-id="6bcb3-113">Remplacement de la recherche de référence SKU codée en dur par une recherche dynamique.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-113">Changed hard coded Sku into dynamic lookup.</span></span>
    * <span data-ttu-id="6bcb3-114">Add-AzureAnalysisServicesAccount pour prendre en charge la connexion avec le principal de service</span><span class="sxs-lookup"><span data-stu-id="6bcb3-114">Add-AzureAnalysisServicesAccount to support login with Service Principal</span></span>
* <span data-ttu-id="6bcb3-115">Automatisation</span><span class="sxs-lookup"><span data-stu-id="6bcb3-115">Automation</span></span>
    * <span data-ttu-id="6bcb3-116">Modifications apportées aux applets de commande AutomationDSC * pour extraire plus de 100 enregistrements</span><span class="sxs-lookup"><span data-stu-id="6bcb3-116">Made changes to AutomationDSC* cmdlets to pull more than 100 records</span></span>
    * <span data-ttu-id="6bcb3-117">Résolution du problème des flux de commentaires qui arrêtaient de fonctionner après l’appel de certaines applets de commande d’automatisation (par exemple, Get-AzureRmAutomationVariable, Get-AzureRmAutomationJob).</span><span class="sxs-lookup"><span data-stu-id="6bcb3-117">Resolved the issue where the Verbose streams stop working after calling some Automation cmdlets (for example Get-AzureRmAutomationVariable, Get-AzureRmAutomationJob).</span></span>
    * <span data-ttu-id="6bcb3-118">Ajout de la prise en charge de la gestion des versions de build NodeConfiguration dans StartAzureAutomationDscCompilationJob et ImportAzureAutomationDscNodeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-118">Support for NodeConfiguration Build versioning added in StartAzureAutomationDscCompilationJob and ImportAzureAutomationDscNodeConfiguration.</span></span>
    * <span data-ttu-id="6bcb3-119">Correctifs de bogues pour les problèmes existants - Résolution du problème d’alias n°3775 et de l’alias runOn, ainsi que de la prise en charge pour HybridWorkers.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-119">Bug fixes for existing issues - Fixes the alias issue is #3775 and the runOn alias and support for HybridWorkers.</span></span>
* <span data-ttu-id="6bcb3-120">Calcul</span><span class="sxs-lookup"><span data-stu-id="6bcb3-120">Compute</span></span>
    * <span data-ttu-id="6bcb3-121">Set-AzureRmVMAEMExtension : Ajout de la prise en charge des nouvelles tailles de disque Premium</span><span class="sxs-lookup"><span data-stu-id="6bcb3-121">Set-AzureRmVMAEMExtension: Add support for new Premium Disk sizes</span></span>
    * <span data-ttu-id="6bcb3-122">Set-AzureRmVMAEMExtension : Ajout de la prise en charge de la série M</span><span class="sxs-lookup"><span data-stu-id="6bcb3-122">Set-AzureRmVMAEMExtension: Add support for M series</span></span>
    * <span data-ttu-id="6bcb3-123">Ajout du paramètre ForceUpdateTag à Add-AzureRmVmssExtension</span><span class="sxs-lookup"><span data-stu-id="6bcb3-123">Add ForceUpdateTag parameter to Add-AzureRmVmssExtension</span></span>
    * <span data-ttu-id="6bcb3-124">Ajout du paramètre Primary à New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="6bcb3-124">Add Primary parameter to New-AzureRmVmssIpConfig</span></span>
    * <span data-ttu-id="6bcb3-125">Ajout du paramètre EnableAcceleratedNetworking à Add-AzureRmVmssNetworkInterfaceConfig</span><span class="sxs-lookup"><span data-stu-id="6bcb3-125">Add EnableAcceleratedNetworking parameter to Add-AzureRmVmssNetworkInterfaceConfig</span></span>
    * <span data-ttu-id="6bcb3-126">Ajout de InstanceId à Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="6bcb3-126">Add InstanceId to Set-AzureRmVmss</span></span>
    * <span data-ttu-id="6bcb3-127">Exposition de MaintenanceRedeployStatus à la sortie Get-AzureRmVM-Status</span><span class="sxs-lookup"><span data-stu-id="6bcb3-127">Expose MaintenanceRedeployStatus to Get-AzureRmVM -Status output</span></span>
    * <span data-ttu-id="6bcb3-128">Exposition de Restriction et de Capability au format de tableau de Get-AzureRmComputeResourceSku</span><span class="sxs-lookup"><span data-stu-id="6bcb3-128">Expose Restriction and Capability to the table format of Get-AzureRmComputeResourceSku</span></span>
* <span data-ttu-id="6bcb3-129">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6bcb3-129">DataLakeStore</span></span>
    * <span data-ttu-id="6bcb3-130">Correctif du problème : https://github.com/Azure/azure-powershell/issues/4323</span><span class="sxs-lookup"><span data-stu-id="6bcb3-130">Fix for issue: https://github.com/Azure/azure-powershell/issues/4323</span></span>
* <span data-ttu-id="6bcb3-131">Event Hub</span><span class="sxs-lookup"><span data-stu-id="6bcb3-131">EventHub</span></span>
    * <span data-ttu-id="6bcb3-132">Ajout de la propriété ResourceGroup à NamespaceAttributes</span><span class="sxs-lookup"><span data-stu-id="6bcb3-132">added ResourceGroup property to NamespaceAttributes</span></span>
        - <span data-ttu-id="6bcb3-133">ResourceGroup - Obtient le nom du groupe de ressources dans lequel se trouve Namespace</span><span class="sxs-lookup"><span data-stu-id="6bcb3-133">'ResourceGroup' Gets the name of the resource group the Namespace is in</span></span>
    * <span data-ttu-id="6bcb3-134">Mise à jour des applets de commande avec le nouveau paramètre et l’alias de paramètre</span><span class="sxs-lookup"><span data-stu-id="6bcb3-134">updated commandlets with new parameter and parameter alias</span></span>
        - <span data-ttu-id="6bcb3-135">Mise à jour des applets de commande ci-dessous avec les jeux de paramètres pour Namespace et EventHub dans l’opération d’AuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-135">below cmdlets updated with Parametersets for Namespace and EventHub for operation of AuthorizationRule</span></span>
        - <span data-ttu-id="6bcb3-136">New-AzureRmEventHubAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-136">New-AzureRmEventHubAuthorizationRule</span></span>
            + <span data-ttu-id="6bcb3-137">Ajoute une nouvelle règle AuthorizationRule au NameSpace ou EventHub existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-137">Adds a new AuthorizationRule to the existing NameSpace or EventHub.</span></span>
        - <span data-ttu-id="6bcb3-138">Get-AzureRmEventHubAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-138">Get-AzureRmEventHubAuthorizationRule</span></span>
            + <span data-ttu-id="6bcb3-139">Obtient la règle AuthorizationRule / la liste des AuthorizationRules pour le NameSpace ou l’EventHub existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-139">Gets AuthorizationRule / List of AuthorizationRules for the existing NameSpace or EventHub.</span></span>
        - <span data-ttu-id="6bcb3-140">Set-AzureRmEventHubAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-140">Set-AzureRmEventHubAuthorizationRule</span></span>
            + <span data-ttu-id="6bcb3-141">Met à jour les propriétés de la règle AuthorizationRule existante de l’EventHub NameSpace.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-141">Updates properties of existing AuthorizationRule of EventHub NameSpace.</span></span>
        - <span data-ttu-id="6bcb3-142">Remove-AzureRmEventHubAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-142">Remove-AzureRmEventHubAuthorizationRule</span></span>
            + <span data-ttu-id="6bcb3-143">Supprime la règle AuthorizationRule existante du NameSpace ou de l’EventHub existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-143">Deletes the existing AuthorizationRule of existing NameSpace or EventHub.</span></span>
        - <span data-ttu-id="6bcb3-144">New-AzureRmEventHubKey</span><span class="sxs-lookup"><span data-stu-id="6bcb3-144">New-AzureRmEventHubKey</span></span>
            + <span data-ttu-id="6bcb3-145">Génère une nouvelle clé principale/secondaire pour la règle AuthorizationRule du NameSpace ou de l’EventHub existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-145">Generates a new Primary/Secondary Key for AuthorizationRule of existing NameSpace or EventHub.</span></span>
        - <span data-ttu-id="6bcb3-146">Get-AzureRmEventHubKey</span><span class="sxs-lookup"><span data-stu-id="6bcb3-146">Get-AzureRmEventHubKey</span></span>
            + <span data-ttu-id="6bcb3-147">Obtient la clé principale/secondaire pour la règle AuthorizationRule du NameSpace ou de l’EventHub existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-147">Gets Primary/Secondary Key for AuthorizationRule of existing NameSpace or EventHub.</span></span>
* <span data-ttu-id="6bcb3-148">Réseau</span><span class="sxs-lookup"><span data-stu-id="6bcb3-148">Network</span></span>
    * <span data-ttu-id="6bcb3-149">New-AzureRmExpressRouteCircuitPeeringConfig : ajout de la prise en charge d’IPv6.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-149">New-AzureRmExpressRouteCircuitPeeringConfig: Added IPv6 support.</span></span> <span data-ttu-id="6bcb3-150">Nouveau paramètre facultatif ajouté</span><span class="sxs-lookup"><span data-stu-id="6bcb3-150">New optional parameter added</span></span>
        - <span data-ttu-id="6bcb3-151">PeerAddressType</span><span class="sxs-lookup"><span data-stu-id="6bcb3-151">PeerAddressType</span></span>
    * <span data-ttu-id="6bcb3-152">Set-AzureRmExpressRouteCircuitPeeringConfig : ajout de la prise en charge d’IPv6.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-152">Set-AzureRmExpressRouteCircuitPeeringConfig: Added IPv6 support.</span></span> <span data-ttu-id="6bcb3-153">Nouveau paramètre facultatif ajouté</span><span class="sxs-lookup"><span data-stu-id="6bcb3-153">New optional parameter added</span></span>
        - <span data-ttu-id="6bcb3-154">PeerAddressType</span><span class="sxs-lookup"><span data-stu-id="6bcb3-154">PeerAddressType</span></span>
    * <span data-ttu-id="6bcb3-155">Remove-AzureRmExpressRouteCircuitPeeringConfig : ajout de la prise en charge d’IPv6.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-155">Remove-AzureRmExpressRouteCircuitPeeringConfig: Added IPv6 support.</span></span> <span data-ttu-id="6bcb3-156">Nouveau paramètre facultatif ajouté</span><span class="sxs-lookup"><span data-stu-id="6bcb3-156">New optional parameter added</span></span>
        - <span data-ttu-id="6bcb3-157">PeerAddressType</span><span class="sxs-lookup"><span data-stu-id="6bcb3-157">PeerAddressType</span></span>
    * <span data-ttu-id="6bcb3-158">Paramètre marqué - ProbeEnabled comme obsolète</span><span class="sxs-lookup"><span data-stu-id="6bcb3-158">Marked parameter -ProbeEnabled as obsolete</span></span>
        - <span data-ttu-id="6bcb3-159">Add-AzureRmApplicationGatewayBackendHttpSettings</span><span class="sxs-lookup"><span data-stu-id="6bcb3-159">Add-AzureRmApplicationGatewayBackendHttpSettings</span></span>
        - <span data-ttu-id="6bcb3-160">New-AzureRmApplicationGatewayBackendHttpSettings</span><span class="sxs-lookup"><span data-stu-id="6bcb3-160">New-AzureRmApplicationGatewayBackendHttpSettings</span></span>
        - <span data-ttu-id="6bcb3-161">Set-AzureRmApplicationGatewayBackendHttpSettings</span><span class="sxs-lookup"><span data-stu-id="6bcb3-161">Set-AzureRmApplicationGatewayBackendHttpSettings</span></span>
* <span data-ttu-id="6bcb3-162">Profil</span><span class="sxs-lookup"><span data-stu-id="6bcb3-162">Profile</span></span>
    * <span data-ttu-id="6bcb3-163">La collecte de données a été activée par défaut.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-163">Data collection has been enabled by default.</span></span> <span data-ttu-id="6bcb3-164">Les données d’utilisation sont collectées par Microsoft afin d’améliorer l’expérience utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-164">Usage data is collected by Microsoft in order to improve the user experience.</span></span> <span data-ttu-id="6bcb3-165">Les données sont anonymes et n’incluent pas de valeurs d’argument de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-165">The data is anonymous and does not include command-line argument values.</span></span>
        - <span data-ttu-id="6bcb3-166">Utilisation de l’applet de commande Disable-AzureRmDataCollection pour désactiver la fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="6bcb3-166">Use the Disable-AzureRmDataCollection cmdlet to turn the feature off</span></span>
        - <span data-ttu-id="6bcb3-167">Utilisation de l’applet de commande Enable-AzureRmDataCollection pour activer la fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="6bcb3-167">Use the Enable-AzureRmDataCollection cmdlet to turn this feature on</span></span>
* <span data-ttu-id="6bcb3-168">Ressources</span><span class="sxs-lookup"><span data-stu-id="6bcb3-168">Resources</span></span>
    * <span data-ttu-id="6bcb3-169">Ajout de la prise en charge de la validation des étendues des applets de commande roledefinition et roleassignment suivantes avant l’envoi de la requête à ARM</span><span class="sxs-lookup"><span data-stu-id="6bcb3-169">Add Support for validation of scopes for the following roledefinition and roleassignment commandlets before sending the request to ARM</span></span>
        - <span data-ttu-id="6bcb3-170">Get-AzureRMRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6bcb3-170">Get-AzureRMRoleAssignment</span></span>
        - <span data-ttu-id="6bcb3-171">New-AzureRMRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6bcb3-171">New-AzureRMRoleAssignment</span></span>
        - <span data-ttu-id="6bcb3-172">Remove-AzureRMRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6bcb3-172">Remove-AzureRMRoleAssignment</span></span>
        - <span data-ttu-id="6bcb3-173">Get-AzureRMRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bcb3-173">Get-AzureRMRoleDefinition</span></span>
        - <span data-ttu-id="6bcb3-174">New-AzureRMRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bcb3-174">New-AzureRMRoleDefinition</span></span>
        - <span data-ttu-id="6bcb3-175">Remove-AzureRMRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bcb3-175">Remove-AzureRMRoleDefinition</span></span>
        - <span data-ttu-id="6bcb3-176">Set-AzureRMRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bcb3-176">Set-AzureRMRoleDefinition</span></span>
* <span data-ttu-id="6bcb3-177">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6bcb3-177">ServiceBus</span></span>
    * <span data-ttu-id="6bcb3-178">Ajout ci-dessous de nouvelles applets de commande pour AuthorizationRules pour NameSpace, Queue et Topic.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-178">Added below new commandlets for AuthorizationRules for NameSpace, Queue and Topic.</span></span> <span data-ttu-id="6bcb3-179">En fonction du jeu de paramètres, les opérations de règle d’autorisation sont effectuées.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-179">according to parameter set the authorization rule orperations are perfomed.</span></span>
     - <span data-ttu-id="6bcb3-180">New-AzureRmServiceBusAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-180">New-AzureRmServiceBusAuthorizationRule</span></span>
       - <span data-ttu-id="6bcb3-181">Ajoute une nouvelle règle AuthorizationRule au NameSpace/Queue/Topic ServiceBus existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-181">Adds a new AuthorizationRule to the existing ServiceBus NameSpace/Queue/Topic.</span></span>
     - <span data-ttu-id="6bcb3-182">Get-AzureRmServiceBusAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-182">Get-AzureRmServiceBusAuthorizationRule</span></span>
       - <span data-ttu-id="6bcb3-183">Obtient la règle AuthorizationRule / la liste des AuthorizationRules pour le NameSpace/Queue/Topic ServiceBus existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-183">Gets AuthorizationRule / List of AuthorizationRules for the existing ServiceBus NameSpace/Queue/Topic.</span></span>
     - <span data-ttu-id="6bcb3-184">Set-AzureRmServiceBusAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-184">Set-AzureRmServiceBusAuthorizationRule</span></span>
       - <span data-ttu-id="6bcb3-185">Met à jour les propriétés de la règle AuthorizationRule existante du NameSpace/Queue/Topic ServiceBus.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-185">Updates properties of existing AuthorizationRule of Servicebus NameSpace/Queue/Topic.</span></span>
     - <span data-ttu-id="6bcb3-186">New-AzureRmServiceBusKey</span><span class="sxs-lookup"><span data-stu-id="6bcb3-186">New-AzureRmServiceBusKey</span></span>
       - <span data-ttu-id="6bcb3-187">Génère une nouvelle clé principale/secondaire pour la règle AuthorizationRule du NameSpace/Queue/Topic ServiceBus existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-187">Generates a new Primary/Secondary Key for AuthorizationRule of existing ServiceBus NameSpace/Queue/Topic.</span></span>
     - <span data-ttu-id="6bcb3-188">Get-AzureRmServiceBusKey</span><span class="sxs-lookup"><span data-stu-id="6bcb3-188">Get-AzureRmServiceBusKey</span></span>
       - <span data-ttu-id="6bcb3-189">Obtient une nouvelle clé principale/secondaire pour la règle AuthorizationRule du NameSpace/Queue/Topic ServiceBus existant.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-189">Gets Primary/Secondary Key for AuthorizationRule of existing ServiceBus NameSpace/Queue/Topic.</span></span>
     - <span data-ttu-id="6bcb3-190">Remove-AzureRmServiceBusNamespaceAuthorizationRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-190">Remove-AzureRmServiceBusNamespaceAuthorizationRule</span></span>
       - <span data-ttu-id="6bcb3-191">Supprime la règle AuthorizationRule existante du NameSpace/Queue/Topic ServiceBus.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-191">Deletes the existing AuthorizationRule of ServiceBus NameSpace/Queue/Topic.</span></span>
    * <span data-ttu-id="6bcb3-192">Ajout de la propriété ResourceGroup à NamespaceAttributes</span><span class="sxs-lookup"><span data-stu-id="6bcb3-192">Added Resource Group property to NamespceAttributes</span></span>
* <span data-ttu-id="6bcb3-193">SQL</span><span class="sxs-lookup"><span data-stu-id="6bcb3-193">Sql</span></span>
    * <span data-ttu-id="6bcb3-194">Mise à jour de Set-AzureRmSqlServerTransparentDataEncryptionProtector pour afficher un avertissement et demander confirmation que le Type du protecteur de chiffrement est bien défini sur AzureKeyVault</span><span class="sxs-lookup"><span data-stu-id="6bcb3-194">Updating Set-AzureRmSqlServerTransparentDataEncryptionProtector to display a warning and require confirmation if the Encryption Protector Type is being set to AzureKeyVault</span></span>
    * <span data-ttu-id="6bcb3-195">Ajout de nouvelles applets de commande mises à jour pour les paramètres d’audit</span><span class="sxs-lookup"><span data-stu-id="6bcb3-195">Adding new updated cmdlets for Auditing settings</span></span>
        - <span data-ttu-id="6bcb3-196">Ajout de l’applet de commande Get-AzureRmSqlDatabaseAuditing qui obtient les paramètres d’audit d’une base de données SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-196">Adding Get-AzureRmSqlDatabaseAuditing cmdlet which gets the auditing settings of an Azure SQL database.</span></span>
        - <span data-ttu-id="6bcb3-197">Ajout de l’applet de commande Get-AzureRmSqlServerAuditing qui obtient les paramètres d’audit d’un serveur SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-197">Adding Get-AzureRmSqlServerAuditing cmdlet which gets the auditing settings of an Azure SQL server.</span></span>
        - <span data-ttu-id="6bcb3-198">Ajout de l’applet de commande Set-AzureRmSqlDatabaseAuditing qui change les paramètres d’audit d’une base de données SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-198">Adding Set-AzureRmSqlDatabaseAuditing cmdlet which changes the auditing settings for an Azure SQL database.</span></span>
        - <span data-ttu-id="6bcb3-199">Ajout de l’applet de commande Set-AzureRmSqlServerAuditing qui change les paramètres d’audit d’un serveur SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-199">Adding Set-AzureRmSqlServerAuditing cmdlet which changes the auditing settings of an Azure SQL server.</span></span>
    * <span data-ttu-id="6bcb3-200">Dépréciation des applets de commande de stratégie d’audit existantes</span><span class="sxs-lookup"><span data-stu-id="6bcb3-200">Deprecating the existing Auditing policy cmdlets</span></span>
        - <span data-ttu-id="6bcb3-201">Dépréciation de Get-AzureRmSqlDatabaseAuditingPolicy</span><span class="sxs-lookup"><span data-stu-id="6bcb3-201">Deprecating Get-AzureRmSqlDatabaseAuditingPolicy</span></span>
        - <span data-ttu-id="6bcb3-202">Dépréciation de Get-AzureRmSqlServerAuditingPolicy</span><span class="sxs-lookup"><span data-stu-id="6bcb3-202">Deprecating Get-AzureRmSqlServerAuditingPolicy</span></span>
        - <span data-ttu-id="6bcb3-203">Dépréciation de Set-AzureRmSqlDatabaseAuditingPolicy</span><span class="sxs-lookup"><span data-stu-id="6bcb3-203">Deprecating Set-AzureRmSqlDatabaseAuditingPolicy</span></span>
        - <span data-ttu-id="6bcb3-204">Dépréciation de Set-AzureRmSqlServerAuditingPolicy</span><span class="sxs-lookup"><span data-stu-id="6bcb3-204">Deprecating Set-AzureRmSqlServerAuditingPolicy</span></span>
        - <span data-ttu-id="6bcb3-205">Dépréciation de Use-AzureRmSqlServerAuditingPolicy</span><span class="sxs-lookup"><span data-stu-id="6bcb3-205">Deprecating Use-AzureRmSqlServerAuditingPolicy</span></span>
        - <span data-ttu-id="6bcb3-206">Dépréciation de Remove-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="6bcb3-206">Deprecating Remove-AzureRmSqlDatabaseAuditing</span></span>
        - <span data-ttu-id="6bcb3-207">Dépréciation de Remove-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="6bcb3-207">Deprecating Remove-AzureRmSqlServerAuditing</span></span>
    * <span data-ttu-id="6bcb3-208">L’analyse du fichier de schéma pour Update-AzureRmSqlSyncGroup ne tient désormais plus compte de la casse.</span><span class="sxs-lookup"><span data-stu-id="6bcb3-208">Schema file parsing for Update-AzureRmSqlSyncGroup is now case insensitive.</span></span>
* <span data-ttu-id="6bcb3-209">Storage</span><span class="sxs-lookup"><span data-stu-id="6bcb3-209">Storage</span></span>
    * <span data-ttu-id="6bcb3-210">Ajout de la prise en charge de NeworkRule aux applets de commande de compte de stockage du mode de ressources</span><span class="sxs-lookup"><span data-stu-id="6bcb3-210">Add NeworkRule support to resource mode storage account cmdlets</span></span>
        - <span data-ttu-id="6bcb3-211">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6bcb3-211">New-AzureRmStorageAccount</span></span>
        - <span data-ttu-id="6bcb3-212">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="6bcb3-212">Set-AzureRmStorageAccount</span></span>
        - <span data-ttu-id="6bcb3-213">Get-AzureRmStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="6bcb3-213">Get-AzureRmStorageAccountNetworkRuleSet</span></span>
        - <span data-ttu-id="6bcb3-214">Update-AzureRmStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="6bcb3-214">Update-AzureRmStorageAccountNetworkRuleSet</span></span>
        - <span data-ttu-id="6bcb3-215">Add-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-215">Add-AzureRmStorageAccountNetworkRule</span></span>
        - <span data-ttu-id="6bcb3-216">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="6bcb3-216">Remove-AzureRmStorageAccountNetworkRule</span></span>

<span data-ttu-id="6bcb3-217">Voir [les modifications apportées depuis la dernière version](https://github.com/Azure/azure-powershell/compare/v4.2.1-July2017...v4.3.1-August2017)</span><span class="sxs-lookup"><span data-stu-id="6bcb3-217">View [changes since last release](https://github.com/Azure/azure-powershell/compare/v4.2.1-July2017...v4.3.1-August2017)</span></span>