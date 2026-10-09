LR CONNECT V3 — IA REAL + BIBLIOTECA RAG

Qué cambia:
- Backend Node/Express para no exponer la API key en el navegador.
- Asistente IA conectado a OpenAI Responses API.
- File Search para consultar los PDFs de docs/ como biblioteca de conocimiento.
- Generador de contenido conectado a la misma biblioteca.
- Endpoint /api/health para saber si IA y biblioteca están configuradas.
- Fallback local si abres index.html sin servidor.

REQUISITOS
1) Node.js 20+ recomendado.
2) Una API key de OpenAI con facturación/crédito disponible.
3) Copia .env.example a .env y añade OPENAI_API_KEY.

INSTALACIÓN
npm install
npm run setup:knowledge

El segundo comando crea una biblioteca vectorial y sube los PDFs de docs/.
Copia el OPENAI_VECTOR_STORE_ID que muestra el comando al archivo .env.

ARRANQUE
npm start
Abre: http://localhost:3000

SEGURIDAD
- NO pongas OPENAI_API_KEY dentro de index.html.
- NO subas .env a GitHub.
- Los documentos cargados deben ser documentos que tengas derecho a usar.
- Antes de publicar comercialmente, confirma autorización para marca, imágenes, catálogo y materiales LR.

NOTA
La V3 es un prototipo funcional de integración. Los precios y productos mostrados en la interfaz siguen siendo los datos de demostración de la V2 hasta que se haga una importación completa y se verifique el catálogo vigente.
