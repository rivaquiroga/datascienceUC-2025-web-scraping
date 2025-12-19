# Web scraping con Python

En esta clase del [Diplomado en Ciencia de Datos UC](https://datascience.uc.cl/) aprenderemos a implementar la técnica de extracción de datos conocida como _web scraping_ usando la librería Beautiful Soup. 

## Preparación

Todas las demostraciones durante la sesión se harán usando un script de Python en [Positron](https://positron.posit.co/), ya que nos va a permitir compartir el código que escribimos _en vivo_ a través de un enlace. Si prefieres trabajar en un notebook, ya sea de forma local o en Google Colab, no hay problema. 

Para realizar las actividades planificadas necesitarás las librerías `request`, `beautifulsoup4` y `pandas`. Se pueden instalar desde [PyPI](https://pypi.org/) con `pip`. No olvides agregar un signo de exclamación al inicio de cada línea si es que estás en un notebook:

```
pip install beautifulsoup4
pip install requests
pip install pandas
pip install lxml
```

Hacia el final de la sesión haremos un demo del trabajo con sitios web dinámicos. Para ese ejemplo instalaremos algunas librerías adicionales. 


## Atajos de teclado útiles

Los siguientes atajos de teclado serán útiles al explorar las páginas web que _escrapearemos_.

| Acción | Windows / Linux | Mac |
|---|---|---|
| Ver el código fuente de una página | ctrl +  u | command + u|
| Abrir el panel de desarrollo | F12<br/>ctrl + shift + i | F12<br/>option + command +i |
| Abrir el panel de desarrollo con la opción de selección activada | ctrl + shift + c | option/ctrl + command + c |


## Enlaces ejemplos

A lo largo de la sesión revisaremos algunos sitios web a modo de ejemplo o para discutir algunas ideas. Los compartiremos por el chat de Zoom y quedarán acá también como referencia.

:link: [Sitio web estático](https://datascience.uc.cl/que-es-ciencia-de-datos)

:link: [Sitio web dinámico](https://www.camara.cl/transparencia/asesoriasexternasgral.aspx)

:link: [Condiciones de uso](https://www.amazon.com/-/es/gp/help/customer/display.html?nodeId=508088&ref_=footer_cou) 

:link: [Licenciamiento y uso del contenido 1](https://www.biobiochile.cl/)

:link: [Licenciamiento y uso del contenido 2](https://prensa.presidencia.cl/)

:link: [robots.txt 1](https://wikipedia.org/)

:link: [robots.txt 2](https://www.oas.org/)

## Actividades

Durante la clase realizaremos una serie de actividades para poner en práctica lo aprendido. Iremos escribiendo el código "en vivo", por lo que el contenido de los archivos con código se irá actualizando a medida que escribamos en ellos. 

### Ejercicio 1: extraer texto

:link: [Página web]()

:page_facing_up: [Código escrito en clases](https://www.dropbox.com/scl/fi/6e2mwni4mzxtl6asgjalx/ejercicio-1_extraer-texto.py?rlkey=jb8mar821cl064mllosj0q3ya&dl=0)


### Ejercicio 2: extraer tablas

:link: [Página web 1](https://www.enap.cl/informacion-comercial/tabla-de-precios-de-paridad) | [Página web 2](https://es.wikipedia.org/wiki/Anexo:%C3%81lbumes_musicales_m%C3%A1s_vendidos)

:page_facing_up: [Código escrito en clases](https://www.dropbox.com/scl/fi/giusljufp9c2z4risdcki/ejercicio-2_extraer-tablas.py?rlkey=m3mgifkbmwd6l715n5bmn0lmc&dl=0)

### Ejercicio 3: extraer enlaces y descargar archivos

:link: [Página web](https://es.wikipedia.org/wiki/Computadora)

:page_facing_up: [Código escrito en clases](https://www.dropbox.com/scl/fi/7l70xqfyuij18xrkj9ysn/ejercicio-3_descargar-archivos.py?rlkey=iemx2bge7gwm8iq35io21iin7&dl=0)


### Ejercicio 4: demo selenium

:link: [Página web](https://www.memoriachilena.gob.cl)

:page_facing_up: [Código escrito en clases](https://www.dropbox.com/scl/fi/qhwgye24wckube1ktqffz/ejercicio-4_demo-selenium.py?rlkey=fa6d0ahhqq5466kgth254lk1e&dl=0)


## Recursos adicionales

### Documentación librerías utilizadas
- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Selenium](https://www.selenium.dev/documentation/)

### Para profundizar
Para quienes tengan interés en escalar, la sugerencia es explorar [Scrapy](https://www.scrapy.org/), un framework que permite extraer datos de forma estructurada y automatizada.
También les sugiero explorar qué son las [GitHub Actions](https://docs.github.com/es/actions), que nos permiten programar la ejecución de scripts de extracción de datos desde su cuenta de GitHub. 

#### En R

Para quienes trabajan en R, el paquete [rvest](https://rvest.tidyverse.org/) nos permite hacer web scraping en sitios web estáticos usando R. [Este tutorial](https://programminghistorian.org/es/lecciones/introduccion-al-web-scraping-usando-r) cubre lo que vimos en el primer ejemplo (extracción de texto). 
Existe también un paquete que se llama [RSelenium](https://docs.ropensci.org/RSelenium/) que permite trabajar con sitios web dinámicos, pero solo funciona con la versión 2.0 de Selenium. 
En la edición 2023 este diplomado consideraba dos sesiones de web scraping con R. El código que escribimos en ese taller está disponible [en este repositorio](https://github.com/rivaquiroga/taller-web-scraping-r-2023). Es posible que algunos ejemplos no funcionen porque las páginas web utilizadas como ejemplo han cambiado. 
