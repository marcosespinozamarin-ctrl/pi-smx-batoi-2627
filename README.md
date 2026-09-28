# pi-smx-batoi-26-27
Este es el repositorio de ejemplo del proyecto de PI de SMX del curso 2026/2027

# # Sistema de Monitoratge de Xarxa Local

# Descripció del Projecte

NetMonitor és una eina informàtica investiga per a analitzar el tràfic de xarxa en temps real, detectar dispositius connectats i generar alertes de seguretat en entorns de feina o domèstics.

# Objectius

* Automatitzar l'escaneig de ports i serveis actius en la xarxa local.
* Identificar amb operacions en temps real qualsevol dispositiu no autoritzat.
* Generar informes periòdics i enviar alertes automatitzades als administradors.

# Tecnologies Utilitzades

* Python 3.10+
* Bash / Shell Scripting
* Wireshark
* GitHub

# Equips i Dispositius

| Dispositiu | Tipus / Rol | Adreça IP / Interfície | Estat |
| Server-Srv01 | Servidor Principal | 192.168.1.10 | Actiu |
| Router-GW01 | Gateway / Router | 192.168.1.1 | Actiu |
| Switch-Core | Switch Gestionable | 192.168.1.2 | Actiu |
| Workstation-Admin | Equip d'Administració | 192.168.1.50 | Apagat |

# Enllaços i Referències

* Visita la [documentació oficial de Python](https://docs.python.org/3/) per a més informació sobre les llibreries utilitzades.

[Esquema de la topologia de xarxa](https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/network/network.png)

# Comando de Linux

Executa `sudo nmap -sP 192.168.1.0/24` per a escanejar la xarxa i trobar tots els equips actius.

# Bloque de Codigo Bash

```bash
#!/bin/bash
# Script de inici i verificació de la xarxa

echo "Iniciant el servei de monitoratge..."
sudo systemctl start netmonitor.service
sudo systemctl status netmonitor.service
```
