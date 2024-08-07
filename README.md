# Proyecto Final

Nombre: Cesar Soto Segura

## Análisis del dataset del desarrollo histórico de la Electromovilidad según la IEA

La electromovilidad, o el uso de vehículos eléctricos (EVs), representa una revolución en la industria del transporte. Esta tecnología se basa en la utilización de motores eléctricos en lugar de motores de combustión interna, ofreciendo una alternativa más limpia y eficiente. A medida que el mundo enfrenta desafíos ambientales cada vez mayores, la electromovilidad se ha posicionado como una solución clave para reducir las emisiones de gases de efecto invernadero, mejorar la calidad del aire y disminuir la dependencia de los combustibles fósiles.

#### Importancia Global

A nivel mundial, la adopción de vehículos eléctricos está creciendo rápidamente, impulsada por los compromisos de los gobiernos y las empresas para alcanzar metas de sostenibilidad. La electromovilidad es crucial para cumplir con los objetivos del Acuerdo de París. Además, los vehículos eléctricos presentan beneficios económicos, como la reducción de los costos operativos y el mantenimiento en comparación con los vehículos tradicionales.

###Electromovilidad en Latinoamérica

En América Latina, la electromovilidad tiene un potencial significativo para transformar el sector del transporte. La región enfrenta desafíos únicos relacionados con la urbanización rápida y la calidad del aire, lo que hace que la adopción de vehículos eléctricos sea particularmente relevante. Países como Brasil, México y Colombia están comenzando a implementar políticas y programas para fomentar el uso de EVs, incluyendo incentivos fiscales, subsidios y la expansión de la infraestructura de carga.

#### El Caso de Chile

Chile se destaca como un líder en la promoción de la electromovilidad en América Latina. El país ha establecido ambiciosos objetivos para aumentar la adopción de vehículos eléctricos, incluyendo la meta de electrificar el 100% del transporte público urbano para 2040. Santiago, la capital, ya cuenta con una de las flotas de autobuses eléctricos más grandes del mundo. Además, Chile es uno de los mayores productores de litio, un componente esencial en las baterías de los vehículos eléctricos, lo que le brinda una ventaja estratégica en el desarrollo de esta industria.

La transición hacia la electromovilidad no solo contribuirá a la reducción de emisiones y a la mejora de la calidad del aire, sino que también ofrecerá oportunidades económicas, como la creación de empleos y el impulso a la innovación tecnológica. En resumen, la electromovilidad es un pilar fundamental para un futuro más sostenible y resiliente, tanto a nivel global como regional.

### Fuente de los Datos

Los datos utilizados para este proyecto vienen de las publicaciones de La Agencia Internacional de Energía (IEA, por sus siglas en inglés, International Energy Agency). La IEA es una organización autónoma fundada en 1974 dentro del marco de la Organización para la Cooperación y el Desarrollo Económicos (OCDE) en respuesta a la crisis del petróleo de los años 70. Su misión principal es promover políticas energéticas que aseguren energía confiable, asequible y limpia para sus países miembros y más allá.

 El dataset utilizado es parte del Global EV Outlook 2024, publicado en abril del 2024.

https://www.iea.org/data-and-statistics/data-product/global-ev-outlook-2024

Del análisis realizado por medio del Notebook Análisis, se identifican que el dataset es complejo con mucha información catalogados como datos históricos o proyecciones declaradas por los gobiernos. Estas proyecciones se evalúan como Escenario de Políticas Declaradas (STEPS, por sus siglas en inglés) está diseñado para proporcionar una idea de la dirección predominante de la progresión del sistema energético, basándose en un análisis detallado del panorama de políticas actual. Proporciona una evaluación más granular, sector por sector, de las políticas que se han puesto en marcha para alcanzar las metas declaradas y otros objetivos relacionados con la energía, teniendo en cuenta no solo las políticas y medidas existentes sino también las que están en desarrollo. El STEPS proporciona un punto de referencia más conservador para el futuro que el Escenario de Promesas Anunciadas (APS, por sus siglas en inglés), al no dar por sentado que los gobiernos alcanzarán todas las metas anunciadas. Al igual que el APS, no está diseñado para lograr un resultado particular.

El Data Set está compuesto por las siguientes columnas:

- Region: Variable categórica del tipo string con información del País
- Category: Variable categórica del tipo string con información que indica el tipo de dato, si es histórico u otra categoría.
- Parameter: Variable categórica del tipo string con información que indica el tipo de dato, representa si son ventas, stock y participación en el mercado.
- Mode: Variable categórica del tipo string con información de si la información está relacionada con qué tipo de vehículo.
- Powetrain: Variable categórica del tipo string con información de si la información está relacionada con la subcategoría de vehículos eléctricos.
- Year: Variable numérica del tipo entero que indica el año al que pertenece la información.
- Unit: Variable del tipo categórica del tipo string que indica la unidad de medida del dato.
- Value: Variable numérica del tipo foat que entrega el valor numérico de la medición.

los detalles de la información de cada columna son:

- Columna region se puede identificar que la información se divide en 3 grupos principales: Valores Globales, Europa-EU27-resto del mundo, y un desglose por país.
- Columna Category, se identifica dos grupos principales compuesto con valores históricos reales, más el grupo de proyecciones compuestos por proyecciones STEP y APS.
- Columna Parameter entrega información relacionada a diferentes parámetros que se miden en general para la electromovilidad, dentro de los que se pueden encontrar el Stock de EV por años, Ventas de EV por año, porcentaje de Ventas y Stock, Numero de cargadores por año, combustible demandado y energía eléctrica demandada.
- Columna Unit indica la unidad de medida de los valores de la columna "Value", donde los valores pueden ser cantidad de vehículos, Porcentajes, Numero de puntos de carga, Millones de Barriles de combustible por día, y GWH de energía eléctrica.

El enfoque del proyecto es visualizar el Escenario de la electromovilidad a nivel mundial usando solo los datos históricos acumulados, realizando una comparación de America latina con respecto al mundo y analizar cómo es el comportamiento de Chile con respecto al resto de LATAM.

El análisis final se presenta en el notebook visualización, donde se utilizan gráficos del tipo barra apilada, gráficos de cinta apilada, gráficos de torta y gráficos de dispersión, para mejor visualización de la información.

Importante: El análisis solo se base en los datos del Dataset. Dentro del análisis se identificó una falta de información para Chile ya que los valores de venta de vehículos eléctricos consideran solo Autos y no Buses y Camiones, los cuales han tenido una tendencia en aumento en los últimos 3 años, tanto por las políticas de transporte público como la información suministrada por la Asociación Nacional Automotriz de Chile ANAC.
