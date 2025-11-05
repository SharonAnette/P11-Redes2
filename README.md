# Práctica 11 — Protocolo DHCP

Este repositorio contiene el desarrollo de la **Práctica 11** de la materia **Aplicaciones para Comunicaciones en Red (6CV2)** de la **ESCOM - IPN**, centrada en la simulación del protocolo **DHCP (Dynamic Host Configuration Protocol)** en un entorno virtual de red con **GNS3**

---

## Objetivo
Simular el funcionamiento de un **servidor DHCP** utilizando un router Cisco 7200 en **GNS3**, el cual asigna automáticamente **direcciones IP** a dos computadoras virtuales conectadas a través de un switch, demostrando la asignación dinámica de parámetros de red.

---

## Funcionamiento
El protocolo **DHCP** permite asignar direcciones IP y configuraciones de red de forma automática a los dispositivos conectados.  
Durante la práctica, se configuró un **router Cisco** con los siguientes pasos:

1. Se habilitó el servicio **DHCP** en el router.  
2. Se definió un **pool de direcciones IP** con parámetros como máscara de subred, puerta de enlace y DNS.  
3. Se excluyó un rango de direcciones reservadas.  
4. Las computadoras virtuales se configuraron para solicitar una IP mediante el comando `dhcp`.  
5. Cada dispositivo obtuvo una IP válida del rango disponible, verificada con `show ip`.
