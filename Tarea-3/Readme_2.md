## Comandos Básicos de gcloud

compañeros    | 
------------- | 
Fernando      | 
Carlos        | 
Luis          |
Mike          |
Valente       |

- Comando para listar las SA existentes en un proyecto

Para listar todas las SA de un proyecto se utiliza el siguiente comando:
gcloud iam service-accounts list


URL: https://cloud.google.com/sdk/gcloud/reference/iam/service-accounts/list

====================================================================================================
# Para listar las direcciones existentes en un projecto de GCP usar:
## gcloud compute addresses list 

### NAME
gcloud compute addresses list - list addresses

### SYNOPSIS

gcloud compute addresses list [NAME …] [--regexp=REGEXP, -r REGEXP] [--global     | --regions=[REGION,…]] [--filter=EXPRESSION] [--limit=LIMIT] [--page-size=PAGE_SIZE] [--sort-by=[FIELD,…]] [--uri] [GCLOUD_WIDE_FLAG …]

### DESCRIPTION

gcloud compute addresses list lists summary information of addresses in a project. The --uri option can be used to display URIs instead. Users who want to see more data should use gcloud compute addresses describe.

By default, global addresses and addresses from all regions are listed. The results can be narrowed down by providing the --regions or --global flag.

### EXAMPLES

To list all addresses in a project in table form, run:

gcloud compute addresses list
To list the URIs of all addresses in a project, run:


gcloud compute addresses list --uri
To list all of the global addresses in a project, run:


gcloud compute addresses list --global
To list all of the addresses from the us-central1 region, run:


gcloud compute addresses list --filter=region:us-central1

### Fuente: https://cloud.google.com/sdk/gcloud/reference/compute/addresses/list
=========================================================================================
