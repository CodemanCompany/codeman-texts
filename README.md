# Codeman Text

El siguiente documento contiene los estándares de textos que se deben utilizar en cada uno de los siguientes contextos:

## Dialogs

Los siguientes textos son referentes a las diálogos que deben aparecer en un Módulo CRUD, Formulario de Contacto etc.

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

Los siguientes textos son referentes al proceso de **Login** y **Logout**. Recuerda que el **Login** no debe tener un diálogo en caso de acceder correctamente (Únicamente la redirección).

#### Error

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Datos de acceso incorrectos, por favor verifica la información proporcionada.",
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

