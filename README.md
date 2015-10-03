# RTVE-API
Documentación (No Oficial) y ejemplos de como usar el API de RTVE

### Ejemplos


### Rutas

Todas las rutas ya incluyen un ejemplo valido en formato json para ilustrar el funcionamiento. 
Se recomienda utilizar *[Jsonviewer](http://jsonviewer.stack.hu/)* para poder visualizar los datos en formato Json más facilmente, por [ejemplo](http://jsonviewer.stack.hu/#http://www.rtve.es/api/directos/ahora.json).

**Directos**
- [http://www.rtve.es/api/tematicas](http://www.rtve.es/api/tematicas.json)
- [http://www.rtve.es/api/directos/{id}](http://www.rtve.es/api/directos/8831.json)
- [http://www.rtve.es/api/directos/proximos](http://www.rtve.es/api/directos/proximos.json)
- [http://www.rtve.es/api/directos/ahora](http://www.rtve.es/api/directos/ahora.json)
- [http://www.rtve.es/api/medios/{id}/directos/ahora](http://www.rtve.es/api/medios/748/directos/ahora.json)
- [http://www.rtve.es/api/medios/{id}/directos/en-vivo/ahora](http://www.rtve.es/api/medios/310/directos/en-vivo/ahora.json)
- [http://www.rtve.es/api/medios/{id}/directos/todos/ahora](http://www.rtve.es/api/medios/310/directos/todos/ahora.json)
- [http://www.rtve.es/api/medios/{id}/directos/proximos](http://www.rtve.es/api/medios/310/directos/proximos.json)
- [http://www.rtve.es/api/medios/{id}/directos/en-vivo/proximos](http://www.rtve.es/api/medios/310//directos/en-vivo/proximos.json)
- [http://www.rtve.es/api/medios/{id}/directos/todos/proximos](http://www.rtve.es/api/medios/310/directos/todos/proximos.json)
- [http://www.rtve.es/api/cadenas/{id}/directos/ahora](http://www.rtve.es/api/cadenas/310/directos/ahora.json)
- [http://www.rtve.es/api/cadenas/{id}/directos/proximos](http://www.rtve.es/api/cadenas/310/directos/proximos.json)


**Noticias**

- [http://www.rtve.es/api/noticias](http://www.rtve.es/api/noticias.json)
- [http://www.rtve.es/api/noticias/{id}](http://www.rtve.es/api/noticias/1230940.json)
- [http://www.rtve.es/api/noticias/ticker](http://www.rtve.es/api/noticias/ticker.json)
- [http://www.rtve.es/api/noticias/{id}/tematicas.json](http://www.rtve.es/api/noticias/1220540/tematicas.json)
- [http://www.rtve.es/api/noticias/{id}/multimedias/relacionados.json](http://www.rtve.es/api/noticias/1220540/multimedias/relacionados.json)
- [http://www.rtve.es/api/noticias/{id}/multimedias/totem.json](http://www.rtve.es/api/noticias/1220540/multimedias/totem.json)
- [http://www.rtve.es/api/noticias/{id}/multimedias/destacado.json](http://www.rtve.es/api/noticias/1220540/multimedias/destacado.json)
- [http://www.rtve.es/api/noticias/ticker/noticias](http://www.rtve.es/api/noticias/ticker/noticias.json)
- [http://www.rtve.es/api/noticias/ticker/deportes](http://www.rtve.es/api/noticias/ticker/deportes.json)
- [http://www.rtve.es/api/noticias/{id}/noticias/relacionados](http://www.rtve.es/api/noticias/1220540/noticias/relacionados.json)
- [http://www.rtve.es/api/noticias/{id}/noticias/especiales](http://www.rtve.es/api/noticias/1220540/noticias/especiales.json)
- [http://www.rtve.es/api/noticias/mas-vistas](http://www.rtve.es/api/noticias/mas-vistas.json)
- [http://www.rtve.es/api/noticias/mas-populares](http://www.rtve.es/api/noticias/mas-populares.json)
- [http://www.rtve.es/api/tematicas/{id}/noticias](http://www.rtve.es/api/tematicas/80550/noticias.json)
- [http://www.rtve.es/api/tematicas/{id}/noticias/mas-vistas](http://www.rtve.es/api/tematicas/80550/noticias/mas-vistas.json)
- [http://www.rtve.es/api/tematicas/{id}/noticias/mas-populares](http://www.rtve.es/api/tematicas/80550/noticias/mas-populares.json)


**Temáticas**

Algunos IDs y UIDs importantes

ID | UID | Descripción
------------ | ------------- | -------------
[814](http://www.rtve.es/api/tematicas/814.json) | [RT_TEMATI](http://www.rtve.es/api/tematicas.json?uid=RT_TEMATI) | Temática
[815](http://www.rtve.es/api/tematicas/815.json) | [TE_PORTAD](http://www.rtve.es/api/tematicas.json?uid=TE_PORTAD) | Categorías
[825](http://www.rtve.es/api/tematicas/825.json) | [TE_NOTICI](http://www.rtve.es/api/tematicas.json?uid=TE_NOTICI) | Notícias
[39190](http://www.rtve.es/api/tematicas/39190.json) | [TE_SESPE01](http://www.rtve.es/api/tematicas.json?uid=TE_SESPE01) | Especiales
[24570](http://www.rtve.es/api/tematicas/24570.json) | [TE_LOSCA01](http://www.rtve.es/api/tematicas.json?uid=TE_LOSCA01) | Los Oscar *(General)*

- [http://www.rtve.es/api/tematicas](http://www.rtve.es/api/tematicas.json)
- [http://www.rtve.es/api/tematicas/{id}](http://www.rtve.es/api/tematicas/80550.json)
- [http://www.rtve.es/api/temticas?uid={UID}](http://www.rtve.es/api/tematicas.json?uid=TE_SOSCA15)
- [http://www.rtve.es/api/tematicas/{id}/descendientes](http://www.rtve.es/api/tematicas/24570/descendientes.json)
- [http://www.rtve.es/api/tematicas/{id}/ancestros](http://www.rtve.es/api/tematicas/45510/ancestros.json)
- [http://www.rtve.es/api/tematicas/{id}/hijos](http://www.rtve.es/api/tematicas/24570/hijos.json)
- [http://www.rtve.es/api/tematicas/{id}/completas](http://www.rtve.es/api/tematicas/24570/completas.json)
- [http://www.rtve.es/api/videos/{id}/tematicas](http://www.rtve.es/api/videos/3013194/tematicas.json)
- *http://www.rtve.es/api/audios/{id}/tematicas*
- *http://www.rtve.es/api/imagenes/{id}/tematicas*
- *http://www.rtve.es/api/encuestas/{id}/tematicas*

**Vídeos**
**Audios**
**Multimedia**
**Blogs**

### Queries

**Format**
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

**Size**
Es posible definir la cantidad de datos que esperamos. Mínimo 1 - Máximo 60

```
http://api.rtve.es/api/tematicas.json?size=60
```

**Pages**
Es posible definir la pagina que esperamos. Por defecto se carga la primera página.
El número total de páginas esta incluido en la respuesta como *"totalPages"*

```
http://api.rtve.es/api/tematicas.json?page=100
```

**Pages**
Es posible definir la pagina que esperamos. Por defecto se carga la primera página.
El número total de páginas esta incluido en la respuesta como *"totalPages"*

```
http://api.rtve.es/api/tematicas.json?page=100
```


**Lang**
Es posible realizar la petición para ver el contenido en varios idiomas. Por defecto los resultados se muestran en español

- Español
```
http://api.rtve.es/api/videos.json?lang=es
```

- Catalán
```
http://api.rtve.es/api/videos.json?lang=ca
```


### Limitaciones Conocidas

**?size=** -> *Mínimo 1 - Máximo 60*
**?lang=** -> *"es"* para español y *"ca"* para catalán

### Información Adiccional
- [API RTVE en Wikibooks](https://es.wikibooks.org/wiki/API_Rtve)
