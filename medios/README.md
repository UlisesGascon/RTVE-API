# /Medios

### Demo

- [Mostrando los audios de un medio partiendo de una ID](demoaudios.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoaudios.html?id=414
```

- [Mostrando los videos de un medio partiendo de una ID](demovideos.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demovideos.html?id=414
```

- [Mostrando los archivos multimedia de un medio partiendo de una ID](demomultimedias.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demomultimedias.html?id=414
```

- [Mostrando los programas de un medio partiendo de una ID](demoprogramas.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoprogramas.html?id=414
```

- [Mostrando los detalles de un medio partiendo de una ID](demoid.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoid.html?id=414
```

- [Mostrando los archivos multimedia más populares del medio](demopopulares.html)
- [Mostrando los archivos multimedia más vistos del medi](demovistos.html)



### Ejemplos


### /medios - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/medios.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/medios.json", true);
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



### /medios/{id} - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/medios/851.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/medios/851.json", true);
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
			- cadenasRef: String
			- uid: String
			- title: String
			- permalink: String
			- fanBoxID: null
			- programasRef: String
			- videosRef: String
			- audiosRef: String
			- multimediasRef: String
			- directosAhoraRef: String
			- directosEnvivoAhoraRef: String
			- directosTodosAhoraRef: String
			- directosProximosRef: String
			- directosEnvivoProximosRef: String
			- directosTodosProximosRef: String
			- agrupadoresRef: String
			- videosVistosRef: String
			- audiosVistosRef: String
			- multimediasVistosRef: String
			- videosPopularesRef: String
			- audiosPopularesRef: String
			- multimediasPopularesRef: String
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number