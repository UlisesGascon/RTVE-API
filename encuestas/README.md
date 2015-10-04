# /Encuestas

### Ejemplos


### /encuestas - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/encuestas.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/encuestas.json", true);
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



### /encuestas/{id} - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/encuestas/51931.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/encuestas/51931.json", true);
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
			- shortTitle: String
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
			- imageSEO: null
			- publicationDateTimestamp: Number
			- contentType: String
			- statistics (Object)
				- numComentarios: Number
				- numCompartidas: Number
			- description: String
			- question: String
			- imageUrl: null
			- image: null
			- commentOptions (Object)
				- code: String
				- description: String
			- links (Object)
				- topicsRef: String
				- optionsRef: String
				- pollsRef: String
				- comentariosRef: String
			- mainCategory: String
			- otherTopicsName [Array]
			- title: String
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number