# Amass

[https://github.com/owasp-amass/amass](https://github.com/owasp-amass/amass)


## Instalación 

[https://github.com/owasp-amass/amass/blob/master/doc/install.md](https://github.com/owasp-amass/amass/blob/master/doc/install.md)

```ruby
sudo apt-get install amass
```

![label text](imgs/01.png)

## Configurar las APIS

Video demostrativo

[https://www.youtube.com/watch?v=DbjVL-bqfl4&ab_channel=BePractical](https://www.youtube.com/watch?v=DbjVL-bqfl4&ab_channel=BePractical)

Ver las apis configuradas

```ruby
amass unum -list
```

![label text](imgs/02.png)

Para configurar este archivo, vamos a google y buscamos.\

[https://github.com/anthrax3/Amass-1/blob/master/examples/config.ini](https://github.com/anthrax3/Amass-1/blob/master/examples/config.ini)

```ruby
amass config.ini github
```

Copiamos el raw en el archivo **config.ini** en la siguiente ruta:\
Empezamos a configurar las APIs

```ruby
nvim ~/.config/amass/config.ini
```

Para ver todas las opciones de la herramienta para enumerar

```ruby
amass enum --help
```

Una vez configuradas las API podremos usar la tool.
* Parametro -o es para el output de los subdominios

```ruby
amass enum -d tinder.com -o subdomains_tinder.txt
```

![label text](imgs/04.png)
















