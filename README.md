Login
Permite ingresar un nombre de usuario y contrasena para entrar a la agencia digital

Facturas
Un repositorio donde el usuario recibe sus facturas (Combos, pague por ver, etc.)

Servicios
Listado de grupos de servicios disponibles para el usuario. Cada servicio tiene un boton de activado y desactivado. Algunos servicios pueden requerir al usuario proveer parametros de operacion. Por ejemplo, el servicio de suscripciones a alertas requiere del email del usuario.

Servicio: Detalle de llamadas
Un listado de las llamadas realizadas usando el servicio de telefonia.

Servicio: Pague por ver
Un listado de programas y productos que pueden ser contratados por el usuario en linea.

Cuenta del Usuario
Una sola pagina que incluye la informacion del usuario y diferentes maneras de mantenerla actualizada.

Boton de cambiar cuenta
Permite ver los datos y servicios de otra cuenta del usuario.

API
POST /access_token
{ usuario: "usuario",
  contrasena: "contrasena }

Respuesta:
{ usuario: "usuario",
  access_token: "1234567890" }


GET /cuentas?access_token=1234567890

Respuesta:
{ usuario: "usuario"
  cuentas: [ {"nombre": "Datilmedia S.A.",
              ruc: "0992716552771"}
              notificaciones_pendientes: true } ] }
