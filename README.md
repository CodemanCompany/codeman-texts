# Codeman Text

El siguiente documento contine los estándares de textos que se deben usar en los siguientes contextos:

## Dialogs

Los siguientes dialogos son referentes a las alertas que deben aparecer en un CRUD.

#### Error

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Por el momento no se puede realizar la operación, intente de nueva más tarde.",
	"title": "Atención",
	"type": "error",
} );
```

#### Loading

```javascript
Swal.fire( {
	"allowOutsideClick": false,
	"text": "Espere un momento por favor.",
	"title": "Realizando operación",
} )
Swal.showLoading();
```

#### Required

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Completa todos los campos requeridos.",
	"title": "Atención",
	"type": "info",
} );
```

#### Success

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Operación realizada con éxito.",
	"title": "Éxito",
	"type": "success",
} );
```

## Authentication

Los siguientes dialogos son referentes al proceso de Login y Logout.

#### Error

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Datos de acceso incorrectos, por favor verifica la información.",
	"title": "Atención",
	"type": "error",
} );
```

#### Loading

```javascript
Swal.fire( {
	"allowOutsideClick": false,
	"text": "Espere un momento por favor.",
	"title": "Verificando datos de acceso",
} );
Swal.showLoading();
```


## Payment

