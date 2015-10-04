# /Tematicas

### Ejemplos


### /tematicas - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/tematicas .json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/tematicas.json", true);
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



### /tematicas/{id} - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/tematicas/814.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/tematicas/814.json", true);
xmlHttp.send();
```

**Respuesta esperada**

- page (Object)
	- items (Array)
		- 0 (Object)
			- uri: String
			- id: String
			- uid: String
			- title: String
			- parentRef: String
			- childrenRef: String
			- descendantsRef: String
			- ancestrosRef: String
			- textoEN: null
			- permalink: String
			- pathUids: null
			- pathNames: null
			- videosRef: String
			- audiosRef: String
			- multimediasRef: String
			- multimediasVistosRef: String
			- videosVistosRef: String
			- audiosVistosRef: String
			- multimediasPopularesRef: String
			- videosPopularesRef: String
			- audiosPopularesRef: String
			- noticiasRef: String
			- noticiasTickerRef: String
			- noticiasTickerNoticiasRef: String
			- noticiasTickerDeportesRef: String
			- noticiasVistasRef: String
			- noticiasPopularesRef: String
			- publicidadRef: String
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number