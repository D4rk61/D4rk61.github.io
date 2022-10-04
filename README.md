# Mi Portafolio 💀

![Imagen principal](https://www.redeszone.net/app/uploads-redeszone.net/2017/06/BlackArch-Linux-junio-2017-800x388.png)

<br>

---

## _Indice_

- [Conocimientos Actuales](#conocimientos-actuales)
- [Tecnologias Dominadas 📚](#tecnologias-dominadas-📚)
- [Certificaciones & logros]()
- [Repositorios]()
- [Conoceme 👀]()

<br>

<!-- En esta parte iran cosas que he ido aprendiendo, tanto como de manera independiente como por cursos, tambien logros o trabajos que quisiera alcanzar -->
## Conocimientos Actuales
<br>

Hola!, Actualmente soy un estudiante en la carrera de computacion, 4to de secundaria, amo la tecnologia esto me ha llevado a profundizar en varios temas de mi interes, tengo conocimientos bases sobre redes, protocolos un area donde me he logrado desarrolar es la ciberseguridad en el area ofensiva (atacante) tambien en sistemas linux (sistema actual arch linux) mi vision o lo que quiero lograr / conseguir es mi primer trabajo formal para comenzar a ganar experiencia, ya sea como ayudante de administrador de servidores o como desarrollador backend, esas areas me apasionan


## Tecnologias Dominadas 📚
### Algunas tecnologias donde tengo conocimientos
<br>


- [Terminal y linea de comandos](#terminal-y-linea-de-comandos)
    - Comandos Basicos sistemas unix
    - Editor vim (basico)
    - Administradores de paquetes (apt, yay, pacman)
    - alias
    - Servicios en el sistema

- Bash scripting
    - Variables
    - Operaciones basicas
    - Sustitucion de comandos
    - Solicitar informacion al usuario
    - Condicionales
    - Funciones
    - Descargas de internet

- Python (aprendiendo)
    - Variables

- Virtualizacion
    - Conceptos y bases 
    - Instalacion de visor nivel 2 en sistemas windows y algunas distribuciones linux
    - Exportar maquinas virtuales
- Hacking 
    - Escaneos de red
    - Conocimientos en la suite de aircrack-ng
    - Envenenamiento ARP
    - Uso de la herramienta nmap
    - Instlacion de sistema kali linux y blackarch

<br>
<br>
<br>


### Terminal y linea de comandos
Como bien explique arriba tengo algunos conocimientos sobre la terminal ya que un futuro desarrollador backend, se tendra que mover mayormente por ella.

#### Comandos Basicos
Tiempo atras estuve pensando en dar clases sobre linux basico, para poner aprueba mis conocimientos, aunque sean algo basicos aqui estaran algunos.
```bash
    mkdir carpeta1
    cd carpeta1

    ls 

    archivo1 archivo2 archivo3 archivo4 ...

    rm archivo1

    mv archivo2 archivo2_copia
```

Se moverme por la terminal, el crear, copiar eliminar y editar archivos es algo de todos los dias desde la terminal.
<br>

Otro conocimiento que va de la mano con el primer punto es el tener conocimiento de un editor de texto desde la terminal, para eso uso vim un editor complejo

``` bash
    vim archivo3

    echo "hola mundo"

```

<br>
Un administrador de paquetes para instalar software o servicios en diferentes distribuciones linux


**Debian / Ubunto & Ubuntu-server** 


``` bash
    sudo apt-get update
    sudo apt firefox
```

**Sistemas Arch**

``` bash
    sudo pacman -Syy
    sudo pacman -Syu
    yay -S firefox
```

Alias y Servicios 
Por un lado alias para creacion de nuestro propios comandos y la segunda para saber el estatus de nuestro sistema / servidor


``` bash
    sudo systemctl status tor.service
```


``` bash
    alias comando1="ls"
```
<br>

---
<br>


### Bash scripting
Este es un lenguaje de programacion el cual nos ayudara para automatizar muchas tareas dentro de un sistema linux

Aqui tratare de centrar mis pocos conocimientos en un pqueño programa
``` bash

#!/bin/bash
#===============================================================================
#
#          FILE:  programa2.sh
# 
#         USAGE:  ./programa2.sh 
# 
#   DESCRIPTION:  Programa para demostrar mis conocimientos. A pequeña escala
# 
#       OPTIONS:  ---
#  REQUIREMENTS:  ---
#          BUGS:  ---
#         NOTES:  ---
#        AUTHOR:  Jose - Blackshark (), reynosojose2005@gmail.com
#       COMPANY:  Evilcompany
#       VERSION:  1.0
#       CREATED:  03/10/22 02:44:43 CST
#      REVISION:  ---
#===============================================================================

# --=[ Este Programa consistira en pedir una clave para actualizar un servidor y acceder a demas registros ]=--

fail () {
  fecha=$(date)
  quien=$(whoami)
    echo -e "\n
    Contraseña incorrecta.. Se notificara que el usuario: $quien Intento ingresar al sistema en la fecha: $fecha"
    sleep 2
    exit
}
echo -e "\nNecesitas los permisos necesarios para ejecutar este script "

safe=""

read -s -p "Porfavor Escribe la contraseña: " safe
if [ $safe == root ]; then
  act () {
    sudo pacman -Syu
    sleep 1
    echo -e "\nEl siguiente comando nos marcara si el sistema esta actualizado por completo"
    echo -e "\n"
    sudo pacman -Syy
  }
  act3=""

  echo "Contraseña Correcta"
  sleep 2
  echo -e "\n"
  read -p "Desea actualizar el servidor [y/n] " act3
  if [ $act3 == "y" ]; then
    act
  else
    echo "No se actualizara el sistema"
  fi  

else
  fail
fi

```

<br>

<iframe width="600" height = "420"
src="https://www.youtube.com/embed/qKf2EwInKbA">
</iframe>

## Certificaciones & logros

## Repositorios

## Conoceme 👀
