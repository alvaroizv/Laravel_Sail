# Laravel_Sail
Proyecto de Laravel realizado desde Docker, utilizando Laravel Sail


# Índice



---

## 1.Requisitos Previos

Previamente deberemos tener Docker Desktop ejecutandose, WSL al usar Windows y una terminal de comandos, en mi caso CMD.

Una vez tenemos todo esto, comenzaremos por la creación de nuestro proyecto.

Antes que nada, tenemos que instalar una distribución a nuestro subsistema de Linux, si previamente no lo teníamos (como es mi caso). En Powershell 
ejecutamos el siguiente comando :

```bash
   wsl --install -d Ubuntu
```

Luego nos pedirá usuario y contraseña, y tendremos Ubuntu instalado :

![Ubuntu Installation](doc/1.Ubuntu.png)


## 2.Creación del Scaffolding

Para crear la estructura del proyecto deberemos entrar a la terminal de WSL y escribir el siguiente comando :

```bash
   curl -s "https://laravel.build/proyectoPiloto" | bash
```

Una vez ejecutado este comando nos aparecerá lo siguiente por consola:

![alt text](doc/2.Scaffolding.png)

Cuando ha finalizado, nos creará una carpeta con el proyecto ya iniciado, esperando a ser desplegado :

![alt text](doc/3.proyectoPiloto.png)

## 3.Configuración de Laravel Sail

Una vez creado nuestro proyecto, ejecutaremos los siguientes comandos para desplegar nuestro proyecto :

```bash
   cd proyectoPiloto
   ./vendor/bin/sail up -d
```