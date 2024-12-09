# Terraform-Packer-CloudInit: Automatización de VMs en Proxmox

[![Terraform](https://img.shields.io/badge/Terraform-v1.x-blue)](https://www.terraform.io/)
[![Packer](https://img.shields.io/badge/Packer-v1.x-green)](https://www.packer.io/)
[![Proxmox](https://img.shields.io/badge/Proxmox-VE-orange)](https://www.proxmox.com/)

Este proyecto implementa un flujo automatizado para crear y configurar máquinas virtuales (VMs) listas para usar en **Proxmox VE**, utilizando herramientas como **Terraform**, **Packer** y **Cloud-Init**. El enfoque está en la infraestructura como código (IaC), optimizando la creación y despliegue de entornos consistentes y reproducibles.

---

## Características

- **Imagen Base con Packer:** Construcción de imágenes personalizadas preconfiguradas con herramientas necesarias.
- **Configuración Dinámica con Cloud-Init:** Configuración automática de red, usuarios y claves SSH al iniciar la VM.
- **Orquestación con Terraform:** Creación de VMs en Proxmox de manera declarativa.
- **Modularidad:** Estructura limpia y escalable para reutilización en múltiples entornos.
- **Compatibilidad:** Soporte para imágenes en formato `qcow2` y otras opciones de Proxmox.

---

## Requisitos Previos

1. **Proxmox VE** con acceso SSH habilitado.
2. **Terraform** y **Packer** instalados:
   - [Terraform](https://www.terraform.io/downloads.html)
   - [Packer](https://www.packer.io/downloads)
3. Acceso a un repositorio remoto de imágenes (opcional para almacenamiento centralizado de plantillas).
4. Sistema operativo anfitrión con soporte para herramientas de automatización (Linux recomendado).
