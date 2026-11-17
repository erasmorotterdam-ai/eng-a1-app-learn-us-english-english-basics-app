# Order Up · Inglés americano del trabajo (Pre-A1 → A1)

App web de un solo archivo (`index.html`), sin servidor, sin cuenta y sin dependencias que instalar. 33 unidades cortas de inglés americano cotidiano: los temas de la vida diaria (saludos, presentaciones, alfabeto, números, países, familia, rutinas, días, comida, restaurante, compras, ropa, casa, direcciones, transporte, clima, salud, pasatiempos, trabajo y estudio), tres escenas extra y 11 sectores de *English at Work* (básico, construcción, agricultura y mantenimiento, limpieza, restaurantes y hoteles, ventas, bancos, hospitales, oficina, transporte y entregas, otras profesiones).

1. **Good morning!** (Tema 1): Saludos y charla breve con compañeros
2. **Nice to meet you** (Tema 2): Presentarte con un compañero nuevo
3. **Alphabet and spelling** (Tema 3): El alfabeto y cómo deletrear
4. **Could you say that again?** (Extra): Pedir que repitan, hablar más lento y deletrear
5. **Numbers and age** (Tema 4): Números, teléfono y edad
6. **Countries and languages** (Tema 5): Países, nacionalidades e idiomas
7. **Family** (Tema 6): Familia y personas cercanas
8. **Daily routines** (Tema 7): Rutinas del día
9. **Days and dates** (Tema 8): Días, meses y fechas
10. **What time is the meeting?** (Extra): Horas, citas y avisos de retraso
11. **Food and drinks** (Tema 9): Comida, bebidas y preferencias
12. **At the coffee shop** (Extra): En la cafetería
13. **At a restaurant** (Tema 10): Pedir una comida y la cuenta
14. **Shopping** (Tema 11): Comprar, preguntar precios y pagar
15. **Clothes and colors** (Tema 12): Ropa, colores y uniformes
16. **Home** (Tema 13): La casa, las habitaciones y el barrio
17. **Where is the break room?** (Tema 14): Preguntar dónde está algo y entender indicaciones
18. **Transport and travel** (Tema 15): Transporte, rutas y viajes
19. **Weather** (Tema 16): El clima y la charla del tiempo
20. **Health and feelings** (Tema 17): Salud, síntomas y emociones
21. **Hobbies and preferences** (Tema 18): Pasatiempos y gustos
22. **Work and study** (Tema 19): Trabajo, estudios y horarios
23. **Workplace basics** (21.1): Comunicación laboral básica
24. **English at Work: Construction** (21.2): Construcción: seguridad, herramientas e instrucciones
25. **English at Work: Farming and maintenance** (21.3): Agricultura y mantenimiento
26. **English at Work: Cleaning and housekeeping** (21.4): Limpieza y servicios generales
27. **English at Work: Restaurants and hotels** (21.5): Restaurantes y hoteles
28. **English at Work: Retail and sales** (21.6): Tiendas y ventas
29. **English at Work: Banking and customer service** (21.7): Bancos y atención al cliente
30. **English at Work: Hospitals and clinics** (21.8): Hospitales y clínicas
31. **English at Work: Office and administration** (21.9): Oficinas y administración
32. **English at Work: Transportation and deliveries** (21.10): Transporte y entregas
33. **English at Work: Other professions** (21.11): Otras profesiones: presentarte y entrevistas

Cada unidad tiene: escena para escuchar, frases completas con variantes (escucha repetida y práctica oral), ejercicios, conversación con opciones, conversación hablada con retroalimentación, repaso espaciado y **enlaces gratuitos a recursos externos de listening y speaking**.

## Publicar en GitHub Pages (https)

1. Crea un repositorio en GitHub (por ejemplo `order-up`), público.
2. Sube a la raíz del repositorio estos archivos: `index.html`, `.nojekyll` y `README.md`.
3. Ve a **Settings → Pages**. En *Build and deployment* elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
4. Espera uno o dos minutos. La app queda en `https://TU-USUARIO.github.io/order-up/`.

GitHub Pages sirve el sitio por **https**, que es lo que el navegador exige para permitir el micrófono.

## Micrófono y voces

- El dictado usa la **Web Speech API** del navegador. Funciona en **Chrome y Edge** (escritorio y Android). Firefox no la ofrece; Safari tiene soporte parcial. Cuando no hay dictado, la app permite **escribir** lo que dirías.
- Chrome y Edge envían el audio a servicios de Google o Microsoft para convertirlo en texto. La app solo recibe el texto.
- El dictado **transcribe lo que dices**; si sale bien, es buena señal de que se te entiende. No mide tu pronunciación sonido por sonido.
- Las voces de audio son las del navegador. En **Edge** hay voces "Natural" en línea. La app elige voz según el sexo que indiques para cada personaje y puedes escoger una voz concreta en el botón *Voces*.
- El progreso, las frases guardadas y los ajustes se guardan en `localStorage` del navegador. No hay cuenta ni servidor.

## Cómo editar o agregar unidades

Todo el contenido está en `index.html`, en el bloque `UNITS.push({...})` de cada unidad: `lines` (escena), `chunks` (frases con variantes), `ex` (ejercicios), `sim` (conversación con opciones), `turns` (conversación hablada con reglas de evaluación), `notes`, `goals` y `res` (enlaces). Copia una unidad existente, cambia el `id` y los `id` de sus frases y ejercicios (deben ser únicos) y agrégala debajo de la última.

## Enlaces externos

Los enlaces se revisaron el 15 de noviembre de 2026. Son sitios de terceros: pueden cambiar de dirección, pedir registro para ciertas funciones o tener acentos variados. Si alguno deja de funcionar, edita el arreglo `res` de la unidad.
