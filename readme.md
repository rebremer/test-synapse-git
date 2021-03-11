# Synapse notebooks to "get things done" as follows:

- **connect_private_storage_aad.ipynb**: Notebook that uses private link to connect to an external storage account and read data using Azure AD. Key in here is the creation of a custom ```CustomTokenCredential``` class that embeds the Azure AD token using the standard method ```mssparkutils.credentials.getToken("storage")``` that is already present in every Spark notebook in Synapse
