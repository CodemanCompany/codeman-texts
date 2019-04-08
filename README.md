# Codeman Text

El siguiente documento contiene los estándares de textos que se deben utilizar en cada uno de los siguientes contextos:

## Básicos

Textos básicos en un **Dashboard**.

* **Sign Up**: Crear cuenta.
* **Log In**: Iniciar sesión.
* **Log Out**: Cerrar sesión.

## Posición de los iconos

Los iconos **preferentemente** deben estar a la izquierda del texto, ejemplo:

* 😎 Codeman

## Posición de los botones de Cancelar y Aceptar

Se debe seguir la siguiente recomendación en todos los sistemas propios.

### En un Modal

El botón de **Cancelar** debe ir a la izquierda y el de **Aceptar** a la derecha.

### En un Diálogo

El botón de **Aceptar** a la izquierda y el de **Cancelar** debe ir a la derecha.

## Dashboard

Las acciones básicas mejor conocidas como **CRUD** deben tener los siguientes nombres (Español / English):

* **Create:** Agregar / Add.
* **Read:** Ver / View.
* **Update:** Editar / Edit.
* **Delete:** Eliminar / Remove.

## Datatables

Los siguientes textos son referentes a los campos que deben aparecer en Datatables.

###### Traducción de Datatables

```json
{
	"sEmptyTable": "Ningún dato disponible en esta tabla",
	"sInfo":  "Mostrando registros del _START_ al _END_ de un total de _TOTAL_ registros",
	"sInfoEmpty": "Mostrando registros del 0 al 0 de un total de 0 registros",
	"sInfoFiltered": "(filtrado de un total de _MAX_ registros)",
	"sInfoPostFix":  "",
	"sInfoThousands": ",",
	"sLengthMenu": "Mostrar _MENU_ registros",
	"sLoadingRecords": "Espere un momento por favor.",
	"sProcessing": "Procesando...",
	"sSearch": "Buscar:",
	"sUrl": "",
	"sZeroRecords": "No se encontraron resultados",
	"oPaginate": {
		"sFirst": "Primero",
		"sLast": "Último",
		"sNext": "Siguiente",
		"sPrevious": "Anterior",
	},
	"oAria": {
		"sSortAscending": ": Activar para ordenar la columna de manera ascendente",
		"sSortDescending": ": Activar para ordenar la columna de manera descendente",
	},
}
```

###### Atributos de una tabla

```html
<table>
	<thead>
		<tr>
			<th>ID</th>
			<th>Fecha de creación</th>
			<th>Fecha de modificación</th>
		</tr>
	</thead>
</table>
```

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

###### Delete

```javascript
Swal.fire( {
	"cancelButtonText": "Cancelar",
	"confirmButtonColor": "#dc3545",
	"confirmButtonText": "Eliminar",
	"reverseButtons": true,
	"showCancelButton": true,
	"text": "¿Realmente deseas eliminar el elemento seleccionado?",
	"title": "Advertencia, esta acción no se puede deshacer",
	"type": "warning",
} ).then( ( result ) => {
	if ( result.value ) {
		// Write here
	}	// end if
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

###### Question

```html
<h3>¿Realmente deseas eliminar el siguiente elemento?</h3>
<p>Advertencia, esta acción no se puede deshacer.</p>
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

###### Synchronization

```javascript
Swal.fire( {
	"allowOutsideClick": false,
	"text": "Un momento por favor.",
	"title": "Sincronizando",
} )
Swal.showLoading();
```

###### Unauthenticated

```javascript
Swal.fire( {
	"confirmButtonText": "Aceptar",
	"text": "Por favor vuelve a iniciar sesión.",
	"title": "Tu sesión ha expirado",
	"type": "error",
} )
.then( ( result ) => {
	if( result.value )
		location.href = '/';
} );
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

###### Loading in authentication

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

## Sign Up

###### Success

```javascript
Swal.fire( {
	"confirmButtonText": "Continuar",
	"text": "Completa tu registro siguiendo las instrucciones enviadas a tu correo electrónico.",
	"title": "Registro exitoso",
	"type": "success",
} );
```

## Payment

###### Loading in payment

```javascript
Swal.fire( {
	"allowOutsideClick": false,
	"text": "Espere un momento por favor.",
	"title": "Realizando transacción",
} )
Swal.showLoading();

// Close dialog
Swal.close();
```
