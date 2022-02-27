# Dockerized Gilded Rose en una VM de Microsoft Azure

### Pasos a seguir:

1. Crear la VM.
2. Conectarse a la VM (en este caso, por ssh)
3. Instalar la paquetería necesaria en la VM (no ha resultado ser necesario)
4. Instalar Git
5. Instalar Docker (https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-es)
6. Dockerizar GildedRose.

---

#### 1. Crear la VM

En Azure, existe la opción de alquilar máquinas virtuales, por lo tanto, según los pasos explicados en clase, esta es la máquina virtual que usaré para realizar el ejercicio (instalado el SO de Debian):

![](doc/1_Creación_VM.png)

---

#### 2. Conectarse a la VM

Me he conectado a la máquina virtual mediante SSH:

![](doc/2_Conexión_VM.png)

---

#### 3. Instalar la paquetería necesaria en la VM

---

#### 4. Instalar Git

Para instalar Git, he usado [apt-get install git]:

![](doc/4_Instalación_Git.png)

---

#### 5. Instalar Docker

He seguido los pasos indicados en esta página -> [Instalar Docker](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-es)

Resumidamente, he seguido los pasos al detalle, aún que he tenido que instalar **gnupg** porque si no, no podía verificar la llave según indican los pasos.

![](doc/5_Docker_Instalado.png)

---

#### 6. Dockerizar GildedRose

He clonado el repositorio de [dfleta](https://github.com/dfleta/docker-multistage-maven-java):

![](doc/6.0_Dockerizar_GildedRose.png)

Seguidamente, creado una imagen a partir del Dockerfile:

![](doc/6.1_Dockerizar_GildedRose.png)
![](doc/6.2_Dockerizar_GildedRose.png)

Finalmente, he creado y ejecutado un contenedor a partir de la imagen:

![](doc/6.3_Dockerizar_GildedRose.png)
![](doc/6.4_Dockerizar_GildedRose.png)
