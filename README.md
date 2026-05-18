# New-Cibersecurity-Lab
# Montaje de Laboratorio Virtual / Virtual Cybersecurity Lab Setup 🛡️

Este repositorio contiene la documentación del **Proyecto 01**, enfocado en la configuración de un entorno virtual aislado para la práctica de ciberseguridad y el reconocimiento inicial de redes.

This repository contains the documentation for **Project 01**, focusing on setting up an isolated virtual environment for cybersecurity practice and initial network reconnaissance.

---

## 🇪🇸 Versión en Español

### 📝 Descripción del Proyecto
Configuración desde cero de un laboratorio virtual completo y aislado para practicar ciberseguridad utilizando **VirtualBox** y **Kali Linux**. El proyecto incluye un primer contacto práctico con el escaneo y reconocimiento de redes.

### 💻 Entorno y Arquitectura


| Componente | Detalle |
| :--- | :--- |
| **Hipervisor** | VirtualBox |
| **Máquina Atacante** | Kali Linux |
| **Modo de Red** | Host-only (`192.168.56.0/24`) |

### 🧠 Aprendizajes Clave
* **Virtualización:** Qué es y qué utilidad tiene para realizar pruebas seguras en ciberseguridad.
* **Direccionamiento IP:** Diferencias fundamentales entre IP pública e IP privada.
* **Red Host-only:** Por qué se utilizan redes aisladas para entornos de laboratorio.
* **Nmap:** Funcionamiento básico y qué información revela sobre los objetivos.

### 🚀 Pasos Realizados

#### 1. Instalación del Entorno
* Instalación de **VirtualBox** en el sistema operativo anfitrión (Windows).
* Descarga y despliegue de la máquina virtual de **Kali Linux**.
* Configuración de la tarjeta de red en modo **Host-only** para garantizar el aislamiento.

#### 2. Reconocimiento de Red
Ejecución de comandos en la terminal de Kali Linux para auditar el entorno local:
```bash
# Ver la IP asignada a Kali dentro de la red virtual
ip a

# Escanear todos los dispositivos activos en la subred
nmap 192.168.56.0/24
```

#### 3. Resultados del Escaneo
* **Gateway de VirtualBox:** `192.168.56.1`
* **Máquina Anfitrión (Windows):** `192.168.56.100`
* **Kali Linux (Atacante):** `192.168.56.102`

### 📚 Conceptos Clave
* **VirtualBox:** Software que permite crear ordenadores virtuales dentro de tu sistema operativo real.
* **Kali Linux:** Distribución de Linux orientada a ciberseguridad que incluye herramientas preinstaladas de pentesting.
* **Nmap:** Herramienta de auditoría de seguridad y escaneo de redes para descubrir hosts y puertos abiertos.
* **Red Host-only:** Red privada interna que no tiene salida a internet ni comunicación externa, ideal para laboratorios.
* **IP Privada:** Dirección de red no accesible desde internet, reservada para redes locales (rangos `192.168.x.x`, `10.x.x.x`, `172.16.x.x`).

---

## 🇺🇸 English Version

### 📝 Project Description
This project focuses on building a complete, isolated virtual laboratory from scratch using **VirtualBox** and **Kali Linux**. It serves as a foundational environment for practicing ethical hacking and includes an initial hands-on experience with network scanning.

### 💻 Environment & Architecture


| Component | Detail |
| :--- | :--- |
| **Hypervisor** | VirtualBox |
| **Attacker Machine** | Kali Linux |
| **Network Mode** | Host-only (`192.168.56.0/24`) |

### 🧠 Core Concepts Learned
* **Virtualization:** Purpose and benefits within cybersecurity testing.
* **IP Addressing:** Key differences between public and private IP addresses.
* **Host-only Network:** Why isolated networks are essential for lab safety.
* **Nmap:** Basic functionality and the data it reveals during a scan.

### 🚀 Steps Executed

#### 1. Environment Installation
* Installed **VirtualBox** on a Windows host machine.
* Downloaded and deployed the **Kali Linux** virtual machine image.
* Configured the network adapter to **Host-only** mode to ensure isolation.

#### 2. Network Reconnaissance
Executed the following commands within the Kali Linux terminal:
```bash
# Check the Kali Linux IP address inside the virtual network
ip a

# Scan all active devices within the local subnet
nmap 192.168.56.0/24
```

#### 3. Scan Results
* **VirtualBox Gateway:** `192.168.56.1`
* **Windows Host Machine:** `192.168.56.100`
* **Kali Linux (Attacker):** `192.168.56.102`

### 📚 Key Glossary
* **VirtualBox:** Software used to create and run isolated virtual computers within a physical host.
* **Kali Linux:** A Debian-derived Linux distribution tailored for digital forensics and penetration testing.
* **Nmap:** A powerful network mapper used for network discovery and vulnerability scanning.
* **Host-only Network:** A private network shared exclusively between the host and the VMs, blockaded from the internet.
* **Private IP:** Non-routable internet addresses reserved for internal networks (e.g., `192.168.x.x`, `10.x.x.x`, `172.16.x.x`).

---

## 🛠️ Herramientas y Enlaces / Tools & Links
* [VirtualBox Official Website](https://virtualbox.org)
* [Kali Linux Official Website](https://kali.org)
* [Nmap Official Website](https://nmap.org)
