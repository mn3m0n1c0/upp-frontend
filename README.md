![Vue.js](https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white)


<div align="center"><a href="https://upp.lol/"><img src="https://github.com/cromeoli/upp-backend-laravel/assets/92324278/fa030cf2-b533-41af-8162-063937f98c94"></a></div>

## Update 2024: Actualmente fuera de producción debido a costes.

## Concepto
<div align="center">
  <img width="360" height="800" alt="V0 5 - Feed" src="https://github.com/user-attachments/assets/b9e03d20-249b-4171-9263-d302867b2d55" />
  <img width="360" height="801" alt="Mis Circulos" src="https://github.com/user-attachments/assets/c21a8aed-a870-48a7-acee-82586bee536b" />
  <img width="360" height="719" alt="Encuentra círculos" src="https://github.com/user-attachments/assets/a0051d93-f457-4bf7-a354-5bdf26cb6c71" />
  <img width="360" height="719" alt="Perfil" src="https://github.com/user-attachments/assets/d1fbb80f-3331-4e50-8028-f0b1e62266b9" />
  <img width="360" height="800" alt="Top" src="https://github.com/user-attachments/assets/35e7765a-aadf-45c9-a19e-c7c57f19d81f" />
  <img width="360" height="800" alt="wall" src="https://github.com/user-attachments/assets/bad5ef64-474c-446f-8a6a-337cc0b9a08d" />
</div>

<br>


Upp es una "red social basada en el contenido". No trata de capturar la atención de usuarios infinitamente, si no más bien ser una herramienta para compartir y almacenar ideas, momentos o _memes_, y en base a su evaluación, conservarlos o no.

Upp tendría usuarios, círculos y muros ( en el momento del desarrollo llamados _walls_). Cada usuario podría pertenecer a distintos círculos, públicos o privados, donde subiría contenido como texto, imágenes o vídeos no demasiado largos. Cada contenido debía recibir "Up" o "Down" al explorarlo. 

La vuelta de tuerca consistía en que cada _x_ tiempo, los posts con más "_Ups_", irían ascendiendo en el "Top", y los primeros lugares se guardarían para siempre en el muro de ese círculo, una especie de _"Salón de la fama"_. 


## Instalación
> [!IMPORTANT]  
> Para que la aplicación funcione, será necesario que tanto el **backend** como el **frontend** de la aplicación estén desplegados. 
> 
> Puedes acceder al backend aquí:
> ### [Upp Backend](https://github.com/cromeoli/upp-backend-laravel)
> 

Para instalar el frontend tan solo es necesario seguir los siguientes pasos:
1. Clonar mediante git u otro sistema de control de versiones el proyecto desde la siguiente URL: https://github.com/cromeoli/pwa-tests.git
2. Una vez clonado el proyecto, debemos ubicarnos en el directorio donde lo hemos clonado y entrar a la carpeta raíz del proyecto. Una vez dentro ejecutamos el siguiente comando:  

```
npm install
```

3. Con el anterior comando deberíamos de haber instalado las dependencias para nuestro proyecto. A continuación para lanzar el servidor de desarrollo en nuestra máquina usaremos el siguiente comando:

```
npm run dev -- --host
```

Habiendo seguido estos pasos debería ser posible ver acceder al proyecto en localhost:3000 (o 3001/3002… dependiendo de si están ocupados se intentará levantar el servidor en cualquiera de los puertos posteriores al 3000 que estén disponibles).

#### Nota
Es importante saber que en el archivo /src/environments/environment.ts se encuentran 2 variables importantes: API e IMAGE. Habrá 4 variables, 2 API y 2 IMAGE, pero una de cada una debería estar comentada. Este archivo establece la ruta a la que las peticiones se van a hacer, al servidor de nuestra maquina local (localhost) o al servidor en railway desplegado.
