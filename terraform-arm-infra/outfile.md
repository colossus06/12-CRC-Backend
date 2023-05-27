

       _               _              
   ___| |__   ___  ___| | _______   __
  / __| '_ \ / _ \/ __| |/ / _ \ \ / /
 | (__| | | |  __/ (__|   < (_) \ V / 
  \___|_| |_|\___|\___|_|\_\___/ \_/  
                                      
By bridgecrew.io | version: 2.3.251 
Update available 2.3.251 -> 2.3.259
Run pip3 install -U checkov to update 


terraform scan results:

Passed checks: 12, Failed checks: 0, Skipped checks: 18

Check: CKV_AZURE_3: "Ensure that 'enable_https_traffic_only' is enabled"
	PASSED for resource: azurerm_storage_account.st
	File: /main.tf:21-39
Check: CKV_AZURE_44: "Ensure Storage Account is using the latest version of TLS encryption"
	PASSED for resource: azurerm_storage_account.st
	File: /main.tf:21-39
	Guide: https://docs.bridgecrew.io/docs/bc_azr_storage_2
Check: CKV_AZURE_36: "Ensure 'Trusted Microsoft Services' is enabled for Storage Account access"
	PASSED for resource: azurerm_storage_account.st
	File: /main.tf:21-39
	Guide: https://docs.bridgecrew.io/docs/enable-trusted-microsoft-services-for-storage-account-access
Check: CKV_AZURE_3: "Ensure that 'enable_https_traffic_only' is enabled"
	PASSED for resource: azurerm_storage_account.st2
	File: /main.tf:40-60
Check: CKV_AZURE_44: "Ensure Storage Account is using the latest version of TLS encryption"
	PASSED for resource: azurerm_storage_account.st2
	File: /main.tf:40-60
	Guide: https://docs.bridgecrew.io/docs/bc_azr_storage_2
Check: CKV_AZURE_36: "Ensure 'Trusted Microsoft Services' is enabled for Storage Account access"
	PASSED for resource: azurerm_storage_account.st2
	File: /main.tf:40-60
	Guide: https://docs.bridgecrew.io/docs/enable-trusted-microsoft-services-for-storage-account-access
Check: CKV_AZURE_43: "Ensure Storage Accounts adhere to the naming rules"
	PASSED for resource: azurerm_storage_account.st2
	File: /main.tf:40-60
	Guide: https://docs.bridgecrew.io/docs/ensure-storage-accounts-adhere-to-the-naming-rules
Check: CKV_AZURE_132: "Ensure cosmosdb does not allow privileged escalation by restricting management plane changes"
	PASSED for resource: azurerm_cosmosdb_account.cosmos
	File: /main.tf:70-103
	Guide: https://docs.bridgecrew.io/docs/bc_azr_storage_4
Check: CKV_AZURE_101: "Ensure that Azure Cosmos DB disables public network access"
	PASSED for resource: azurerm_cosmosdb_account.cosmos
	File: /main.tf:70-103
	Guide: https://docs.bridgecrew.io/docs/ensure-that-azure-cosmos-db-disables-public-network-access
Check: CKV_AZURE_99: "Ensure Cosmos DB accounts have restricted access"
	PASSED for resource: azurerm_cosmosdb_account.cosmos
	File: /main.tf:70-103
	Guide: https://docs.bridgecrew.io/docs/ensure-cosmos-db-accounts-have-restricted-access
Check: CKV_AZURE_140: "Ensure that Local Authentication is disabled on CosmosDB"
	PASSED for resource: azurerm_cosmosdb_account.cosmos
	File: /main.tf:70-103
	Guide: https://docs.bridgecrew.io/docs/ensure-azure-cosmosdb-has-local-authentication-disabled
Check: CKV_AZURE_211: "Ensure App Service plan suitable for production use"
	PASSED for resource: azurerm_service_plan.asp
	File: /main.tf:105-112
Check: CKV_AZURE_59: "Ensure that Storage accounts disallow public access"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
	Guide: https://docs.bridgecrew.io/docs/ensure-that-storage-accounts-disallow-public-access
Check: CKV_AZURE_33: "Ensure Storage logging is enabled for Queue service for read, write and delete requests"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
	Guide: https://docs.bridgecrew.io/docs/enable-requests-on-storage-logging-for-queue-service
Check: CKV_AZURE_190: "Ensure that Storage blobs restrict public access"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
Check: CKV_AZURE_206: "Ensure that Storage Accounts use replication"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
Check: CKV_AZURE_59: "Ensure that Storage accounts disallow public access"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
	Guide: https://docs.bridgecrew.io/docs/ensure-that-storage-accounts-disallow-public-access
Check: CKV_AZURE_33: "Ensure Storage logging is enabled for Queue service for read, write and delete requests"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
	Guide: https://docs.bridgecrew.io/docs/enable-requests-on-storage-logging-for-queue-service
Check: CKV_AZURE_190: "Ensure that Storage blobs restrict public access"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
Check: CKV_AZURE_206: "Ensure that Storage Accounts use replication"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
Check: CKV_AZURE_100: "Ensure that Cosmos DB accounts have customer-managed keys to encrypt data at rest"
	SKIPPED for resource: azurerm_cosmosdb_account.cosmos
	Suppress comment: No comment provided
	File: /main.tf:70-103
	Guide: https://docs.bridgecrew.io/docs/ensure-that-cosmos-db-accounts-have-customer-managed-keys-to-encrypt-data-at-rest
Check: CKV_AZURE_212: "Ensure App Service has a minimum number of instances for failover"
	SKIPPED for resource: azurerm_service_plan.asp
	Suppress comment: No comment provided
	File: /main.tf:105-112
Check: CKV2_AZURE_18: "Ensure that Storage Accounts use customer-managed key for encryption"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
	Guide: https://docs.bridgecrew.io/docs/ensure-that-storage-accounts-use-customer-managed-key-for-encryption
Check: CKV2_AZURE_18: "Ensure that Storage Accounts use customer-managed key for encryption"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
	Guide: https://docs.bridgecrew.io/docs/ensure-that-storage-accounts-use-customer-managed-key-for-encryption
Check: CKV2_AZURE_33: "Ensure storage account is configured with private endpoint"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
Check: CKV2_AZURE_33: "Ensure storage account is configured with private endpoint"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
Check: CKV2_AZURE_1: "Ensure storage for critical data are encrypted with Customer Managed Key"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
	Guide: https://docs.bridgecrew.io/docs/ensure-storage-for-critical-data-are-encrypted-with-customer-managed-key
Check: CKV2_AZURE_1: "Ensure storage for critical data are encrypted with Customer Managed Key"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
	Guide: https://docs.bridgecrew.io/docs/ensure-storage-for-critical-data-are-encrypted-with-customer-managed-key
Check: CKV2_AZURE_38: "Ensure soft-delete is enabled on Azure storage account"
	SKIPPED for resource: azurerm_storage_account.st
	Suppress comment: No comment provided
	File: /main.tf:21-39
Check: CKV2_AZURE_38: "Ensure soft-delete is enabled on Azure storage account"
	SKIPPED for resource: azurerm_storage_account.st2
	Suppress comment: No comment provided
	File: /main.tf:40-60
arm scan results:

Passed checks: 0, Failed checks: 7, Skipped checks: 0

Check: CKV_AZURE_132: "Ensure cosmosdb does not allow privileged escalation by restricting management plane changes"
	FAILED for resource: Microsoft.DocumentDB/databaseAccounts.cosmos-cloud
	File: /json/cosmos.json:12-73
	Guide: https://docs.bridgecrew.io/docs/bc_azr_storage_4

		Code lines for this resource are too many. Please use IDE of your choice to review the file.
Check: CKV_AZURE_18: "Ensure that 'HTTP Version' is the latest if used to run the web app"
	FAILED for resource: Microsoft.Web/sites.func-topcugcrc
	File: /json/function.json:16-70
	Guide: https://docs.bridgecrew.io/docs/bc_azr_networking_8

		Code lines for this resource are too many. Please use IDE of your choice to review the file.
Check: CKV_AZURE_17: "Ensure the web app has 'Client Certificates (Incoming client certificates)' set"
	FAILED for resource: Microsoft.Web/sites.func-topcugcrc
	File: /json/function.json:16-70
	Guide: https://docs.bridgecrew.io/docs/bc_azr_networking_7

		Code lines for this resource are too many. Please use IDE of your choice to review the file.
Check: CKV_AZURE_14: "Ensure web app redirects all HTTP traffic to HTTPS in Azure App Service"
	FAILED for resource: Microsoft.Web/sites.func-topcugcrc
	File: /json/function.json:16-70
	Guide: https://docs.bridgecrew.io/docs/bc_azr_networking_5

		Code lines for this resource are too many. Please use IDE of your choice to review the file.
Check: CKV_AZURE_15: "Ensure web app is using the latest version of TLS encryption"
	FAILED for resource: Microsoft.Web/sites.func-topcugcrc
	File: /json/function.json:16-70
	Guide: https://docs.bridgecrew.io/docs/bc_azr_networking_6

		Code lines for this resource are too many. Please use IDE of your choice to review the file.
Check: CKV_AZURE_16: "Ensure that Register with Azure Active Directory is enabled on App Service"
	FAILED for resource: Microsoft.Web/sites.func-topcugcrc
	File: /json/function.json:16-70
	Guide: https://docs.bridgecrew.io/docs/bc_azr_iam_1

		Code lines for this resource are too many. Please use IDE of your choice to review the file.
Check: CKV_AZURE_13: "Ensure App Service Authentication is set on Azure App Service"
	FAILED for resource: Microsoft.Web/sites/config.[concat(parameters('sites_func_topcugcrc_name'), '/web')]
	File: /json/function.json:105-195
	Guide: https://docs.bridgecrew.io/docs/bc_azr_general_2

		Code lines for this resource are too many. Please use IDE of your choice to review the file.

