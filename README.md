# Codeman Text

El siguiente documento contiene los estándares de textos que se deben utilizar en cada uno de los siguientes contextos:

## Dialogs

Los siguientes textos son referentes a las diálogos que deben aparecer en un Módulo CRUD, Formulario de Contacto etc.

###### Error

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Por el momento no se puede realizar la operación, intente de nuevo más tarde.",
	"title": "Atención",
	"type": "error",
} );
```

###### Loading

```javascript
Swal.fire( {
	"allowOutsideClick": false,
	"text": "Espere un momento por favor.",
	"title": "Realizando operación",
} )
Swal.showLoading();

// Close dialog
Swal.close();
```

###### Required

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Completa todos los campos requeridos.",
	"title": "Atención",
	"type": "info",
} );
```

###### Success

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Operación realizada con éxito.",
	"title": "Éxito",
	"type": "success",
} );
```

###### Question

```html
<h3>¿Realmente deseas eliminar el siguiente elemento?</h3>
<p>Advertencia, está acción no se puede deshacer.</p>
```


## Authentication

Los siguientes textos son referentes al proceso de **Login** y **Logout**. Recuerda que el **Login** no debe tener un diálogo en caso de acceder correctamente (Únicamente la redirección).

###### Error

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Datos de acceso incorrectos, por favor verifica la información proporcionada.",
	"title": "Atención",
	"type": "error",
} );
```

###### Loading

```javascript
Swal.fire( {
	"allowOutsideClick": false,
	"text": "Espere un momento por favor.",
	"title": "Verificando datos de acceso",
} );
Swal.showLoading();

// Close dialog
Swal.close();
```

###### Logout

Se recomienda que al "cerrar sesión" se haga una redirección inmedia al "Inicio". Pero también se proporciona un diálogo en caso de ser necesario.

```javascript
Swal.fire( {
	"cancelButtonText": "Cancelar",
	"confirmButtonText": "Aceptar",
	"reverseButtons": true,
	"showCancelButton": true,
	"text": "Nos vemos pronto.",
	"title": "¿Realmente deseas salir?",
	"type": "warning",
} );
```

## Payment

###### Loading

```javascript
Swal.fire( {
	"allowOutsideClick": false,
	"text": "Espere un momento por favor.",
	"title": "Realizando operación",
} )
Swal.showLoading();

// Close dialog
Swal.close();
```