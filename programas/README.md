# /Programas

### Ejemplos


### /programas - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/programas.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/programas.json", true);
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


### /programas/{id} - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/programas/92590.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/programas/92590.json", true);
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
			- ctvId: Number
			- uid: String
			- name: String
			- permalink: String
			- language: String
			- longTitle: String
			- shortTitle: String
			- description: String
			- longDescription: String
			- showMan: String
			- director: String
			- contact: null
			- emission: String
			- publicationDate: String
			- expirationDate: null
			- orden: Number
			- thumbnail: String
			- logo: String
			- imgBackground: String
			- imgPoster: String
			- imgPortada: String
			- outOfEmission: Boolean
			- channel (Object)
				- uri: String
				- htmlUrl: String
				- htmlShortUrl: String
				- id: String
				- medioRef: String
				- uid: String
				- title: String
				- permalink: String
				- programsRef: String
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
			- fanBoxID: null
			- ageRangeUid: null
			- ageRange: null
			- recommendAgesForChilds (Array)
			- seccionesRef: String
			- temporadasRef: String
			- agrupadoresRef: String
			- videosRef: String
			- audiosRef: String
			- multimediasRef: String
			- relacionadosRef: String
			- otherChannelsRef: String
			- childrenInfoRef: String
			- filtro: null
			- webRtve: null
			- webOficial: null
			- relatedByLangRef: String
			- publicationDateTimestamp: Number
			- contentType: String
			- imageSEO: String
			- imgPinta: String
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number