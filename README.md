# Análisis del terreno mediante MDT — Cerdanya y Alt Urgell

![Modelo Digital del Terreno de la Cerdanya y el Alt Urgell](MDT.png)

## Descripción

Análisis territorial del relieve de la **Cerdanya y el Alt Urgell**, dos comarcas de montaña situadas en el Pirineo catalán.

El proyecto utiliza un **Modelo Digital del Terreno (MDT) de 5 metros de resolución** para generar una base cartográfica regional y estudiar las principales variables topográficas: elevación, sombreado del relieve, curvas de nivel, pendiente y orientación de las laderas.

Los resultados permiten interpretar la estructura física del territorio y sirven como información de partida para estudios posteriores de hidrología, riesgos naturales, planificación territorial y gestión ambiental.

## Objetivos

- Caracterizar el relieve de la Cerdanya y el Alt Urgell.
- Representar la distribución espacial de las elevaciones.
- Identificar valles, divisorias y sectores de relieve abrupto.
- Analizar la pendiente y la orientación de las laderas.
- Elaborar una serie cartográfica homogénea y legible.
- Preparar una base territorial para futuros análisis ambientales e hidrológicos.

## Área de estudio

![Localización de la Cerdanya y el Alt Urgell](localizacion.png)

El ámbito comprende las comarcas de la **Cerdanya y el Alt Urgell**. La representación conjunta permite analizar la continuidad del relieve más allá de los límites administrativos y observar la relación entre las zonas de alta montaña, los valles principales y las áreas de menor pendiente.

La configuración topográfica condiciona la ocupación del territorio, las comunicaciones, la distribución de la vegetación y la organización del drenaje superficial.

## Datos y herramientas

| Recurso | Fuente | Características | Aplicación |
|---|---|---|---|
| Modelo Digital del Terreno | Institut Cartogràfic i Geològic de Catalunya (ICGC) | Resolución espacial de 5 m | Elevación y variables derivadas |
| Límites administrativos | ICGC | Datos vectoriales | Delimitación y contextualización del ámbito |
| QGIS | Versión 3.44 | Software SIG | Procesamiento, análisis y composición cartográfica |

Los datos originales no se incluyen en el repositorio debido a su volumen. Pueden obtenerse a través de los servicios oficiales del ICGC.

## Metodología

El flujo de trabajo se ha desarrollado en QGIS:

1. Obtención y organización del MDT y de los límites administrativos.
2. Comprobación de la coherencia espacial de las capas.
3. Preparación del MDT para el ámbito de estudio.
4. Generación de las variables derivadas del relieve.
5. Clasificación y simbolización de los resultados.
6. Diseño y exportación de las composiciones cartográficas.

El análisis incluye los siguientes productos:

- Modelo Digital del Terreno.
- Sombreado del relieve.
- Curvas de nivel.
- Pendiente.
- Orientación de las laderas.

## Resultados

### Modelo Digital del Terreno

![Modelo Digital del Terreno](MDT.png)

El MDT representa la distribución espacial de las elevaciones y constituye la base del análisis. Permite reconocer los principales valles, las áreas de alta montaña y las divisorias topográficas que organizan el territorio.

### Sombreado del relieve

![Sombreado del relieve](HS.png)

El sombreado facilita la lectura tridimensional del terreno mediante la simulación de una fuente de iluminación. Ayuda a identificar crestas, fondos de valle, laderas y cambios en la morfología que pueden resultar menos evidentes en una representación basada únicamente en intervalos de elevación.

Se utiliza como recurso de apoyo visual y no como una variable física independiente.

### Curvas de nivel

![Curvas de nivel](CURVAS.png)

Las curvas de nivel conectan puntos situados a la misma altitud y complementan la representación continua del MDT. Su densidad permite interpretar cualitativamente la inclinación del terreno: una mayor proximidad entre curvas corresponde generalmente a pendientes más pronunciadas.

### Pendiente

![Mapa de pendientes](pendiente.png)

La pendiente expresa el grado de inclinación del terreno y permite diferenciar los fondos de valle y las superficies relativamente suaves de los sectores montañosos más abruptos.

Esta variable es especialmente relevante para:

- Modelización de la escorrentía superficial.
- Evaluación preliminar de procesos erosivos.
- Planificación de infraestructuras.
- Gestión forestal.
- Estudios de accesibilidad y aptitud territorial.
- Análisis de riesgos naturales.

### Orientación de las laderas

![Mapa de orientaciones](orientacion.png)

La orientación indica la dirección dominante hacia la que desciende cada ladera. En ambientes de montaña puede influir en la exposición solar, la humedad, la persistencia de la nieve y la distribución de la vegetación.

Su interpretación conjunta con la elevación y la pendiente permite caracterizar mejor los contrastes ambientales existentes entre vertientes.

## Aplicaciones

La información generada puede utilizarse como base para:

- Delimitación y caracterización de cuencas hidrográficas.
- Extracción de redes de drenaje.
- Estudios de inundabilidad y erosión.
- Análisis del riesgo de incendios forestales.
- Inventarios ambientales y forestales.
- Planificación territorial.
- Evaluación preliminar de trazados e infraestructuras.
- Estudios de accesibilidad y usos del suelo.

## Limitaciones

- El nivel de detalle está condicionado por la resolución espacial de 5 metros del MDT.
- Las variables derivadas dependen de la calidad y el preprocesamiento del modelo de elevaciones.
- No se ha realizado una validación topográfica de campo.
- La cartografía tiene una finalidad analítica y de portfolio; no sustituye un levantamiento topográfico, un estudio geotécnico ni una evaluación de riesgos de detalle.
- Las aplicaciones profesionales requerirían adaptar la escala, las fuentes y la validación a los objetivos de cada proyecto.

## Continuación del trabajo

Este análisis constituye la base topográfica de un estudio posterior sobre el comportamiento hidrológico del territorio, que incluye delimitación de cuencas, acumulación de flujo y jerarquización de la red de drenaje.

→ [Consultar el proyecto Hidrologia-Cerdanya](https://github.com/jovaro90/Hidrologia-Cerdanya)

## Estructura del repositorio

```text
Terrain-lidar-analysis/
├── README.md
├── localizacion.png
├── MDT.png
├── HS.png
├── CURVAS.png
├── pendiente.png
└── orientacion.png
```

## Autor

**Jordi Valls Roig**  
GIS Analyst · WebGIS Developer · Oceanógrafo

- [Portfolio GIS](https://github.com/jovaro90)
- [Paper Maps — WebGIS](https://github.com/jovaro90/WebGis-Paper-Maps)
- [Análisis hidrológico de la Cerdanya](https://github.com/jovaro90/Hidrologia-Cerdanya)
