---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
ms.assetid: E460D108-2BF9-4F57-AF3D-13868DC73EA0
online version: 
schema: 2.0.0
---

# New-AzureRmRoleAssignment

## SYNOPSIS
Assigns the specified RBAC role to the specified principal, at the specified scope.

## SYNTAX

### EmptyParameterSet (Default)
```
New-AzureRmRoleAssignment -ObjectId <Guid> -Scope <String> -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ScopeWithObjectIdParameterSet
```
New-AzureRmRoleAssignment -ObjectId <Guid> [-Scope <String>] -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ResourceWithObjectIdParameterSet
```
New-AzureRmRoleAssignment -ObjectId <Guid> -ResourceGroupName <String> -ResourceName <String>
 -ResourceType <String> [-ParentResource <String>] -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ResourceGroupWithObjectIdParameterSet
```
New-AzureRmRoleAssignment -ObjectId <Guid> -ResourceGroupName <String> -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### RoleIdWithScopeAndObjectIdParameterSet
```
New-AzureRmRoleAssignment -ObjectId <Guid> -Scope <String> -RoleDefinitionId <Guid>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ResourceWithSignInNameParameterSet
```
New-AzureRmRoleAssignment -SignInName <String> -ResourceGroupName <String> -ResourceName <String>
 -ResourceType <String> [-ParentResource <String>] -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ResourceGroupWithSignInNameParameterSet
```
New-AzureRmRoleAssignment -SignInName <String> -ResourceGroupName <String> -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ScopeWithSignInNameParameterSet
```
New-AzureRmRoleAssignment -SignInName <String> [-Scope <String>] -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ResourceGroupWithSPNParameterSet
```
New-AzureRmRoleAssignment -ServicePrincipalName <String> -ResourceGroupName <String>
 -RoleDefinitionName <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ResourceWithSPNParameterSet
```
New-AzureRmRoleAssignment -ServicePrincipalName <String> -ResourceGroupName <String> -ResourceName <String>
 -ResourceType <String> [-ParentResource <String>] -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### ScopeWithSPNParameterSet
```
New-AzureRmRoleAssignment -ServicePrincipalName <String> [-Scope <String>] -RoleDefinitionName <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
The **New-AzureRMRoleAssignment** cmdlet assigns the specified RBAC role to the specified principal, at the specified scope.

Access is granted by assigning the appropriate RBAC role to them at the right scope.
To grant access to the entire subscription, assign a role at the subscription scope.
To grant access to a specific resource group within a subscription, assign a role at the resource group scope.

The subject of the assignment must be specified.
To specify a user, use the *SignInName* or *ObjectId* parameters.
To specify a security group, use the *ObjectId* parameter.
And to specify an Azure AD application, use the *ServicePrincipalName* or *ObjectId* parameters.

The role that is being assigned must be specified using the *RoleDefinitionName* parameter.

The scope at which access is being granted may be specified.
It defaults to the selected subscription. 
The scope of the assignment can be specified using one of the following parameter combinations:
        
- *Scope* - This is the fully qualified scope starting with /subscriptions/\<subscriptionId\>

- *ResourceGroupName* - to grant access to the specified resource group.

- *ResourceName*, *ResourceType*, *ResourceGroupName*, and *ParentResource* - to specify a particular resource within a resource group to grant access to.

## EXAMPLES

### Example 1: Grant reader role access to a user


```
PS C:\> New-AzureRmRoleAssignment -ResourceGroupName rg1 -SignInName "patti.fuller@contoso.com" -RoleDefinitionName Reader
```

This command grants reader role access to a user at a resource group scope.

### Example 2: Grant access to a security group


```
PS C:\> Get-AzureRMADGroup -SearchString "PattiFuller"

          DisplayName                    Type                           ObjectId
          -----------                    ----                           --------
          PattiFuller                                                   2f9d4375-cbf1-48e8-83c9-2a0be4cb33fb

          PS C:\> New-AzureRmRoleAssignment -ObjectId 2f9d4375-cbf1-48e8-83c9-2a0be4cb33fb -RoleDefinitionName Contributor  -ResourceGroupName rg1
```

This command grants access to a security group.

### Example 3: Grant access to a resource


```
PS C:\> New-AzureRmRoleAssignment -SignInName john.doe@contoso.com -RoleDefinitionName Owner -Scope "/subscription/86f81fc3-b00f-48cd-8218-3879f51ff362/resourcegroups/rg1/providers/Microsoft.Web/sites/site1"
```

This command grants access to a user at a website resource.

### Example 4: Grant access to a nested resource


```
PS C:\> New-AzureRMRoleAssignment -ObjectId 5ac84765-1c8c-4994-94b2-629461bd191b -RoleDefinitionName "Virtual Machine Contributor" -ResourceName Devices-Engineering-ProjectRND -ResourceType Microsoft.Network/virtualNetworks/subnets -ParentResource virtualNetworks/VNET-EASTUS-01 -ResourceGroupName Network
```

This command grants access to a group at a nested subnet resource.

## PARAMETERS

### -ObjectId
Specifies an Azure Active Directory object ID of the user, group or service principal.

```yaml
Type: Guid
Parameter Sets: EmptyParameterSet, ScopeWithObjectIdParameterSet, ResourceWithObjectIdParameterSet, ResourceGroupWithObjectIdParameterSet, RoleIdWithScopeAndObjectIdParameterSet
Aliases: Id, PrincipalId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Scope
Specifies the scope of the role assignment.
In the format of relative URI.
For instance,
"/subscriptions/9004a9fd-d58e-48dc-aeb2-4a4aec58606f/resourceGroups/TestRG".

If not specified, will create the role assignment at subscription level.
If specified, it should start with "/subscriptions/{id}".

```yaml
Type: String
Parameter Sets: EmptyParameterSet, RoleIdWithScopeAndObjectIdParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ScopeWithObjectIdParameterSet, ScopeWithSignInNameParameterSet, ScopeWithSPNParameterSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RoleDefinitionName
Specifies the name of the RBAC role that needs to be assigned to the principal.
For instance: Reader, Contributor, Virtual Network Administrator.

```yaml
Type: String
Parameter Sets: EmptyParameterSet, ScopeWithObjectIdParameterSet, ResourceWithObjectIdParameterSet, ResourceGroupWithObjectIdParameterSet, ResourceWithSignInNameParameterSet, ResourceGroupWithSignInNameParameterSet, ScopeWithSignInNameParameterSet, ResourceGroupWithSPNParameterSet, ResourceWithSPNParameterSet, ScopeWithSPNParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group.
Creates an assignment that is effective at the specified resource group.
When used in conjunction with the *ResourceName*, *ResourceType*, and *ParentResource* parameters, the command constructs a hierarchical scope in the form of a relative URI that identifies a resource.

```yaml
Type: String
Parameter Sets: ResourceWithObjectIdParameterSet, ResourceGroupWithObjectIdParameterSet, ResourceWithSignInNameParameterSet, ResourceGroupWithSignInNameParameterSet, ResourceGroupWithSPNParameterSet, ResourceWithSPNParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceName
Specifies the name of the resource.

This parameter should only be used in conjunction with the *ResourceGroupName*, *ResourceType*, and *ParentResource* parameters to construct a hierarchical scope in the form of a relative URI that identifies a resource.

```yaml
Type: String
Parameter Sets: ResourceWithObjectIdParameterSet, ResourceWithSignInNameParameterSet, ResourceWithSPNParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceType
Specifies the resource type.

This parameter should only be used in conjunction with the *ResourceGroupName*, *ResourceName*, and *ParentResource* parameters to construct a hierarchical scope in the form of a relative URI that identifies a resource.

```yaml
Type: String
Parameter Sets: ResourceWithObjectIdParameterSet, ResourceWithSignInNameParameterSet, ResourceWithSPNParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ParentResource
Specifies the parent resource in the hierarchy (of the resource specified using the *ResourceName* parameter).
This parameter should only be used in conjunction with the *ResourceGroupName*, *ResourceType*, and *ResourceName* parameters to construct a hierarchical scope in the form of a relative URI that identifies a resource.

```yaml
Type: String
Parameter Sets: ResourceWithObjectIdParameterSet, ResourceWithSignInNameParameterSet, ResourceWithSPNParameterSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RoleDefinitionId
Specifies the ID of the RBAC role that needs to be assigned to the principal.

```yaml
Type: Guid
Parameter Sets: RoleIdWithScopeAndObjectIdParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SignInName
Specifies the email address or the user principal name of the user.

```yaml
Type: String
Parameter Sets: ResourceWithSignInNameParameterSet, ResourceGroupWithSignInNameParameterSet, ScopeWithSignInNameParameterSet
Aliases: Email, UserPrincipalName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServicePrincipalName
Specifies the ServicePrincipalName of the Azure Active Directory application.

```yaml
Type: String
Parameter Sets: ResourceGroupWithSPNParameterSet, ResourceWithSPNParameterSet, ScopeWithSPNParameterSet
Aliases: SPN

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, resource, group, template, deployment

## RELATED LINKS

[Get-AzureRmRoleAssignment](./Get-AzureRmRoleAssignment.md)

[Remove-AzureRmRoleAssignment](./Remove-AzureRmRoleAssignment.md)

[Get-AzureRmRoleDefinition](./Get-AzureRmRoleDefinition.md)