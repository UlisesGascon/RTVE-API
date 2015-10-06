# /Imagenes

### Demo

- [Mostrando una imagen partiendo de una ID](demoid.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoid.html?id=3312498
```

- [Mostrando las imagenes más populares](demopopulares.html)
- [Mostrando las imagenes más vistas](demovistos.html)


### Ejemplos


### /imagenes - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/imagenes.json**

```javascript
var xmlHttp = new XMLHttpRequest()

xmlHttp.onreadystatechange = function() {
    var datos = {};
    if (xmlHttp.readyState === 4 && xmlHttp.status === 200) {
        datos = JSON.parse(xmlHttp.responseText);
        console.info(datos);
    } else if (xmlHttp.readyState === 4 && xmlHttp.status === 400) {
        datos = JSON.parse(xmlHttp.responseText);
        console.error("ERROR! 400 - Solicitud incorrecta!");         
    } else if (xmlHttp.readyState === 4 && xmlHttp.status === 404) {
        datos = JSON.parse(xmlHttp.responseText);
        console.error("ERROR! 404 - No encontrado!");
    }
};

xmlHttp.open("GET", "http://api.rtve.es/api/imagenes.json", true);
xmlHttp.send();
```

**Respuesta esperada**

- page (Object)
	- items (Array)
		- 0 (Object)
		- ...
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number



### /imagenes/{id} - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/imagenes/3311283.json**

```javascript
var xmlHttp = new XMLHttpRequest()

xmlHttp.onreadystatechange = function() {
    var datos = {};
    if (xmlHttp.readyState === 4 && xmlHttp.status === 200) {
        datos = JSON.parse(xmlHttp.responseText);
        console.info(datos);
    } else if (xmlHttp.readyState === 4 && xmlHttp.status === 400) {
        datos = JSON.parse(xmlHttp.responseText);
        console.error("ERROR! 400 - Solicitud incorrecta!");         
    } else if (xmlHttp.readyState === 4 && xmlHttp.status === 404) {
        datos = JSON.parse(xmlHttp.responseText);
        console.error("ERROR! 404 - No encontrado!");
    }
};

xmlHttp.open("GET", "http://api.rtve.es/api/imagenes/3311283.json", true);
xmlHttp.send();
```

**Respuesta esperada**

- page (Object)
	- items (Array)
		- 0 (Object)
			- uri: String
			- htmlUrl: String
			- htmlShortUrl: String
			- id: String
			- language: String
			- longTitle: String
			- shortTitle: null
			- mainCategoryRef: String
			- popularity: String
			- popHistoric: String
			- numVisits: String
			- publicationDate: String
			- expirationDate: null
			- modificationDate: String
			- pubState (Object)
				- code: String
				- description: String
			- breadCrumbRef: String
			- imageSEO: String
			- publicationDateTimestamp: Number
			- contentType: String
			- statistics (Object)
				- numComentarios: Number
				- numCompartidas: Number
			- alt: String
			- foot: String
			- shortDescription: String
			- description: String
			- otherTopicsRefs: String
			- qualities (Array)
				- 0 (Object)
					- identifier: Number
					- filePath: String
					- preset: String
					- filesize: Number
					- type: String
					- height: Number
					- width: Number
					- orientation: String
				- ...
			- qualitiesRef: String
			- mainTopic: String
			- topicsName (Array)
			- sourceReference: String
			- sign: String
			- title: String
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number