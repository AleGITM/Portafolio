# Portafolio Web | Guillermo Muñoz

Portafolio web desarrollado como proyecto académico de Ingeniería en Informática. Su propósito es presentar mi perfil profesional, las tecnologías utilizadas durante mi formación y uno de mis principales proyectos de análisis de datos.

El sitio está construido con **Astro, JavaScript, TypeScript y Tailwind CSS**, con un diseño inspirado en la **estética cyberpunk** y el uso de colores neón, contrastes oscuros y efectos visuales.

## Sitio web

🌐 **[Ver portafolio](https://portafolio-alem.netlify.app/)**

## Tecnologías utilizadas

- **Astro:** estructura del sitio y generación de páginas estáticas.
- **JavaScript y TypeScript:** funcionalidades interactivas, navegación y cambio de tema.
- **Tailwind CSS:** estilos, diseño adaptable y distribución de elementos.
- **CSS:** animaciones, transiciones y efectos visuales personalizados.
- **Node.js y npm:** entorno de desarrollo, administración de dependencias y ejecución de comandos.
- **Git y GitHub:** control de versiones y seguimiento del desarrollo.
- **Netlify:** alojamiento y publicación del portafolio.

## Estructura del portafolio

El sitio contiene tres páginas principales:

### Inicio

Presentación personal con una interfaz de inspiración cyberpunk, colores neón, efectos visuales y acceso a las demás secciones.

### Sobre mí

Información sobre mi formación académica, intereses profesionales y tecnologías relacionadas con el desarrollo de software.

### Proyectos

Presentación del proyecto de Business Intelligence **«Resiliencia Económica del Territorio Agrícola de Colchagua»**.

La investigación estudia características económicas, agrícolas y ambientales de las diez comunas de la provincia de Colchagua mediante datos oficiales.

El trabajo se organiza en cinco etapas:

1. **Datos y Datamart:** recopilación, limpieza e integración de información de SII, CONAF, DGA, ODEPA y ODEPA–CIREN.
2. **Análisis exploratorio:** estudio de indicadores territoriales y registros históricos de incendios forestales.
3. **Machine Learning:** segmentación de las comunas mediante clustering jerárquico.
4. **Forecast:** comparación de métodos para pronosticar incendios forestales.
5. **Power BI:** visualización de indicadores mediante un dashboard desarrollado en Power BI Desktop.

La página permite descargar los datasets, notebooks y el archivo del dashboard para consultar el trabajo realizado.

## Archivos disponibles

Los entregables se encuentran en `public/archivos/`:

| Archivo | Descripción |
|---|---|
| `Datasets.zip` | Conjunto de datos utilizados en el proyecto. |
| `Notebooks.zip` | Colección de notebooks de investigación. |
| `Analisis_Exploratorio.ipynb` | Análisis exploratorio y visualizaciones. |
| `ML_SEGMENTACION.ipynb` | Segmentación territorial mediante Machine Learning. |
| `FORECAST.ipynb` | Modelos de pronóstico y evaluación. |
| `DashboardColch.pbix` | Dashboard desarrollado en Power BI Desktop. |

**Nota:** el archivo `.pbix` requiere Power BI Desktop para abrirse.

## Organización de carpetas

El proyecto sigue la estructura de Astro, separando los componentes reutilizables, las páginas, los estilos y los archivos públicos.

```text
Portafolio/
├── .github/
│   └── workflows/
│       └── ci.yml         # Verificación automática: ESLint y compilación
├── public/
│   ├── archivos/          # Datasets, notebooks y dashboard Power BI
│   └── icons/             # Íconos del sitio
├── src/
│   ├── components/        # Componentes reutilizables de la interfaz
│   ├── layouts/           # Estructura compartida de las páginas
│   ├── pages/             # Inicio, Sobre mí y Proyectos
│   └── styles/            # Estilos globales (global.css)
├── astro.config.mjs       # Configuración de Astro
├── eslint.config.js       # Reglas de ESLint
├── tsconfig.json          # Configuración de TypeScript
├── package.json           # Dependencias y comandos del proyecto
└── README.md              # Documentación del portafolio
```

Esta organización permite mantener separadas las distintas partes del sitio y facilita su mantenimiento.

## Instalación y ejecución local

Para ejecutar el portafolio en un entorno local, se necesita **Node.js y npm**. Durante el desarrollo se utilizó **Node.js 22.15.0**.

Clonar el repositorio:

```bash
git clone https://github.com/AleGITM/Portafolio.git
```

Ingresar al directorio:

```bash
cd Portafolio
```

Instalar las dependencias:

```bash
npm install
```

Iniciar el servidor de desarrollo:

```bash
npm run dev
```

Abrir la dirección indicada en la terminal, normalmente `http://localhost:4321`.

## Comandos disponibles

| Comando | Función |
|---|---|
| `npm run dev` | Inicia el servidor de desarrollo. |
| `npm run lint` | Ejecuta ESLint para revisar el código. |
| `npm run build` | Genera la versión de producción en `dist/`. |
| `npm run preview` | Permite revisar localmente la versión compilada. |

## Características del sitio

- Diseño adaptable a dispositivos móviles y computadores.
- Modo oscuro y claro.
- Navegación entre páginas.
- Estética cyberpunk con colores neón y ambientación nocturna.
- Animaciones y efectos visuales personalizados acordes con la estética del sitio.
- Presentación interactiva de las etapas del proyecto.
- Enlaces de descarga de la investigación realizada.
- Publicación mediante Netlify.

## Uso de inteligencia artificial

Durante el desarrollo de este portafolio utilicé **ChatGPT (OpenAI)** como herramienta de apoyo tanto en el diseño como en la programación del sitio web.

La idea inicial y la propuesta estética surgieron de mis propias preferencias, especialmente de elementos de la estética cyberpunk. A partir de esa idea, utilicé inteligencia artificial para ayudarme a implementar las distintas funcionalidades del portafolio.

Su utilización incluyó:

- **Desarrollo de código:** generación, adaptación y modificación de código en Astro, JavaScript, TypeScript, Tailwind CSS y CSS.
- **Diseño visual:** implementación de la estética nocturna, colores neón, animaciones, transiciones y efectos interactivos.
- **Corrección de errores:** identificación de problemas, propuestas de solución y ajustes realizados durante el desarrollo.
- **Simplificación y optimización:** revisión de partes del código para reducir complejidad, evitar elementos innecesarios y mejorar su organización.
- **Pruebas y verificación:** apoyo en la revisión del funcionamiento del sitio, la compatibilidad entre dispositivos y la interpretación de los resultados de las herramientas de validación.

El código desarrollado con asistencia de IA fue revisado, probado y ajustado durante el proceso. También utilicé herramientas como ESLint y la compilación de Astro para comprobar que el proyecto no presentara errores de análisis estático ni de construcción.

## Control de versiones

El desarrollo se gestionó mediante Git y GitHub, utilizando commits para registrar la evolución del portafolio y sus modificaciones.

Cada push o pull request hacia `main` activa un flujo de GitHub Actions (`.github/workflows/ci.yml`) que instala las dependencias con `npm ci`, revisa el código con ESLint y compila el sitio con Astro, usando Node.js 22. Si alguno de los pasos falla, GitHub marca el cambio con error.

**Repositorio:** [github.com/AleGITM/Portafolio](https://github.com/AleGITM/Portafolio)

## Autor

**Guillermo Muñoz**  
Estudiante de Ingeniería en Informática  
Chile

---

2026.