# Azure

Adresse du site static hebergé chez azure: https://csb10032000ecb5f443.z6.web.core.windows.net/

J'ai utilisé Azure CLI.
Voici les commandes utilisées:

az storage blob service-properties update --account-name csb10032000ecb5f443 --static-website --404-document error.html --index-document index.html

az storage blob upload-batch -s C:\Cloud -d '$web' --account-name csb10032000ecb5f443

az storage account show -n csb10032000ecb5f443 -g cloud-shell-storage-westeurope --query "primaryEndpoints.web" --output tsv
