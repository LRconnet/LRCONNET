LR CONNECT V9 — PAQUETE PREPARADO PARA PUBLICACIÓN

QUÉ ES
Una aplicación web unificada en fase de prototipo, basada en las versiones anteriores. Incluye interfaz, catálogo inicial, biblioteca documental, área de contenido, CRM local y endpoints de IA preparados.

IMPORTANTE: TODAVÍA NO ES UNA APP DE PRODUCCIÓN
- No hay registro/inicio de sesión real ni base de datos online.
- Los contactos del CRM se guardan en el navegador del dispositivo; no introduzcas datos reales sensibles.
- La IA requiere OPENAI_API_KEY y OPENAI_VECTOR_STORE_ID en el servidor. Si no se configuran, el resto de la demo puede abrirse pero la IA responderá que no está configurada.
- Los precios incluidos proceden del catálogo Collection 2025|02 aportado y deben verificarse antes de uso comercial.
- La app es independiente y no oficial de LR Health & Beauty. Comprueba los permisos de marca y documentos antes de hacerla pública.

PROBAR EN ORDENADOR
1. Instala Node.js 20 o superior desde https://nodejs.org
2. Descomprime este ZIP en una carpeta.
3. Abre una terminal en esa carpeta.
4. Ejecuta: npm install
5. Ejecuta: npm start
6. Abre http://localhost:3000

PUBLICAR ONLINE (PASO SIGUIENTE)
El archivo render.yaml deja preparada la configuración inicial para un servicio Node en Render. Para publicarla necesitas una cuenta y subir este proyecto a un repositorio GitHub privado. Luego conectas ese repositorio a Render. No compartas claves en GitHub.

VARIABLES DE ENTORNO DEL SERVIDOR (solo cuando quieras activar IA)
OPENAI_API_KEY = tu clave privada, introducida directamente en el panel del hosting
OPENAI_VECTOR_STORE_ID = identificador de la biblioteca vectorial creada
OPENAI_MODEL = gpt-6-luna (o un modelo habilitado en tu proyecto)

PARA ACTIVAR LA BIBLIOTECA IA
En un entorno local de confianza, configura OPENAI_API_KEY y ejecuta npm run setup:knowledge. El proceso sube los PDFs incluidos a OpenAI y puede generar costes de API/almacenamiento. No ejecutes el proceso hasta que quieras activar esa función.

NO HAGAS AÚN
No invites socios, no guardes datos reales de clientes y no anuncies la app como oficial. Antes del lanzamiento público hay que implementar autenticación real, base de datos con aislamiento por usuario, privacidad/cumplimiento RGPD, protección antiabuso, límites de gasto y pruebas de seguridad.
