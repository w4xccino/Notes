
# The most useful commands for me
- `cd` para moverse entre carpetas
- `chmod` cambia los permisos de archivos `-R` para que sea recursivo.
- `mount` ,`umount`,`remount` para montar y desmontar unidades
- `blkid` para ver las unidades  montadas. 
- `ls` para ver archivos `-la` para archivos escondidos.
- `top` para mostrar procesos.
- `flatpak` es un gestor de paquetes multi-distribucion.
- `mv` para mover archivos.
- `cp` copiar archivos
- `rmdir` elimina carpetas
- `rm -rf` comando de eliminacion
- `pwd` muestra la ubicacion actual
- `wget <url>` descargar archivos. 
- `screen` instancias separadas de terminal 
- `find . -name <name>` Buscar en la carpeta actual por nombre
	- `service <process_name> status` ver si un proceso está siendo ejecutado
	- `ps aux | grep <process_name>` ver si un proceso está siendo ejecutado
- `which` para obtener la locacion de otro comando 
- `du -h` . ver peso de la carpeta actal.
# Locaciones importantes
- `/etc/fstab` es un archivo para modificar las particiones y discos.
- `/boot/grub/grub.conf` archivo para modificar el grub.
- `/etc/apt/sources.list.d/` carpeta para repositorios


## PATH
### PATH TEMPORAL
- `echo $PATH` Ver al path
- `export PATH="$PATH:<location>"` Agregar al path
### PATH PERMATENTE
Editar cualquiera de estos dos archivos con los comandos de arriba:
- `source ~/.bashrc`
- `source ~/.profile`
## shortcuts
- `shift` + `CAPS LOCK` cambiar el layout del teclado. Muy util


# GIT
- `git config credential.helper store`Guardar credenciales de github
- `git reset`
- `git checkout`
- `git revert` 
### Resolving conflicts
We only have 3 options
1. `git commit`We could commit our changes. The problem is we'll just overriding our local changes if we do that.
2. `git reset --hard HEAD` This is good one but we all just we do is bring back our changes locally to the previous commit.
3. `git stash` Basically this does is it will take our all changes and stashing(hide) apart for a moment.

# Alacritty
`alacritty-themes` configura los colorcitos del alacritty

# PULSEAUDIO

Avoid the sound card be inactive
3

I've been struggling with the same problem & found no solution on the web (in hindsight I was using incorrect / too vague search terms). But I finally figured it out so here it is, hoping this helps others.

Edit `/etc/pulse/default.pa` and comment the following line:

`load-module module-suspend-on-idle`
which becomes:

`# load-module module-suspend-on-idle`
Then restart the sound server.
`pulseaudio -k`




