# AzureComandos
Lista de comandos Azure en Bash 

**Desde Cloud Shell, ejecuta el siguiente comando az vm create para crear una máquina virtual Linux:**
```az vm create \
  --resource-group "<grupo de recurso>" \
  --name <nombre de la maquina virtual> \
  --public-ip-sku Standard \
  --image <imagen de la VM> \
  --admin-username <nombre de usuario> \
  --generate-ssh-keys  ´´´

### Para abreviar el resource-group asegurate de que estés utilizando el identificador del grupo de recursos de forma correcta. En Azure CLI, la forma más común de abreviar un recurso como un grupo de recursos o una máquina virtual es usando su nombre corto si ya tienes acceso a ese recurso en el contexto de tu suscripción y cuenta. Un ejemplo de abreviación es el siguiente código:

```resource_group="learn-e584da6e-a829-4673-bba9-86a34b07c5cb"
    az vm create \
      --resource-group "$resource_group" \
      --name my-vm \
      --public-ip-sku Standard \
      --image Ubuntu2204 \
      --admin-username azureuser \
      --generate-ssh-keys´´´
**La máquina virtual tarda unos instantes en aparecer. Ha asignado el nombre my-vm a la máquina virtual. Use este nombre para hacer referencia a la máquina virtual en los pasos posteriores.**



**Ejecuta el siguiente comando az vm extension set para configurar Nginx en la máquina virtual:**
