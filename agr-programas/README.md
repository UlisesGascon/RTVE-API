# /Agr-programas

### Demo

- [Mostrando los audios de un agr-programas partiendo de una ID](demoaudios.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoaudios.html?id=42172
```

- [Mostrando los videos de un agr-programas partiendo de una ID](demovideos.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demovideos.html?id=42172
```

- [Mostrando los archivos multimedia de un agr-programas partiendo de una ID](demomultimedias.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demomultimedias.html?id=42172
```

- [Mostrando los programas de un agr-programas partiendo de una ID](demoprogramas.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoprogramas.html?id=42172
```

- [Mostrando lso detalles de un agr-programa partiendo de una ID](demoid.html)

Para utilizar otra id, solo necesitas pasarlo como parámetro en la url.

```
demoid.html?id=3312498
```

- [Mostrando los agr-programas más populares](demopopulares.html)
- [Mostrando los agr-programas más vistos](demovistos.html)


### Ejemplos


### /agr-programas - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/agr-programas.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/agr-programas.json", true);
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



### /agr-programas/{id} - Peticiones Ajax y respuestas esperadas

**Petición Ajax a http://api.rtve.es/api/agr-programas/1130.json**

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

xmlHttp.open("GET", "http://api.rtve.es/api/agr-programas/1130.json", true);
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
			- agrupador: null
			- name: String
			- title: null
			- url: null
			- programsRef: String
			- videosRef: String
			- audiosRef: String
			- multimediasRef: String
	- number: Number
	- size: Number
	- offset: Number
	- total: Number
	- totalPages: Number
	- numElements: Number