[← Volver al inicio](../index.md)

# 2. Proceso de instalación y configuración de VirtualBox
Para implementar la infraestructura de red virtualizada se utilizará VirtualBox, una plataforma de virtualización gratuita que permite ejecutar múltiples sistemas operativos simultáneamente. La instalación consistió en descargar el software desde la página oficial y ejecutar con configuraciones predeterminadas. Esto nos proporcionó la base para poder crear y gestionar nuestras máquinas virtuales de forma aislada y flexible.

Configuramos tres máquinas virtuales clave:
- Un router MikroTik como núcleo de la red
- Un servidor Ubuntu para alojar servicios
- Un cliente Linux para pruebas de conectividad

Todas se interconectan mediante una red en VirtualBox asignando recursos adecuados de RAM y almacenamiento según sus exigencias. Esto nos permitirá simular un entorno corporativo completo sin necesidad de hardware físico adicional, facilitando la experimentación y el aprendizaje en un ambiente controlado.

## Creación de las máquinas virtuales

### Router MikroTik:
- **ISO:** MikroTik Cloud Hosted Router (CHR)
- **CPU:** 1
- **RAM:** 1024 MB
- **Red:**
    - **Adaptador 1:**
        - Red NAT
    - **Adaptador 2:** 
        - Red Interna  
        - Intnet
    - **Adaptador 3:** 
        - Red Interna  
        - lan2

### Servidor Ubuntu Zentyal:
- **ISO:** Ubuntu Server Zentyal
- **CPU:** 2
- **RAM:** 5034 MB
- **Red:** 
    - **Adaptador 1:** 
        - Red Interna  
        - Intnet

### Cliente Linux 1:
- **ISO:** Linux Mint
- **CPU:** 2
- **RAM:** 2048 MB
- **Red:** 
    - **Adaptador 1:** 
        - Red Interna  
        - Intnet

## Cliente Linux 2
- **ISO:** Lubuntu
- **CPU** 1
- **RAM:** 1024 MB
- **Red:** 
    - **Adaptador 1:** 
        - Red Interna  
        - Intnet

