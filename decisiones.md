# Registro de Decisiones de Arquitectura

Aquí dejamos anotadas las decisiones clave que tomamos como grupo para armar los servidores.

| Fecha | Componente | Opciones | Qué elegimos | Por qué lo elegimos |
| :--- | :--- | :--- | :--- | :--- |
| 31/08/2026 | Sistema Operativo | Debian / Ubuntu Server | **Ubuntu Server** | Básicamente porque es la restricción que pide el alcance del proyecto y es fácil encontrar documentación. |
| 07/09/2026 | Plataforma Web (CMS) | WordPress vs PrestaShop | **WordPress + WooCommerce** | Elegimos WordPress porque además de la tienda nos deja hacer páginas normales y subir noticias. También nos hace más fácil la vida para separar la base de datos en otra máquina tocando el archivo `wp-config.php`. |
| 10/09/2026 | Base de Datos | Todo junto vs Servidor Dedicado | **Servidor MySQL separado** | La rúbrica exige que esté en una VM distinta por seguridad. Además, así si se cae el servidor web, no se comprometen los datos directamente. |
