# ⛵ Timonelingo - Curso de Timonel YCN & PNA

Aplicación interactiva gamificada (estilo Duolingo) para estudiar y repasar los contenidos del **Curso de Timonel de Yate Vela Motor (Prefectura Naval Argentina / Yacht Club Neuquén)**.

Diseñada para estudiantes principiantes con rigor conceptual oficial, navegación táctil y simulacro de examen.

---

## 🚀 Cómo publicarlo en GitHub Pages (Paso a Paso)

GitHub Pages es un servidor estático gratuito ideal para esta app. No requiere instalar servidores ni configurar bases de datos complejas:

1. **Subir el proyecto a GitHub**:
   - Crea un nuevo repositorio en tu cuenta de GitHub (ej. `timonelingo`).
   - Sube este archivo `index.html` (y la carpeta `Bibliografia` si deseas conservarla de referencia).
2. **Activar GitHub Pages**:
   - En tu repositorio de GitHub, haz clic en **Settings** (Configuración) ⚙️.
   - En el menú lateral izquierdo, ve a **Pages**.
   - En **Build and deployment > Source**, selecciona **Deploy from a branch**.
   - En **Branch**, selecciona `main` (o `master`) y la carpeta `/ (root)`.
   - Haz clic en **Save** (Guardar).
3. **¡Listo!**:
   - En unos minutos, GitHub te dará un enlace público (ej. `https://tu-usuario.github.io/timonelingo/`) para compartir directamente por WhatsApp o grupo de estudio con tus compañeros.

---

## 📱 Características y Módulos

1. **🗺️ Temario Progresivo (12 Subunidades)**:
   - **Unidad 1: Aerodinámica, Carta y Mareas**: Viento aparente, empuje en sotavento, escala lateral de latitudes (millas), Cero de Cartas, regla de los duodécimos y declinación magnética.
   - **Unidad 2: Maniobras, Fondeo y Amarras**: Hombre al agua (timón a la banda de caída), Curva de Boutakov, desatraque con spring, longitud de fondeo (3 a 5 veces la sonda), cabos de fondeo (nylon vs prohibición de polipropileno flotante), As de Guía, Ballestrinque y amarre a cornamusa.
   - **Unidad 3: Motores Marinos y Cuidado**: Diésel vs nafta (autoignición por compresión vs chispa de bujía, seguridad en sentina), filtro trampa de agua/decantador, purga manual, rodete de goma (impeller) y apagado seguro tras enfriar en ralentí.
   - **Unidad 4: Meteorología, RIPA y Balizamiento**: El Pampero (achicar paño antes de la racha), caída del barómetro, Sudestada, luces de navegación (tope 225°, alcance 135°, bandas verde/roja), buque sin gobierno (dos rojas), prioridades vela vs vela y boyas IALA B (Regla SIR).
2. **🎯 Reconocimiento Táctil Gráfico (2 Modos Especializados)**:
   - **⛵ Partes del Velero (FIG. 1 del Manual YCN)**: Identificación de 15 partes de casco, cubierta y aparejo: Púlpito de proa, Proa, Tambucho, Carlinga, Mástil, Botavara, Candeleros y Guardamancebos, Escotilla principal, Molinete (winche), Cockpit (bañera), Caña del timón, Balcón de popa, Espejo, Pala del timón y Quillote.
   - **🪁 Partes de la Vela Mayor (FIG. 16 del Manual YCN)**: Identificación de 9 elementos de la vela: Puño de driza, Puño de amura, Puño de escota, Grátil, Baluma, Pujámen, Battens (sables), Faja o mano de rizos y Ollaos.
3. **🃏 Fichas Mnemotécnicas (Flashcards)**:
   - 12 tarjetas de repaso rápido con los conceptos clave y reglas mnemotécnicas.
4. **📜 Simulacro de Examen Oficial**:
   - 10 preguntas aleatorias del banco con exigencia del 70% de aprobación reglamentario.

---

## 🛠️ Arquitectura y Datos

- **100% Frontend Estático**: No requiere servidores backend, API keys ni bases de datos pesadas (como SQLite/sql.js), lo que garantiza carga instantánea en cualquier celular con bajo consumo de datos.
- **Persistencia con `localStorage`**: Cada compañero guarda su propio progreso, racha de días, puntos ganados y vidas en su propio dispositivo sin mezclar datos con los demás.
- **Efectos de sonido nativos**: Generados con la Web Audio API del navegador, sin dependencias de archivos de audio externos.
