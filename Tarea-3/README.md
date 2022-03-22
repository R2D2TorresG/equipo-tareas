![GitHub Light](https://github.com/github-light.png#gh-dark-mode-only)

### Comandos Básicos de gcloud

compañeros    | 
------------- | 
Fernando      | 
Carlos        | 
Luis          |
Mike          |
Valente       |
Jorge         |
Daniela       |

==========================================
## LISTAR COMPUTER ENGINE

Google Cloud CLI te permite administrar los recursos de Compute Engine mediante el grupo de comandos  --gcloud compute. gcloud compute  --es una alternativa al uso de la API de Compute Engine.

La CLI de gcloud forma parte de Google Cloud CLI y es una herramienta de línea de comandos unificada que incluye funciones como el autocompletado de declaraciones, la actualización in situ y la ayuda de la línea de comandos, formatos de salida legibles y procesables, además de integración con Google Cloud CLI.

- Antes de comenzar
Si deseas ejecutar gcloud compute en un símbolo del sistema, instala, actualiza e inicializa Google Cloud CLI.
Si no tienes un símbolo del sistema disponible, intenta usar gcloud compute en Cloud Shell. Cloud Shell se instala, actualiza e inicializa de manera automática con Google Cloud CLI más reciente.
Propiedades predeterminadas
Cuando creas una instancia de máquina virtual, Compute Engine configura una VM con las propiedades predeterminadas del servidor de metadatos. Para verificar las propiedades predeterminadas de tu VM, ejecuta el siguiente comando:

gcloud compute project-info describe --project PROJECT_ID

Reemplaza PROJECT_ID con el ID del proyecto.

### URL
https://cloud.google.com/compute/docs/gcloud-compute?hl=es-419

==========================================

# Para listar las Service Accounts existentes en un proyecto de GCP:

Para listar todas las SA de un proyecto se utiliza el siguiente comando:
gcloud iam service-accounts list [--filter=EXPRESSION] [--limit=LIMIT] [--sort-by=[FIELD,…]] [--uri] [GCLOUD_WIDE_FLAG …]

### Banderas adicionales:

--filter=EXPRESSION
Bandera que permite filtrar las SA que seran listadas.

--limit=LIMIT
Permite limitar el número de items que se van a listar. EL default es ilimitado.

--sort-by=[FIELD,…]
Listar por campos claves (separados por comas). El default es ascendente.

--uri
Se listan las URIs de los recursos en lugar de la salida default. 

URL: https://cloud.google.com/sdk/gcloud/reference/iam/service-accounts/list

====================================================================================================
# Para listar las direcciones existentes en un projecto de GCP usar:
## gcloud compute addresses list 

### NAME:
gcloud compute addresses list - list addresses

### SYNOPSIS:

gcloud compute addresses list [NAME …] [--regexp=REGEXP, -r REGEXP] [--global     | --regions=[REGION,…]] [--filter=EXPRESSION] [--limit=LIMIT] [--page-size=PAGE_SIZE] [--sort-by=[FIELD,…]] [--uri] [GCLOUD_WIDE_FLAG …]

### DESCRIPTION:

gcloud compute addresses list lists summary information of addresses in a project. The --uri option can be used to display URIs instead. Users who want to see more data should use gcloud compute addresses describe.

By default, global addresses and addresses from all regions are listed. The results can be narrowed down by providing the --regions or --global flag.

### EXAMPLES:

To list all addresses in a project in table form, run:

gcloud compute addresses list
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
To list the URIs of all addresses in a project, run:

gcloud compute addresses list --uri
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
To list all of the global addresses in a project, run:

gcloud compute addresses list --global
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
To list all of the addresses from the us-central1 region, run:

gcloud compute addresses list --filter=region:us-central1
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
### Fuente: https://cloud.google.com/sdk/gcloud/reference/compute/addresses/list
=========================================================================================


## Enlistando buckets

### lineas de comando

Para completar esta guía con una utilidad de línea de comandos, debe tener los permisos de IAM adecuados. Si no creó el proyecto al que desea acceder, es posible que necesite que el propietario del proyecto le otorgue un rol que contenga los permisos necesarios.

Para obtener una lista de los permisos necesarios para acciones específicas, consulte Permisos de IAM para comandos de gsutil .

Para obtener una lista de roles relevantes, consulte Roles de [Cloud Storage](https://cloud.google.com/storage/docs/access-control/iam-roles/) . Como alternativa, puede crear un rol personalizado que tenga permisos específicos y limitados.

## GCLOUD
gcloud alpha storage ls

## Ejemplo dentro del proyecto

![List-bucket](https://user-images.githubusercontent.com/97456443/158726353-7221cc9e-37fb-4d8b-9316-656cd73d22ae.PNG)


## Comandos Extras

### Inhabilita mensajes
Algunos comandos de la CLI de gcloud son interactivos y solicita a los usuarios la confirmación de una operación o una solicitud adicional para un comando ingresado.

En la mayoría de los casos, esto no es conveniente cuando se ejecutan comandos en una secuencia de comandos o cualquier otra automatización. Puedes inhabilitar los mensajes desdegcloud mediante los comandos de la CLIdisable_prompts en tu configuración aTrue o mediante la función--quiet o-q marca. La mayoría de los comandos interactivos tienen valores predeterminados cuando se requiere una entrada o una confirmación adicional. Si se inhabilitan los mensajes, se usan estos valores predeterminados.

### Por ejemplo:
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
gcloud debug targets list --quiet
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -