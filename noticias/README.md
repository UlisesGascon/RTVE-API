# /Noticias

### Demo

- [Mostrando multimedia similar a la noticia partiendo de una ID](demosimilaresmultimedia.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demosimilaresmultimedia.html?id=1233541
```

- [Mostrando noticias similares partiendo de una ID](demosimilares.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demosimilares.html?id=1233541
```

- [Mostrando los detalles de una noticia partiendo de una ID](demoid.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoid.html?id=1233541
```

- [Mostrando las noticias más vistas](demovistas.html)
- [Mostrando las noticias más populares](demopopulares.html)


### Ejemplos


### /noticias - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/noticias.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/noticias.json", true);
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



### /noticias/{id} - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/noticias/1231780.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/noticias/1231780.json", true);
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
			- anteTitle: null
			- frontTitle: null
			- tabTitle: null
			- ticker (Object)
				- tickerSports: Boolean
				- tickerNews: Boolean
			- essentialInfo (Object)
				- info: null
				- photo: null
			- summary: String
			- frontSummary: null
			- text: String
			- refreshSeconds: Number
			- sign (Object)
				- ctvId: null
				- name: null
				- photo: null
				- firma: String
				- twitter: null
				- facebook: null
				- googlePlus: null
			- mainCategory: String
			- otherTopicsName (Array)
				- 0: String
				- ...
			- otherTopicsRef: String
			- newsRelatedRef: String
			- newsEspecialesRef: String
			- multimediaRelatedRef: String
			- multimediaTotemRef: String
			- multimediaDestacadoRef: String
			- links (Object)
				- galeriasRelacionadasRef: String
				- galeriasTotemRef: String
				- encuestaDestacadaRef: String
				- encuestasRelacionadasRef: String
				- encuestasTotemRef: String
				- comentariosRef: String
				- tagsRef: String
				- estadisticasRef: String
			- image: String
			- commentOptions: null
			- rightModule: null
			- title: String
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number