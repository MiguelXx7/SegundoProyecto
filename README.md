# Proyecto de Monitoreo de Contenedores y Máquinas Virtuales

Este proyecto tiene como objetivo comparar el comportamiento de **máquinas virtuales** (Arch, Manjaro, Rocky) y **contenedores Docker** (Fedora, Alpine, Debian, Garuda) en un entorno de red híbrido. Utilizando herramientas de análisis como `htop`, `tcpdump`, `nmap` y plataformas de monitoreo como **Prometheus** y **Grafana**, se evaluaron aspectos clave como el uso de recursos, servicios en ejecución y tráfico de red.

El contenedor personalizado **Fedora Central** fue diseñado como nodo maestro para ejecutar escaneos, consultas de red y capturas de tráfico hacia todos los nodos. Además, se documentó todo el proceso y se expusieron resultados mediante dashboards interactivos.

---

## 🧱 Arquitectura del Proyecto

![Arquitectura de red del sistema](imagenes/arquitectura.png)

- Red Docker: `192.168.200.0/24`  
- Red VMs (bridge): `192.168.100.0/24`  
- Fedora Central: nodo de análisis y monitoreo  
- Conectividad cruzada validada entre contenedores y VMs  

---

## 🧪 Tecnologías y Herramientas

- 🔧 `htop`, `ps aux`, `tcpdump`, `nmap`, `netstat`, `ping`, `iftop`, `nethogs`
- 📦 Docker, QEMU/KVM, Virt-Manager
- 📊 Prometheus + Grafana para métricas en tiempo real
- 🐧 Sistemas operativos: Arch, Manjaro, Rocky, Alpine, Garuda, Debian, Fedora

---

## 📊 Resultados Clave

- Se logró comunicación entre todos los sistemas virtuales y contenerizados.
- Se recolectaron métricas de CPU y red, visualizadas con Grafana.
- Fedora Central ejecutó con éxito comandos de monitoreo a cada nodo.
- Zabbix fue intentado pero no implementado por errores de base de datos.

---

## 📁 Repositorio y Publicaciones

- 📦 Imagen Docker Fedora Central: [Docker Hub](https://hub.docker.com/r/tu_usuario/fedora_central)
- 📁 Repositorio con documentación y evidencias: [GitHub](https://github.com/tu_usuario/proyecto-monitor-vm-vs-docker)

---

## 👥 Autores

- Miguel Ángel Jiménez Morales  
- Dikersson Alexis Cañon Vanegas
