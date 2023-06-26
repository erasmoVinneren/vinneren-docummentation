Indicaciones para resolver el error de "EntityNotFound" utilizando Postman:

Abre Postman en tu computadora y asegúrate de tener acceso a la API.

Identifica qué entidad de datos falta en VTEX IO y recopila los detalles necesarios para crearla. Por ejemplo, si es un producto, asegúrate de tener el nombre, descripción, precio y otros campos relevantes.
En caso de que ya exista esa entidad de datos pero con otro nombre, haz un GET que traiga esta información.
Abre una nueva solicitud en Postman y establece el método HTTP en "POST".
Ingresa la URL de la API de VTEX correspondiente a la creación de la entidad que falta. 
En el encabezado de la solicitud, asegúrate de incluir las credenciales y los encabezados necesarios para autenticarte y autorizar el acceso a la API de VTEX IO.
En el cuerpo de la solicitud, proporciona los datos necesarios para crear la entidad que falta. Asegúrate de seguir el formato adecuado y cumplir con los requisitos de la entidad en cuestión.
Haz clic en el botón "Enviar" para enviar la solicitud a la API de VTEX IO.
Verifica la respuesta de la API para asegurarte de que la entidad se haya creado correctamente. Si recibes una respuesta exitosa con el ID o detalles de la entidad creada, significa que se ha solucionado el error de "EntityNotFound".
Si la respuesta indica algún error, verifica los datos proporcionados, los encabezados de autenticación y los permisos de acceso. Asegúrate de corregir cualquier error y volver a enviar la solicitud.
