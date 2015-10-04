# RTVE-API
Documentación (No Oficial) y ejemplos de como usar el API de RTVE

### Ejemplos


### Rutas

Todas las rutas ya incluyen un ejemplo valido en formato json para ilustrar el funcionamiento. 
Se recomienda utilizar *[Jsonviewer](http://jsonviewer.stack.hu/)* para poder visualizar los datos en formato Json más facilmente, por [ejemplo](http://jsonviewer.stack.hu/#http://www.rtve.es/api/directos/ahora.json).


**Encuestas**

*[Ejmeplos y detalles](encuestas/README.md)*

- [/encuestas](http://www.rtve.es/api/encuestas.json)
- [/encuestas/{id}](http://www.rtve.es/api/encuestas/51931.json)
- */encuestas/{id}/breadcrumb - ERROR 400*
- [/encuestas/{id}/tematicas](http://www.rtve.es/api/encuestas/51931/tematicas.json)
- [/encuestas/{id}/opciones](http://www.rtve.es/api/encuestas/51931/opciones.json)
- [/encuestas/{id}/relacionadas](http://www.rtve.es/api/encuestas/51931/relacionadas.json)
- [/encuestas/{id}/comentarios](http://www.rtve.es/api/encuestas/51931/comentarios.json)


**VideoGalerias**

*[Ejmeplos y detalles](videogalerias/README.md)*

- [/videogalerias](http://www.rtve.es/api/videogalerias.json)
- [/videogalerias/{id}](http://www.rtve.es/api/videogalerias/147975.json)
- */videogalerias/{id}/breadcrumb - ERROR 400*
- [/videogalerias/{id}/multimedias](http://www.rtve.es/api/videogalerias/147975/multimedias.json)
- [/videogalerias/{id}/relacionadas](http://www.rtve.es/api/videogalerias/147975/relacionadas.json)
- [/videogalerias/{id}/links](http://www.rtve.es/api/videogalerias/147975/links.json)
- [/videogalerias/{id}/estadisticas](http://www.rtve.es/api/videogalerias/147975/estadisticas.json)
- */videogalerias/{id}/tematicas - ERROR 400*


**Agr-programas**

*[Ejmeplos y detalles](agr-programas/README.md)*

- [/agr-programas](http://www.rtve.es/api/agr-programas.json)
- [/agr-programas/{id}](http://www.rtve.es/api/agr-programas/1130.json)
- [/agr-programas/{id}/programas](http://www.rtve.es/api/agr-programas/1130/programas.json)
- [/agr-programas/{id}/videos](http://www.rtve.es/api/agr-programas/1130/videos.json)
- [/agr-programas/{id}/audios](http://www.rtve.es/api/agr-programas/1130/audios.json)
- [/agr-programas/{id}/multimedias](http://www.rtve.es/api/agr-programas/1130/multimedias.json)


**Multimedias**

*[Ejmeplos y detalles](multimedias/README.md)*

- [/multimedias](http://www.rtve.es/api/multimedias.json)
- [/multimedias/{id}](http://www.rtve.es/api/multimedias/3309959.json)


**Noticias**

*[Ejmeplos y detalles](noticias/README.md)*

- [/noticias](http://www.rtve.es/api/noticias.json)
- [/noticias/{id}](http://www.rtve.es/api/noticias/1231600.json)
- [/noticias/{id}/tematicas](http://www.rtve.es/api/noticias/1231600/tematicas.json)
- [/noticias/{id}/noticias/relacionados](http://www.rtve.es/api/noticias/1231600/noticias/relacionados.json)
- [/noticias/{id}/noticias/especiales](http://www.rtve.es/api/noticias/1231600/noticias/especiales.json)
- [/noticias/{id}/multimedias/relacionados](http://www.rtve.es/api/noticias/1231600/multimedias/relacionados.json)
- [/noticias/{id}/multimedias/totem](http://www.rtve.es/api/noticias/1231600/multimedias/totem.json)
- [/noticias/{id}/multimedias/destacado](http://www.rtve.es/api/noticias/1231600/multimedias/destacado.json)


**Cadenas**

*[Ejmeplos y detalles](cadenas/README.md)*

- [/cadenas](http://www.rtve.es/api/cadenas.json)
- [/cadenas/{id}](http://www.rtve.es/api/cadenas/745.json)
- [/cadenas/{id}/programas](http://www.rtve.es/api/cadenas/745/programas.json)
- [/cadenas/{id}/videos](http://www.rtve.es/api/cadenas/745/videos.json)
- [/cadenas/{id}/audios](http://www.rtve.es/api/cadenas/745/audios.json)
- [/cadenas/{id}/multimedias](http://www.rtve.es/api/cadenas/745/multimedias.json)
- [/cadenas/{id}/directos/ahora](http://www.rtve.es/api/cadenas/745/directos/ahora.json)
- [/cadenas/{id}/directos/en-vivo/ahora](http://www.rtve.es/api/cadenas/745/directos/en-vivo/ahora.json)
- [/cadenas/{id}/directos/todos/ahora](http://www.rtve.es/api/cadenas/745/directos/todos/ahora.json)
- [/cadenas/{id}/directos/proximos](http://www.rtve.es/api/cadenas/745/directos/proximos.json)
- [/cadenas/{id}/directos/en-vivo/proximos](http://www.rtve.es/api/cadenas/745/directos/en-vivo/proximos.json)
- [/cadenas/{id}/directos/todos/proximos](http://www.rtve.es/api/cadenas/745/directos/todos/proximos.json)
- [/cadenas/{id}/agrupadores](http://www.rtve.es/api/cadenas/745/agrupadores.json)
- [/cadenas/{id}/videos/mas-vistos](http://www.rtve.es/api/cadenas/745/videos/mas-vistos.json)
- [/cadenas/{id}/audios/mas-vistos](http://www.rtve.es/api/cadenas/745/audios/mas-vistos.json)
- [/cadenas/{id}/multimedias/mas-vistos](http://www.rtve.es/api/cadenas/745/multimedias/mas-vistos.json)
- [/cadenas/{id}/videos/mas-populares](http://www.rtve.es/api/cadenas/745/videos/mas-populares.json)
- [/cadenas/{id}/audios/mas-populares](http://www.rtve.es/api/cadenas/745/audios/mas-populares.json)
- [/cadenas/{id}/multimedias/mas-populares](http://www.rtve.es/api/cadenas/745/multimedias/mas-populares.json)


**Agrupadores**

*[Ejmeplos y detalles](agrupadores/README.md)*

- [/agrupadores](http://www.rtve.es/api/agrupadores.json)
- [/agrupadores/{id}](http://www.rtve.es/api/agrupadores/42273.json)
- [/agrupadores/{id}/hijos](http://www.rtve.es/api/agrupadores/42273/hijos.json)
- [/agrupadores/{id}/programas](http://www.rtve.es/api/agrupadores/42273/programas.json)
- [/agrupadores/{id}/videos](http://www.rtve.es/api/agrupadores/42273/videos.json)
- [/agrupadores/{id}/audios](http://www.rtve.es/api/agrupadores/42273/audios.json)
- [/agrupadores/{id}/multimedias](http://www.rtve.es/api/agrupadores/42273/multimedias.json)


**Temáticas**

*[Ejmeplos y detalles](tematicas/README.md)*

Algunos IDs y UIDs importantes

ID | UID | Descripción
------------ | ------------- | -------------
[814](http://www.rtve.es/api/tematicas/814.json) | [RT_TEMATI](http://www.rtve.es/api/tematicas.json?uid=RT_TEMATI) | Temática
[815](http://www.rtve.es/api/tematicas/815.json) | [TE_PORTAD](http://www.rtve.es/api/tematicas.json?uid=TE_PORTAD) | Categorías
[825](http://www.rtve.es/api/tematicas/825.json) | [TE_NOTICI](http://www.rtve.es/api/tematicas.json?uid=TE_NOTICI) | Notícias
[39190](http://www.rtve.es/api/tematicas/39190.json) | [TE_SESPE01](http://www.rtve.es/api/tematicas.json?uid=TE_SESPE01) | Especiales
[24570](http://www.rtve.es/api/tematicas/24570.json) | [TE_LOSCA01](http://www.rtve.es/api/tematicas.json?uid=TE_LOSCA01) | Los Oscar *(General)*


- [/tematicas](http://www.rtve.es/api/tematicas.json)
- [/tematicas/{id}](http://www.rtve.es/api/tematicas/830.json)
- [/tematicas/{uid}](http://www.rtve.es/api/tematicas.json?uid=RT_TEMATI)
- [/tematicas/{id}/hijos](http://www.rtve.es/api/tematicas/814/hijos.json)
- [/tematicas/{id}/descendientes](http://www.rtve.es/api/tematicas/814/descendientes.json)
- [/tematicas/{id}/ancestros](http://www.rtve.es/api/tematicas/814/ancestros.json)
- [/tematicas/{id}/videos](http://www.rtve.es/api/tematicas/830/videos.json)
- [/tematicas/{id}/audios](http://www.rtve.es/api/tematicas/830/audios.json)
- [/tematicas/{id}/multimedias](http://www.rtve.es/api/tematicas/830/multimedias.json)
- [/tematicas/{id}/multimedias/mas-vistos](http://www.rtve.es/api/tematicas/830/multimedias/mas-vistos.json)
- [/tematicas/{id}/videos/mas-vistos](http://www.rtve.es/api/tematicas/830/videos/mas-vistos.json)
- [/tematicas/{id}/audios/mas-vistos](http://www.rtve.es/api/tematicas/830/audios/mas-vistos.json)
- [/tematicas/{id}/multimedias/mas-populares](http://www.rtve.es/api/tematicas/830/multimedias/mas-populares.json)
- [/tematicas/{id}/videos/mas-populares](http://www.rtve.es/api/tematicas/830/videos/mas-populares.json)
- [/tematicas/{id}/audios/mas-populares](http://www.rtve.es/api/tematicas/830/audios/mas-populares.json)
- [/tematicas/{id}/noticias](http://www.rtve.es/api/tematicas/830/noticias.json)
- */tematicas/{id}/noticias/ticker - ERROR 400*
- */tematicas/{id}/noticias/ticker/noticias - ERROR 400*
- */tematicas/{id}/noticias/ticker/deportes - ERROR 400*
- [/tematicas/{id}/noticias/mas-vistas](http://www.rtve.es/api/tematicas/830/noticias/mas-vistas.json)
- [/tematicas/{id}/noticias/mas-populares](http://www.rtve.es/api/tematicas/830/noticias/mas-populares.json)
- [/tematicas/{id}/publicidad/roba](http://www.rtve.es/api/tematicas/830/publicidad/roba.json)


**Blogs**

*[Ejmeplos y detalles](blogs/README.md)*

- [/blogs](http://www.rtve.es/api/blogs.json)
- [/blogs/{id}](http://www.rtve.es/api/blogs/5330.json)
- */blogs/{id}/breadcrumb - ERROR 400*


**Programas**

*[Ejmeplos y detalles](programas/README.md)*

- [/programas](http://www.rtve.es/api/programas.json)
- [/programas/{id}](http://www.rtve.es/api/programas/63010.json)
- [/programas/{id}/secciones](http://www.rtve.es/api/programas/63010/secciones.json)
- [/programas/{id}/temporadas](http://www.rtve.es/api/programas/63010/temporadas.json)
- [/programas/{id}/agrupadores](http://www.rtve.es/api/programas/63010/agrupadores.json)
- [/programas/{id}/videos](http://www.rtve.es/api/programas/63010/videos.json)
- [/programas/{id}/audios](http://www.rtve.es/api/programas/63010/audios.json)
- [/programas/{id}/multimedias](http://www.rtve.es/api/programas/63010/multimedias.json)
- [/programas/{id}/relacionados](http://www.rtve.es/api/programas/63010/relacionados.json)
- [/programas/{id}/otras-cadenas](http://www.rtve.es/api/programas/63010/otras-cadenas.json)
- [/programas/{id}/info-infantil](http://www.rtve.es/api/programas/63010/info-infantil.json)
- [/programas/{id}/relacionados/relacionados-por-idioma](http://www.rtve.es/api/programas/63010/relacionados/relacionados-por-idioma.json)



**Videos**

*[Ejmeplos y detalles](videos/README.md)*

- [/videos/{id}/tematicas](http://www.rtve.es/api/videos/3309918/tematicas.json)
- [/videos/{id}/calidades](http://www.rtve.es/api/videos/3309918/calidades.json)
- [/videos/{id}/cuepoints](http://www.rtve.es/api/videos/3309918/cuepoints.json)
- [/videos/{id}/config/video](http://www.rtve.es/api/videos/3309918/config/video.json)
- [/api/videos/{id}/transcripcion](http://www.rtve.es/api/videos/3309918/transcripcion.json)
- [/videos/{id}/temporadas](http://www.rtve.es/api/videos/3309918/temporadas.json)
- [/videos/{id}/relacionados](http://www.rtve.es/api/videos/3309918/relacionados.json)
- [/videos/{id}/relacionados/manuales](http://www.rtve.es/api/videos/3309918/relacionados/manuales.json)
- [/videos/{id}/publicidad](http://www.rtve.es/api/videos/3309918/publicidad.json)
- [/videos/{id}/comentarios](http://www.rtve.es/api/videos/3309918/comentarios.json)
- [/videos/{id}/relacionados/relacionados-por-idioma](http://www.rtve.es/api/videos/3309918/relacionados/relacionados-por-idioma.json)
- [/videos/{id}/estadisticas](http://www.rtve.es/api/videos/3309918/estadisticas.json)
- [/videos/{id}/subtitulos](http://www.rtve.es/api/videos/3309918/subtitulos.json)


**Medios**

*[Ejmeplos y detalles](medios/README.md)*

- [/medios/{id}](http://www.rtve.es/api/medios/310.json)
- [/medios/{id}/cadenas](http://www.rtve.es/api/medios/310/cadenas.json)
- [/medios/{id}/programas](http://www.rtve.es/api/medios/310/programas.json)
- */medios/{id}/videos - ERROR 400*
- */medios/{id}/audios - ERROR 400*
- */medios/{id}/multimedias - ERROR 400*
- [/medios/{id}/directos/en-vivo/ahora](http://www.rtve.es/api/medios/310/directos/en-vivo/ahora.json)
- [/medios/{id}/directos/todos/ahora](http://www.rtve.es/api/medios/310/directos/todos/ahora.json)
- [/medios/{id}/directos/proximos](http://www.rtve.es/api/medios/310/directos/proximos.json)
- [/medios/{id}/directos/en-vivo/proximos](http://www.rtve.es/api/medios/310/directos/en-vivo/proximos.json)
- [/medios/{id}/directos/todos/proximos](http://www.rtve.es/api/medios/310/directos/todos/proximos.json)
- [/medios/{id}/agrupadores](http://www.rtve.es/api/medios/310/agrupadores.json)
- */medios/{id}/videos/mas-vistos - ERROR 400*
- */medios/{id}/audios/mas-vistos - ERROR 400*
- */medios/{id}/multimedias/mas-vistos - ERROR 400*
- */medios/{id}/videos/mas-populares - ERROR 400*
- */medios/{id}/audios/mas-populares - ERROR 400*
- */medios/{id}/multimedias/mas-populares - ERROR 400*


### Queries

- **Format**
Es posible solicitar los datos en diversos formatos, esta extensión debe colocarse al final de la URL.

	- [Json](https://www.wikiwand.com/es/JSON)
	```
	http://api.rtve.es/api/tematicas.json
	```

	- [Xml](https://www.wikiwand.com/es/Extensible_Markup_Language)
	```
	http://api.rtve.es/api/tematicas.xml
	```

	- [RSS](https://www.wikiwand.com/es/RSS)
	```
	http://api.rtve.es/api/tematicas.rss
	```

	- Txt, *Es una version del xml*
	```
	http://api.rtve.es/api/tematicas.txt
	```

- **Size**
Es posible definir la cantidad de datos que esperamos. Mínimo 1 - Máximo 60

```
http://api.rtve.es/api/tematicas.json?size=60
```

- **Pages**
Es posible definir la pagina que esperamos. Por defecto se carga la primera página.
El número total de páginas esta incluido en la respuesta como *"totalPages"*

```
http://api.rtve.es/api/tematicas.json?page=100
```

- **Lang**
Es posible realizar la petición para ver el contenido en varios idiomas. Por defecto los resultados se muestran en español

	- Español
	```
	http://api.rtve.es/api/videos.json?lang=es
	```

	- Catalán
	```
	http://api.rtve.es/api/videos.json?lang=ca
	```


- **startWithLetter**
Es posible realizar un filtro de los programas, limtiando los resutlados a la letra deseada 
```
http://www.rtve.es/api/programas.json?startWithLetter=z
```


- **from**
Podemos realizar un filtro usando una fecha. El formato es *ddMMyyyyHHmmss*

```
http://www.rtve.es/api/programas.json?from=02102015001015
```

- **lastDays**
Podemos realizar un filtro contando los dias hacia atras.
```
http://www.rtve.es/api/programas.json?lastDays=2
```

### Limitaciones Conocidas

- **?size=** -> *Mínimo 1 - Máximo 60*
- **?lang=** -> *"es"* para español y *"ca"* para catalán
- **Videos** -> *Es necesario un Token y un Provedor, la url por defecto de todos los videos es "http://ztnr.rtve.es/ztnr/res/_PROVIDER_/video/med/_TOKEN_"*


### Información Adiccional
- [API RTVE en Wikibooks](https://es.wikibooks.org/wiki/API_Rtve)
