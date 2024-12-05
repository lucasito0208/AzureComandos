# Guía de Comandos Principales de Azure CLI en Bash

Este archivo contiene los comandos principales de la **Azure CLI** que puedes usar en Bash para gestionar recursos en Microsoft Azure. La **Azure CLI** es una herramienta de línea de comandos que facilita la administración de tus servicios y recursos en la nube de Azure.

---

## 1. Autenticación y Gestión de Subscripciones

### Iniciar sesión en Azure
Inicia sesión en tu cuenta de Azure:
```bash
az login

### Mostrar suscripciones
Lista de suscripciones disponibles:
```bash
az account list

### Establecer una subscripción activa
Establece una subscripción activa por su nombre o ID:
```bash
az account set --subscription "Nombre o ID de la suscripción"

---

## 2. Gestión de Recursos

### Crear un grupo de recursos
Crea un grupo de recursos en una ubicación específica:
```bash
az group create --name <nombre-del-grupo> --location <ubicación>

### Listar grupos de recursos
Lista todos los grupos de recursos en tu cuenta:
```bash
az group list

### Eliminar un grupo de recursos
Elimina un grupo de recursos:
```bash
az group delete --name <nombre-del-grupo>

---

## 3. Máquinas Virtuales (VM)

### Crear una máquina virtual
Crea una máquina virtual con un nombre y una imagen específica:
```bash
az vm create --resource-group <grupo-de-recursos> --name <nombre-vm> --image <imagen> --admin-username <usuario> --admin-password <contraseña>

### Listar máquinas virtuales
Lista todas las máquinas virtuales:
```bash
az vm list --output table

### Iniciar una máquina virtual
Inicia una máquina virtual:
```bash
az vm start --name <nombre-vm> --resource-group <grupo-de-recursos>

### Detener una máquina virtual
Detén una máquina virtual:
```bash
az vm stop --name <nombre-vm> --resource-group <grupo-de-recursos>

### Eliminar una máquina virtual
Elimina una máquina virtual:
```bash
az vm delete --name <nombre-vm> --resource-group <grupo-de-recursos> --yes

---




