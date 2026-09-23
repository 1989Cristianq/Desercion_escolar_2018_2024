

## 1







Especialización en Analítica de Datos
Proyecto II



Título del Proyecto:
Modelo de aprendizaje automático para predicción del índice de deserción escolar a nivel
departamental en Colombia entre (2018- 2024) basado en indicadores de salud pública


Presentado por:

## Angelica Mayerly Tamayo Suarez
## Cristian Camilo Quintero Mejía
## José Raúl Leiva Méndez


Bajo la dirección de:
## Raul Alejandro Muñoz Galindo
Bogotá DC,

## 2

Tabla de contenido
- Introducción .............................................................................................................................. 4
-  Identificación y planteamiento del problema ........................................................................... 5
2.1 Formulación o Pregunta de Investigación ........................................................................ 7
- Objetivos ................................................................................................................................... 8
3.1 Objetivo general ............................................................................................................... 8
3.2 Objetivos específicos ........................................................................................................ 8
- Justificación .............................................................................................................................. 9
- Marco de Referencia ............................................................................................................... 11
Antecedentes internacionales: .................................................................................................... 12
Marco Teórico ............................................................................................................................ 16
Marco Conceptual .................................................................................................................... 18
Marco Contextual ..................................................................................................................... 19
Marco Legal ............................................................................................................................... 20
- Metodología CRISP-DM ........................................................................................................ 23
Fases de CRISP-DM aplicadas al proyecto ................................................................................ 24
I. Comprensión del negocio ................................................................................................... 24
II. Comprensión de los datos .............................................................................................. 24
III. Preparación de los datos ............................................................................................. 24
IV. Modelado .................................................................................................................... 25
Protocolo de Investigación ............................................................................................................. 26
- Técnicas investigativas ....................................................................................................... 26
- Tipo de estudio, métodos y diseño de investigación .......................................................... 27
- Enfoque Metodológico ....................................................................................................... 27
- Diseño Metodológico ......................................................................................................... 27

## 3

- Modelado Predictivo .......................................................................................................... 28
- Triangulación ..................................................................................................................... 28
- Participantes o unidad de análisis ....................................................................................... 28
- Técnicas e instrumentos de recolección de datos ............................................................... 29
- Planificación y Viabilidad del proyecto .................................................................................. 29
- Presupuesto ............................................................................................................................. 29
- Consideraciones éticas, de gobernanza de datos y reproducibilidad ...................................... 31
-  Referencias bibliográficas ................................................................................................. 34



## 4

## 1. Introducción

La educación básica y media constituye el pilar fundamental para el desarrollo
socioeconómico de cualquier país. Sin embargo, la permanencia de los estudiantes en el sistema
educativo está condicionada por múltiples factores externos que van más allá del entorno
académico. La deserción escolar ha sido tradicionalmente analizada desde perspectivas
socioeconómicas o de infraestructura, pero el impacto directo del panorama epidemiológico y de
salud pública en la continuidad educativa ha recibido menor atención.
La deserción escolar en Colombia trasciende el ámbito académico, viéndose condicionada
por las condiciones sanitarias y epidemiológicas del entorno departamental, las cuales actúan
como barreras externas a la permanencia. La mala salud, tanto por enfermedades crónicas como
por episodios recurrentes de morbilidad, afecta la asistencia y el rendimiento académico, mientras
que las condiciones socioeconómicas limitan la capacidad de las familias para garantizar la
permanencia de sus hijos en el sistema educativo
Al explorar la intersección de educación y salud aplicando técnicas de analítica de datos
sobre fuentes abiertas gubernamentales, Este proyecto propone la construcción de un modelo
predictivo que permita anticipar la deserción escolar en los niveles de educación básica y media,
considerando las condiciones de salud como variable explicativa central. El periodo de análisis
comprendido entre 2018 y 2024, busca ofrecer una visión amplia y actualizada de las tendencias
nacionales, con el fin de aportar insumos para la toma de decisiones. De esta manera, se pretende
contribuir a la reducción de la deserción escolar y al fortalecimiento de la equidad en el acceso a
la educación en Colombia.


## 5

-      Identificación y planteamiento del problema

La deserción escolar es un fenómeno complejo y multifactorial que trasciende las aulas,
afectando directamente el desarrollo integral, la formación de capital humano, la movilidad social
y la equidad en Colombia (Ministerio de Educación Nacional, 2022).En la última década, las
cifras de abandono han mostrado variaciones significativas: la tasa de deserción interanual en el
sector oficial descendió del 4,80 % en 2010 al 2,37 % en 2020, pero repuntó hasta el 3,58 % en
2021 debido a los efectos de la pandemia por COVID-19 (Ministerio de Educación Nacional,
2022). Para 2022, el panorama se agudizó, alcanzando una tasa nacional del 4,11 %, con una
brecha de equidad de 1,55 puntos porcentuales entre instituciones oficiales y no oficiales (Verbel
et al., 2024)
La literatura académica confirma que la interrupción de la trayectoria educativa responde
a la convergencia de factores de orden socioeconómico, demográfico y de salud pública (Guzmán
Rincón et al., 2021). En particular, la pobreza y la necesidad de trabajar son impulsores
sistemáticos del abandono escolar, mientras que los problemas de salud —crónicos o
recurrentes— afectan la asistencia y el rendimiento académico (Ministerio de Educación
## Nacional, 2022).
Este proyecto aporta a la comprensión de la deserción escolar desde un enfoque territorial
y temporal, evitando la falacia ecológica de atribuir comportamientos individuales a partir de
datos agregados (Robinson, 1950). Al estimar tasas departamentales de deserción escolar, se
busca generar evidencia que fortalezca las políticas públicas de permanencia. Además, el estudio
dialoga directamente con los Objetivos de Desarrollo Sostenible (ODS): el ODS 4 (Educación de
Calidad), al contribuir a la reducción del abandono escolar, y el ODS 3 (Salud y Bienestar), al

## 6

integrar indicadores epidemiológicos como predictores de la continuidad educativa (Moran, s. f.-
a, s. f.-b).
"En Colombia, como lo señala el (Ministerio de Educación Nacional, 2022), a pesar de
los esfuerzos gubernamentales por ampliar la cobertura, persisten altas tasas de abandono escolar,
especialmente en la transición de primaria a secundaria. Además, reportes recientes del  (Ruiz &
Navia, 2025), evidencian que la pérdida de estudiantes al llegar a la educación media sigue
siendo crítica.
El problema central radica en la brecha de integración analítica entre el sector educativo al
proponer que el riesgo de abandono no es solo un fenómeno individual, sino un comportamiento
territorial influenciado por la carga de morbilidad local y la precariedad económica agregada a
condiciones de salud, condiciones socioeconómicas y condiciones demográficas. Actualmente,
los datos del Sistema de Vigilancia en Salud Pública, estadísticas de matrícula del Ministerio de
Educación y DANE se analizan en silos independientes. Esta falta de correlación impide
identificar de manera proactiva cómo, cuándo y cuáles factores específicos actúan como
catalizadores directos del abandono escolar, limitando la capacidad del Estado para generar
alertas tempranas conjuntas.
Esta desconexión impide observar cómo la carga de morbilidad local y la precariedad
económica agregada actúan como presiones estructurales sobre el sistema educativo
departamental (Ruiz & Navia, 2025). Al no existir un modelo de evaluación territorial conjunto,
se limita la capacidad del Estado para generar políticas públicas focalizadas que mitiguen el
impacto de las condiciones de salud y pobreza sobre las tasas agregadas de deserción escolar.




## 7



2.1 Formulación o Pregunta de Investigación
¿De qué manera factores como la incidencia de enfermedades reportadas en el sistema de
vigilancia de salud pública, condiciones socioeconómicas y condiciones demográficas influyó en
las tasas de deserción escolar en los niveles de educación básica y media en Colombia durante el
periodo 2018-2024?













## 8

## 3. Objetivos
3.1 Objetivo general
Desarrollar  y  evaluar  un  modelo  de  aprendizaje  automático  para  estimar  la  tasa  anual  de
deserción  escolar  en  los  departamentos  de  Colombia  durante  el  periodo  2018–2024,  integrando
información educativa, epidemiológica, socioeconómica y demográfica mediante una arquitectura
Medallion en Databricks.
3.2 Objetivos específicos
- Preprocesar los conjuntos de datos del Ministerio de Educación Nacional (MEN),
Terridata y el portal de Datos de Vigilancia en Salud Pública (SIVIGILA), consolidando
una base de datos unificada exclusivamente a nivel departamental para el periodo de
estudio.
- Identificar las variables epidemiológicas con mayor correlación estadística respecto a los
picos históricos de deserción escolar en la transición de la educación primaria a la
secundaria.
- Entrenar diferentes algoritmos de predicción (como Regresión Logística, Random Forest
o XGBoost) para pronosticar el comportamiento de la deserción escolar basándose en el
panorama de salud pública de una región específica.
- Examinar la interacción entre los perfiles epidemiológicos territoriales (enfermedades
infecciosas vs. nutricionales) y los índices de pobreza departamental frente a la deserción
escolar.



## 9


## 4. Justificación

El impacto multidimensional de la deserción escolar en Colombia
La deserción escolar es un fenómeno complejo y multifactorial que trasciende las aulas,
afectando directamente el desarrollo integral, la formación de capital humano, la movilidad social
y la equidad en Colombia (Ministerio de Educación Nacional, 2022). A lo largo de la última
década, las cifras de abandono han fluctuado significativamente; por ejemplo, la tasa de deserción
interanual en el sector oficial descendió del 4,80 % en 2010 al 2,37 % en 2020, pero experimentó
un repunte crítico hasta el 3,58 % en 2021 debido a los profundos efectos de la pandemia por
COVID-19.(Ministerio de Educación Nacional, 2022).
Para el año 2022, el panorama se agudizó, alcanzando una tasa de deserción nacional del
4,11%, evidenciando además una alarmante brecha de equidad de 1,55 puntos porcentuales,
donde las instituciones educativas oficiales reportaron un 4,37 % de abandono frente al 2,82 %
del sector no oficial (Procuraduría General de la Nación)(Verbel et al., 2024).
La convergencia de factores de salud, socioeconómicos y demográficos, La literatura
académica y los diagnósticos territoriales confirman que la interrupción de la trayectoria
educativa responde a la convergencia de variables de orden individual, familiar, escolar y
contextual (Ministerio de Educación Nacional, 2022). Entre estas variables, la pobreza, la falta de
recursos económicos en los hogares y la necesidad de trabajar destacan sistemáticamente como
principales impulsores de la salida del sistema educativo (Ministerio de Educación Nacional,
2022; Verbel et al., 2024).
Asimismo, la salud pública y el bienestar físico y mental han demostrado ser determinantes
silenciosos pero críticos. A través de mesas consultivas regionales en Colombia, los "problemas

## 10

de salud" son recurrentemente identificados por la comunidad educativa como causas directas del
abandono escolar a nivel personal y contextual (Ministerio de Educación Nacional, 2022). Desde
la perspectiva demográfica, el riesgo se concentra fuertemente en la transición de la educación
primaria a la secundaria; históricamente, la deserción es mayor en la básica secundaria,
presentándose picos críticos en el grado sexto, lo que afecta directamente a la población de niños
y adolescentes tempranos (Ministerio de Educación Nacional, 2022).
En síntesis, este proyecto no solo aporta a la comprensión de la deserción escolar en
Colombia desde un enfoque territorial, sino que también dialoga directamente con los Objetivos
de Desarrollo Sostenible. Por un lado, se conecta con el ODS 4 (Educación de Calidad), al buscar
reducir las tasas de abandono escolar y promover la permanencia en la educación básica y media.
Por otro lado, se vincula con el ODS 3 (Salud y Bienestar), al integrar indicadores
epidemiológicos como predictores de la deserción, reconociendo que la salud pública es un factor
determinante en la continuidad educativa. De esta manera, la analítica de datos se convierte en
una herramienta estratégica para abordar problemas estructurales de gran escala, ofreciendo
evidencia que puede orientar políticas públicas más inclusivas y sostenibles.(Moran, s. f.-a)
La necesidad de innovación analítica y modelos predictivos
A pesar de que el Estado colombiano ha implementado herramientas tecnológicas valiosas
como el Sistema de Información para el Monitoreo, la Prevención y el Análisis de la Deserción
Escolar (SIMPADE) para calcular el riesgo de abandono (Verbel et al., 2024) , los expertos
coinciden en la imperiosa necesidad de crear modelos estadísticos predictivos más robustos que
brinden alertas tempranas eficaces (Ministerio de Educación Nacional, 2022). Para lograr esto, se
ha recomendado explícitamente complementar los sistemas de información educativa con bases
de datos externas provenientes de otros sectores, como la salud y el trabajo, con el fin de
perfeccionar los análisis predictivos (Ministerio de Educación Nacional, 2022).

## 11


El valor aportado por este proyecto de grado
Es en este contexto donde radica la innovación y pertinencia de la presente investigación.
El desarrollo de un modelo predictivo basado en algoritmos de aprendizaje automático (tales
como Regresión Logística, Random Forest y XGBoost) permitirá unificar y explotar el valor
latente en las bases de datos del SIVIGILA y Terridata. Al correlacionar directamente las
incidencias epidemiológicas, los niveles de pobreza y la edad poblacional con las bases históricas
de deserción (2018-2024), el proyecto trascenderá el análisis descriptivo tradicional.
Esta solución de analítica avanzada permitirá cuantificar el peso real que tiene el
ecosistema de salud pública regional sobre el abandono de las aulas, proporcionando a los
tomadores de decisiones gubernamentales una herramienta basada en evidencia para anticipar las
tasas de deserción escolar a nivel departamental. De este modo, se aporta directamente a la
mitigación de una problemática que, tan solo en 2022, superó la media nacional de deserción
escolar en 41 Entidades Territoriales Certificadas (ETC) del país (Verbel et al., 2024).

- Marco de Referencia
La deserción escolar en Colombia representa un hito para el sistema educativo no solo a
nivel nacional, sino también a nivel internacional. Incrementando su criticidad al combinarse con
factores socioeconómicos, demográficos, culturales, políticos y de condiciones de salud; lo que
limita el desarrollo y avance en diversos campos en lo que la educación como pilar juega un
papel importante.
Teniendo en cuenta el abrupto incremento en el índice de deserción escolar presentado a
nivel global dado en el marco de la pandemia presentada por COVID-19, se ha visto la necesidad
de estudiar mucho más a fondo la causalidad y los diferentes factores que pueden influir de

## 12

manera directa o indirecta en la deserción escolar, teniendo en cuenta los contextos presentados
en cada región, entendiendo que las causas estructurales de la deserción escolar no se pueden
generalizar o sesgar a un solo contexto homogéneo, debido a que en cada región, distrito o
departamento se presentan contextos o condiciones totalmente diferentes.
Así las cosas, surge la necesidad de incorporar perspectivas o estudios de diversos autores
con relación a la deserción escolar a nivel internacional, nacional y regional; buscando con esto
integrar una visión más amplia de los factores que inciden en la materialización de la deserción
escolar, marcando una hoja de ruta marcada para la toma de decisiones o implementación de
planes de acción que permitan disminuir la deserción escolar en Colombia.

Antecedentes internacionales:
La deserción en estudios de posgrado es un fenómeno creciente en América Latina que
también afecta a la Universidad Técnica de Manabí, un entorno donde resulta prioritario
identificar los factores que influyen en el abandono. El problema central identificado en esta
situación radica en el abandono de los estudiantes de posgrado debido a causas socioeconómicas
y personales, lo cual limita de manera drástica la culminación de sus programas académicos. Para
abordar esta problemática, en la investigación de (Solís Ventura et al., 2022) se aplicó un enfoque
cuantitativo mediante un modelo de regresión logística binaria con datos recolectados de 729
estudiantes. Los resultados principales muestran que el modelo logró una alta precisión en la
predicción de la deserción, alcanzando un 98,6% en la muestra piloto y un 99,06% en la fase de
validación; asimismo, se identificó que el estado civil, la situación laboral, la edad y el salario son
los factores más significativos que inciden en la decisión de abandonar los estudios.


## 13

En el contexto indonesio, la educación ha sido reconocida como un eje fundamental para el
desarrollo económico y social. A pesar de que el gobierno destina al menos el 20% del
presupuesto nacional a este sector, aún persisten dificultades para garantizar el acceso equitativo,
especialmente en regiones remotas y con condiciones económicas desfavorables, lo que ha
generado preocupación por las tasas de participación y deserción escolar en el nivel secundario.
El problema central identificado en la investigación de (Budi Suharto et al., 2025) radica en que,
aunque el gasto educativo ha aumentado de manera sostenida, las tasas de participación escolar
muestran descensos en ciertos grupos de edad. Esto evidencia que la inversión en educación, por
sí sola, no asegura la permanencia de los estudiantes, ya que factores económicos y de salud
también inciden en la decisión de continuar o abandonar los estudios. Para abordar esta
problemática, los autores emplearon un enfoque cuantitativo explicativo, utilizando modelos de
ecuaciones estructurales (SEM) con análisis de rutas basado en datos secundarios de 34
provincias de Indonesia, recopilados entre 2014 y 2023 (considerandos variables como gastos,
PIB per cápita y ratios educativas). Los resultados principales muestran que el gasto en educación
incrementa significativamente las tasas de graduación, aunque no tiene un efecto directo sobre la
participación escolar. En contraste, el gasto en salud afecta negativamente las tasas de
graduación. Asimismo, el PIB per cápita y la relación estudiante-docente contribuyen a reducir la
deserción, mientras que la relación estudiante-clase mejora las tasas de graduación, confirmando
la complejidad de los factores que impactan la participación escolar.

En el contexto de Luanda, Angola, el embarazo a temprana edad representa un desafío
crítico de salud y bienestar social, tal como se evidencia en la población de pacientes atendidas en
el Hospital Central de Maternidad (Lucrecia Paím) durante el año 2020. El problema central
abordado en la investigación de (Quinto, 2020), radica en las severas repercusiones del embarazo

## 14

adolescente, una situación que frecuentemente deriva en matrimonios precoces —generalmente
obligados por factores culturales— y que genera un déficit económico, limitando drásticamente el
desarrollo personal y la calidad de vida de las jóvenes. Para estudiar el perfil epidemiológico de
este grupo y abordar dicha problemática, se empleó una metodología mixta (cuantitativa y
cualitativa) con un diseño descriptivo, transversal y observacional, la cual consistió en la
aplicación de un cuestionario a una muestra representativa de 758 adolescentes gestantes. Los
resultados principales revelaron que la deserción escolar es la consecuencia más grave y directa
del embarazo adolescente, ya que este grupo demográfico se ve forzado a abandonar sus estudios
para dedicarse prematuramente a la familia, estancando así su desarrollo educativo.Antecedentes
nacionales:
Durante la pandemia por COVID-19 en 2020, la Escuela Normal Superior de Cartagena de
Indias enfrentó un contexto crítico marcado por un aumento del ausentismo y el riesgo de
deserción escolar en estudiantes de preescolar, primaria y secundaria. El problema principal de
este escenario radicó en que las múltiples dificultades socioeconómicas, familiares y académicas
derivadas del confinamiento y la abrupta transición a la modalidad virtual generaron altos índices
de inasistencia y abandono escolar. Para abordar y comprender esta problemática, la metodología
empleada consistió en una investigación diagnóstica de carácter mixto, la cual incluyó la
aplicación de encuestas, entrevistas y el análisis riguroso de documentos institucionales. Los
resultados principales evidenciaron que las condiciones sociales, económicas y psicosociales —
tales como los bajos ingresos familiares, las limitaciones tecnológicas y diversas afectaciones
emocionales— fueron determinantes directos en el ausentismo y la deserción, un hallazgo que
permitió finalmente proponer estrategias de intervención integral desde el área de trabajo social
(Andrea & Margarita, 2022).


## 15

En un estudio realizado para determinar las causas que conllevan a la deserción escolar,
mediante la aplicación de fuentes primarias de información, con el fin de proponer la
implementación de un plan de acción que disminuya la deserción escolar en la Institución
Educativa Don Alonso Patía, de la Vereda Don Alonso Patía, de Cauca, en el año 2022 - 2023.
Llegó a la conclusión que entre las razones principales para que un estudiante abandone los
estudio, se encuentran las dificultades de acceso, la condición socioeconómica de la familia, la
falta de oportunidades para dar continuidad al estudio y el abandono gubernamental del
corregimiento. Además, manifiesta que los padres de familia no cumplen con su rol de manifestar
afecto emocional, por lo que los estudiantes no sienten el apoyo necesario para continuar con sus
actividades académicas, quienes les avalan a sus hijos el hecho de dejar sus estudios para
centrarse en actividades laborales para devengar dinero. (Gómez Martínez, 2023)
En Colombia, las poblaciones rurales han enfrentado históricamente profundas
desigualdades derivadas del conflicto armado, el narcotráfico, la corrupción y el limitado acceso
a la tierra, condiciones que han generado altos índices de pobreza y exclusión social, llevando al
Estado a considerar la educación superior como un eje estratégico para la transformación y el
cumplimiento de la Agenda 2030. El problema central identificado en la investigación de
(Guzmán Rincón et al., 2021), es la elevada tasa de deserción en programas de educación
superior virtual dirigidos a estudiantes rurales, ya que, a pesar de las políticas públicas
implementadas para ampliar el acceso (como becas y créditos condonables), cerca del 50%
abandona sus estudios. Esto evidencia que el acceso por sí solo no garantiza la permanencia, pues
existen diversos factores que inciden en el abandono. Para analizar esta problemática, la
metodología empleada consistió en un estudio exploratorio, cuantitativo y transversal con una
muestra de 291 estudiantes rurales matriculados en programas virtuales de Bogotá entre 2018 y

## 16

2020, aplicando instrumentos de caracterización e implementando análisis factoriales
exploratorios, de conglomerados jerárquicos y estadística descriptiva. Los resultados principales
mostraron que las variables académicas no tienen un impacto significativo en la deserción; en
cambio, factores como la edad, el estado civil, las obligaciones familiares, el estrato
socioeconómico, el nivel educativo de los padres, la situación laboral y el número de
dependientes económicos influyen directamente en la probabilidad de abandono, lo que sugiere
que la deserción en estos contextos está más asociada a condiciones socioeconómicas y
personales que al desempeño académico.
## Marco Teórico
El análisis para predicción del índice de deserción escolar en Colombia entre (2018- 2024)
basado en indicadores de salud pública requiere de una base teórica solida  que permita la
integración de  las variables socioeconómicas y demográficas involucradas en este fenómeno, por
esta razón este estudio se fundamenta en dos enfoques fundamentales,  Teoría de la Reproducción
Social de Bourdieu (1977) ,  Modelo de Integración Académica y Social de Tinto (1975, 1993).
La teoría de la reproducción social de Bourdieu (1977)
Plantea que las desigualdades educativas se explican por la transmisión del capital cultural
y social entre generaciones. En contextos rurales, los estudiantes suelen tener un acceso limitado
a recursos culturales y académicos, lo que se traduce en desventajas acumuladas frente a sus
pares urbanos. Esta teoría ayuda a entender cómo las condiciones estructurales de origen influyen
en la probabilidad de abandono escolar.(Bourdieu, 1977).


## 17

Modelo de Integración Académica y Social de Tinto (1975, 1993)
Sostiene que la permanencia en la educación superior depende de la capacidad del
estudiante para integrarse tanto en el ámbito académico como en el social. En la modalidad
virtual, esta integración se ve afectada por la distancia física y la falta de interacción directa con
docentes y compañeros, lo que puede generar aislamiento y aumentar el riesgo de deserción. El
modelo de Tinto resulta especialmente útil para identificar variables institucionales y sociales que
deben fortalecerse para garantizar la continuidad educativa.(Tinto, 1994).
En conjunto, Estas dos teorías se enlazan lo que permite construir un marco completo e
integral, estos dos enfoques ofrecen un marco teórico integral que articula las dimensiones
sociales, institucionales y psicológicas de la deserción escolar en zonas rurales de Colombia.
Además, proporcionan bases sólidas para el desarrollo de modelos predictivos que permitan
identificar factores de riesgo y orientar políticas públicas más efectivas.












## 18

## Marco Conceptual
En este proyecto se determinan las siguientes definiciones claves:
➢ Salud Publica: Hace referencia al conjunto de acciones y políticas orientadas a prevenir
enfermedades, promover el bienestar y garantizar el acceso equitativo a servicios de
salud. En el contexto educativo, las condiciones de salud de los estudiantes influyen
directamente en su asistencia y rendimiento académico.(Ruiz & Navia, 2025)
➢ Indicadores Epidemiológicos: Son variables estadísticas que permiten medir la incidencia
y prevalencia de enfermedades en una población. En este proyecto, se consideran como
factores explicativos de la deserción escolar, dado que problemas de salud recurrentes
pueden limitar la continuidad educativa. (Solís Ventura et al., 2022)
➢ Deserción Escolar: Se entiende como el abandono definitivo del sistema educativo por
parte de un estudiante antes de culminar el nivel en el que se encuentra matriculado. Este
fenómeno afecta el desarrollo personal, la movilidad social y el capital humano del
país.(Ministerio de Educación Nacional, 2022).
➢ Condiciones socioeconómicas: Engloban aspectos como el nivel de ingresos, empleo y
acceso a recursos básicos de los hogares. La pobreza y la necesidad de trabajar son
factores que incrementan el riesgo de abandono escolar. (Verbel et al., 2024).
➢ Factores demográficos: Se refieren a características poblacionales como edad, sexo y
lugar de residencia. En Colombia, la edad es un factor crítico, especialmente en la
transición de primaria a secundaria, donde se concentran los mayores índices de deserción
(Ministerio de Educación Nacional, 2022).
➢ Aprendizaje automático (Machine Learning): Es una rama de la inteligencia artificial que
utiliza algoritmos para identificar patrones en grandes volúmenes de datos y realizar
predicciones. En este proyecto, se emplean modelos como regresión logística, Random

## 19

Forest y XGBoost para estimar la probabilidad de deserción escolar.(Solís Ventura et al.,
## 2022).
## Marco Contextual
La deserción escolar en Colombia es un problema multifactorial que afecta principalmente
a los niveles de educación básica y media. Este fenómeno se relaciona con condiciones
socioeconómicas, demográficas y de salud pública que limitan la permanencia de los estudiantes
en el sistema educativo. La pandemia por COVID-19 evidenció la fragilidad del sistema, pues la
tasa de deserción nacional pasó de 2,37 % en 2020 a 3,58 % en 2021, mostrando cómo las crisis
sanitarias impactan directamente la continuidad escolar. (Ministerio de Educación Nacional,
## 2022).
La necesidad de este proyecto radica en que, aunque existen sistemas de información como
el SIMPADE, aún no se integran de manera suficiente los datos de salud pública con los
educativos. Estudios recientes han demostrado que problemas de salud, pobreza y desigualdad
territorial son factores recurrentes en el abandono escolar (Ruiz & Navia, 2025). Por ello, un
modelo predictivo que correlacione indicadores epidemiológicos y socioeconómicos puede
aportar evidencia sólida para diseñar políticas públicas más efectivas.
El proyecto se centra en el periodo 2018-2024 y en los niveles de educación básica y media
en Colombia. Se consideran variables epidemiológicas provenientes del Sistema de Vigilancia en
Salud Pública (SIVIGILA), junto con indicadores socioeconómicos y demográficos de Terridata.
El análisis se focaliza en la transición de primaria a secundaria, etapa crítica donde se concentran
los mayores índices de abandono (Ministerio de Educación Nacional, 2022).
La investigación se apoya en técnicas de aprendizaje automático, como regresión logística,
Random Forest y XGBoost, para identificar patrones y estimar la probabilidad de deserción
escolar. Este enfoque metodológico permite analizar grandes volúmenes de datos y generar

## 20

modelos predictivos que integren variables de salud, economía y demografía. (Solís Ventura
et al., 2022).
El marco contextual ofrece una visión integral que articula el fenómeno de la deserción
escolar con sus causas estructurales y coyunturales. Al vincular datos de salud pública con
información educativa, se facilita la interpretación de los resultados y se justifica la pertinencia
del modelo predictivo. De esta manera, los hallazgos podrán ser comprendidos en relación con el
entorno social y sanitario del país, fortaleciendo la toma de decisiones en política educativa.
(Verbel et al., 2024).
Este panorama contextual evidencia que la deserción escolar es un fenómeno multifactorial
que requiere un abordaje integral. En el caso colombiano, la articulación entre educación y salud
pública se convierte en un eje central para comprender y anticipar el riesgo de abandono. Por
ello, el presente proyecto se inscribe en este contexto, proponiendo un modelo predictivo basado
en aprendizaje automático que permita correlacionar indicadores epidemiológicos,
socioeconómicos y demográficos con las tasas de deserción escolar entre 2018 y 2024.

## Marco Legal
El marco normativo de este proyecto se apoya en las leyes y políticas que garantizan el
derecho a la educación en Colombia y en los compromisos internacionales que promueven la
equidad. En el caso colombiano, la Constitución establece que la educación es un derecho
fundamental y un servicio público obligatorio entre los 5 y los 15 años
(Constitución_Política_1_de_1991_Asamblea_Nacional_Constituyente, s. f.). Además, normas
como la Ley General de Educación (Ley 115 de 1994) y la Ley 1620 de 2013 refuerzan la
obligación del Estado de asegurar la permanencia escolar y prevenir la deserción.

## 21

A nivel de políticas públicas, el Ministerio de Educación ha implementado estrategias como
el SIMPADE y los Modelos Educativos Flexibles, que buscan identificar riesgos y ofrecer
alternativas para que los estudiantes permanezcan en el sistema (Ministerio de Educación
## Nacional, 2022).
En el plano internacional, instrumentos como la Declaración Universal de los Derechos
Humanos (ONU, 1948, art. 26) y el Pacto Internacional de Derechos Económicos, Sociales y
Culturales (ONU, 1966, art. 13) reconocen la educación como un derecho universal y obligatorio
en la enseñanza básica. Asimismo, el Objetivo de Desarrollo Sostenible 4 de la ONU insiste en
garantizar una educación inclusiva y de calidad.
Finalmente, este proyecto se sustenta también en la normativa sobre datos abiertos y
transparencia, como la Ley 1712 de 2014 y el Decreto 103 de 2015, que permiten acceder y
utilizar información pública en formatos abiertos. Esto legitima el uso de bases de datos oficiales
como SIVIGILA y Terridata para construir modelos predictivos que anticipen la deserción
escolar.
## Normativa Nacional
- Constitución Política de Colombia (1991): Reconoce la educación como un derecho
fundamental y un servicio público que debe garantizarse con calidad y cobertura, El articulo 44
reconoce la educación como un derecho fundamental de los niños, junto con la salud, la
alimentación y la seguridad social. Establece que la familia, la sociedad y el Estado tienen la
obligación de proteger estos derechos.
- Ley 1620 de 2013: Crea el Sistema Nacional de Convivencia Escolar y Formación para el
Ejercicio de los Derechos Humanos, la Educación para la Sexualidad y la Prevención y
Mitigación de la Violencia Escolar.

## 22

- Decreto 1965 de 2013: Reglamenta la Ley 1620 y establece lineamientos para la
prevención de la deserción escolar.
- SIMPADE (Sistema de Información para el Monitoreo, la Prevención y el Análisis de la
Deserción Escolar): Herramienta oficial del Ministerio de Educación para calcular y analizar el
riesgo de abandono escolar.
## Políticas Públicas Relevantes
- Estrategias de Permanencia Escolar del MEN: Incluyen modelos educativos flexibles,
residencias escolares y programas de jornada complementaria para garantizar la permanencia de
niños y adolescentes en el sistema educativo.
- Programas de Inclusión Educativa: Orientaciones para promover el bienestar y la
permanencia de estudiantes con discapacidad en el marco de la educación inclusiva
- Políticas de Equidad Territorial: Acciones para reducir las brechas entre zonas rurales y
urbanas en acceso y permanencia escolar.
## Normativa Internacional
Declaración Universal de los Derechos Humanos (1948): Artículo 26 establece que toda
persona tiene derecho a la educación gratuita en la instrucción elemental.
Pacto Internacional de Derechos Económicos, Sociales y Culturales (1966): Artículo 13
reconoce la obligatoriedad de la enseñanza primaria y la necesidad de accesibilidad en niveles
superiores.
UNESCO – Instrumentos Jurídicos Internacionales: Convenciones y recomendaciones que
orientan a los Estados en la garantía del derecho a la educación.
Objetivo de Desarrollo Sostenible 4 (ONU): Garantizar una educación inclusiva, equitativa
y de calidad, promoviendo oportunidades de aprendizaje durante toda la vida.


## 23

Normativa sobre Datos Abiertos y Transparencia
Ley 1712 de 2014: Ley de Transparencia y del Derecho de Acceso a la Información Pública
Nacional. Define los datos abiertos como información pública disponible en formatos estándar e
interoperables para su libre uso.
Política de Datos Abiertos (MINTIC): Promueve la publicación y reutilización de datos
públicos para investigación y toma de decisiones.
Portal Datos Abiertos Colombia: Plataforma oficial que centraliza bases de datos
gubernamentales para consulta y análisis.

- Metodología CRISP-DM
En esta sección se detalla todo el paso a paso llevado para el presente proyecto “Modelo de
aprendizaje automático para predicción del índice de deserción escolar en Colombia entre 2018 a
2024 basado en indicadores de salud pública”. La elección de la metodología CRISP-DM (Cross
Industry Standard Process for Data Mining) responde a la necesidad de estructurar de manera
clara y sistemática el proceso de análisis de datos, desde la comprensión del problema hasta la
implementación de modelos predictivos.
La conexión con los antecedentes es fundamental: a nivel nacional, investigaciones como
las de (Gómez-Restrepo et al., 2016) y (Guzmán Rincón et al., 2021) han mostrado que la
deserción escolar en contextos rurales y virtuales está fuertemente asociada a factores
socioeconómicos y familiares, más que al desempeño académico. A nivel internacional, estudios
como el de (Budi Suharto et al., 2025) en Indonesia evidencian que el gasto en educación por sí
solo no garantiza la permanencia, y que variables como el PIB per cápita y la relación estudiante-
docente influyen directamente en la deserción. Estos hallazgos justifican la necesidad de un

## 24

modelo predictivo que integre datos de salud pública, demografía y economía para anticipar
riesgos de abandono escolar en Colombia.
Fases de CRISP-DM aplicadas al proyecto
I. Comprensión del negocio
El proyecto busca estimar la tasa de deserción escolar en Colombia entre 2018 y 2024, a
nivel  departamental, integrando indicadores de salud pública (SIVIGILA), demográficos y
socioeconómicos (Terridata/DANE). La deserción escolar es un problema estructural que afecta
la equidad educativa y se relaciona con factores de salud y pobreza. (Ministerio de Educación
Nacional, 2022) (Guzmán Rincón et al., 2021)
II. Comprensión de los datos
Se identifican y analizan las fuentes de información:
- SIVIGILA: reportes de incidencia de enfermedades.
- Terridata/DANE: indicadores socioeconómicos y demográficos.
- Registros de matrícula del MEN: tasas de deserción y cobertura educativa.
Se  evalúa  la  calidad  de  los  datos,  la  granularidad  temporal  y  espacial,  y  la  consistencia  entre
fuentes. Se identifican valores faltantes y se documenta la correlación espacial y temporal.(Budi
Suharto et al., 2025)
III. Preparación de los datos
La preparación de los datos se orquestará utilizando una Arquitectura Medallion en la
plataforma Databricks:

## 25

- Capa Bronce (Raw): Almacenamiento de los archivos crudos (.csv) extraídos del portal
de Datos Abiertos para SIVIGILA, Terridata y MEN, sin alteraciones.
- Capa Plata (Cleansed): Limpieza de datos, normalización de los códigos DIVIPOLA
departamentales, tratamiento de valores nulos y estandarización del periodo (2018-2024).
- Capa Oro (Curated): Consolidación de la tabla maestra analítica (Feature Store)
estructurada en la unidad de análisis Departamento-Año, lista para el consumo de los
algoritmos de Machine Learning.
Este paso responde al objetivo específico de Preprocesar los conjuntos de datos.
IV. Modelado

El modelado se centra en regresión de tasas de deserción escolar territorial:
- Baseline: regresión lineal múltiple.
- Modelos  avanzados: Random  Forest,  Gradient  Boosting  Machines  (GBM),  XGBoost  y
LightGBM.
- Ingeniería  de  características: creación  de  variables  temporales  (lag  de  enfermedades),
interacción entre pobreza y ruralidad.
- Interpretabilidad: uso de SHAP para explicar la contribución de cada variable (Lundberg
## & Lee, 2017)
- Validación: validación cruzada espaciotemporal para evitar autocorrelación (Valavi et al.,
## 2019)
El modelado busca cumplir el objetivo de pronosticar el comportamiento de la deserción escolar
basándose en el panorama de salud pública.(Solís Ventura et al., 2022)
## V. Evaluación
Se aplican métricas de regresión:
- RMSE (Raíz del Error Cuadrático Medio).

## 26

- MAE (Error Absoluto Medio).
- R² (Coeficiente de Determinación).
Además, se comparan resultados por subgrupos territoriales (rural vs urbano, alta vs baja
pobreza). (Valavi et al., 2019).
VI. Implementación
Los resultados se presentan en:
- Mapas de predicciones por departamento.
- Mapas de calor de errores.
- Dashboards interactivos para apoyar la toma de decisiones en política educativa.
La implementación conecta directamente con los ODS 4 (Educación de Calidad) y ODS
3 (Salud y Bienestar), mostrando cómo la analítica de datos puede contribuir a resolver problemas
estructurales de gran escala.(Moran, s. f.-b)

Protocolo de Investigación
- Técnicas investigativas
El proyecto se fundamenta en técnicas de minería de datos aplicada a fuentes
administrativas y abiertas, siguiendo la metodología CRISP-DM. Se emplean procedimientos de
extracción, transformación y carga (ETL) para consolidar información de diferentes sistemas
(SIVIGILA, Terridata, MEN). La técnica principal es el análisis predictivo de series temporales
agregadas, complementado con ingeniería de características para generar variables derivadas que
capturen relaciones entre salud pública y educación.(Chapman, 2000).

## 27


- Tipo de estudio, métodos y diseño de investigación
Tipo de estudio: Observacional, retrospectivo y longitudinal.

Método: Cuantitativo,  basado  en  análisis  macro  de  tasas  de  deserción  escolar  por  municipio  y
departamento.

Diseño: Predictivo  de  regresión,  orientado  a  estimar  índices  continuos  de  deserción  escolar,
evitando la falacia ecológica de inferir riesgos individuales (Robinson, 1950).
## 3. Enfoque Metodológico
El  enfoque  es  cuantitativo  y  computacional,  centrado  en  el  uso  de  aprendizaje  automático
para  modelar  la  deserción  escolar  como  un  fenómeno  agregado.  Se  prioriza  la  reproducibilidad
mediante prácticas básicas de MLOps (versionado de datasets, documentación de pipelines) y la
validación espaciotemporal para garantizar robustez en los resultados. (Valavi et al., 2019)
## 4. Diseño Metodológico
- Nivel de análisis: tasas de deserción escolar por municipio/departamento.

- Horizonte temporal: 2018–2024 (7 años de datos).

- Modelos: regresión  lineal  múltiple  como  línea  base;  modelos  avanzados  de
ensamble y boosting (Random Forest, XGBoost, LightGBM).


## 28

- Métricas de evaluación: RMSE, MAE y R².

## 5. Modelado Predictivo
El modelado se centra en estimar la tasa de deserción escolar territorial.
- Baseline: regresión lineal múltiple para establecer un punto de comparación.

- Modelos  avanzados:  Random  Forest,  Gradient  Boosting  Machines  (GBM),  XGBoost  y
LightGBM, que permiten capturar relaciones no lineales y jerárquicas.
- Interpretabilidad:  uso  de  SHAP  para  explicar  la  contribución  de  cada  variable  en  la
predicción (Lundberg & Lee, 2017).

## 6. Triangulación
Se realiza un análisis de heterogeneidad dividiendo resultados por contexto:
- Departamentos rurales vs. urbanos.
- Departamentos con alta vs. baja pobreza.
Esto permite comprender cómo varían las predicciones según el entorno territorial y fortalecer la
pertinencia de las recomendaciones.(Guzmán Rincón et al., 2021)

- Participantes o unidad de análisis
- Fuentes primarias: de datos (administrativos):
- Unidad primaria:  departamentos de Colombia.

## 29

- Unidades secundarias: indicadores agregados de salud pública (SIVIGILA),
socioeconómicos (Terridata/DANE) y educativos (MEN).
- Muestra cualitativa: no aplica, dado que el enfoque es exclusivamente macro y
cuantitativo.
- Técnicas e instrumentos de recolección de datos
Procedimiento ETL:
- Extracción: descarga de datos abiertos de SIVIGILA, Terridata y MEN.
- Transformación: estandarización  de  códigos  territoriales  (DANE),  normalización  de
fechas, creación de variables derivadas (ej. tasa de morbilidad anual).

- Carga: consolidación  en  una  base  relacional  con  diccionario  de  datos  y  control  de
versiones.
Instrumentos cualitativos: no se incluyen, dado que el alcance es cuantitativo y macro.
- Planificación y Viabilidad del proyecto
- Desarrollo de cronograma

## 8. Presupuesto
Este  proyecto  se  desarrolla  en  el  marco  de  una  investigación  académica,  por  lo  que  los
recursos   requeridos   son   principalmente   de   tipo   tecnológico,   bibliográfico   y   humano.   A
continuación, se detallan los rubros principales:
Recursos tecnológicos:
Se  requiere  un  computador  con  capacidad  de  procesamiento  medio-alto  para  manejar  bases  de
datos y ejecutar algoritmos de aprendizaje automático. El software utilizado será de acceso libre,

## 30

como  Python,  R  y  sus  librerías  especializadas  (Scikit-learn,  XGBoost,  LightGBM,  entre  otras).
También  se  emplearán  gestores  de  bases  de  datos  como  PostgreSQL,  igualmente  de  licencia
abierta.
Costo estimado: $0 (uso de software libre y equipo propio).

Acceso a datos:
Las fuentes de información provienen de sistemas oficiales y abiertos como SIVIGILA, Terridata,
DANE y MEN. Al ser datos públicos, no generan costos de adquisición.
Costo estimado: $0.
Bibliografía y referencias académicas:
Se  utilizarán  artículos  científicos  y  documentos  oficiales  disponibles  en  repositorios  abiertos
(Scielo, Redalyc, Google Scholar, ONU, MEN).
Costo estimado: $0.
Recursos humanos:
El trabajo será desarrollado por los estudiantes , Cristian Camilo Quintero Mejia, Angelica Mayerly
Tamayo Suarez y Jose Raul Leiva Méndez investigadores principales, con apoyo permanente del
evaluador académico de la institución. No se contempla contratación externa.
Costo estimado: $0 (dedicación académica).
Otros recursos:
Posible impresión de informes finales y anexos para la entrega física.
Costo estimado: $50.000 COP.
Total, estimado del presupuesto

## 31

El  costo  total  del  proyecto  es  mínimo,  dado  que  se  apoya  en  recursos  tecnológicos  y
bibliográficos  de  acceso  libre.  El  único  gasto  directo  previsto  corresponde  a  la  impresión  de
documentos, con un valor aproximado de $50.000 COP.
- Consideraciones éticas, de gobernanza de datos y reproducibilidad
Ética y protección de datos. Manejo de datos personales conforme a la normativa
colombiana (Ley 1581 de 2012 y decretos reglamentarios) y principios de minimización:
anonimización/pseudonimización de registros individuales, almacenamiento seguro y control de
accesos. Solicitud de autorizaciones institucionales si se requiere acceso a datos no públicos.
Transparencia y reproducibilidad. Documentación completa del pipeline ETL, scripts de
análisis (control de versiones en Git), diccionario de variables y notebook reproducible con
ejemplos de ejecución. Entregables: dataset anonimizado (si es posible), código y manual de uso.
Limitaciones esperadas. Calidad y cobertura de datos en municipios remotos; sesgo por
subregistro en SIVIGILA; cambios en definiciones administrativas a lo largo del periodo 2018–
- Estas limitaciones se abordarán con análisis de sensibilidad y documentación explícita.
- Instrumentos y Recolección de información
## Sivigila
Elementos Descripción del dataset
Fuente Sistema nacional de vigilancia en salud publica
Unidad de análisis Evento Epidemiológico
## Periodo 2018-2024
Variable Objetivo Nombre del Evento
Variables Predictoras Semana epidemiológica, departamento, año.
Formato csv
## Registros 3.056.235
Problemas Iniciales Desagregación de la información, formato incorrecto,
datos nulos, valores especiales.
Tratamiento Ético N/A




## 32





## Terridata
Elementos Descripción del dataset
Fuente DNP-Terridata
Unidad de análisis Pobreza
## Periodo 2018-2024
Variable Objetivo Índice de pobreza
Variables Predictoras Departamento, año, mes
## Formato Csv
## Registros 47.771
Problemas Iniciales Periodo de la información
Tratamiento Ético N/A

Ministerio de Educación
Elementos Descripción del dataset
Fuente Ministerio de Educación
Unidad de análisis Tasas de deserción
## Periodo 2018-2024
## Variable Objetivo Deserción Escolar
Variables Predictoras Departamento, año.
## Formato Csv
## Registros 7.853
Problemas Iniciales Periodo de la información
Tratamiento Ético N/A

- Diagnostico Inicial de los datasets
## Sivigila
Fuentes de los Datos Sistema nacional de vigilancia en salud publica
Numero de Registros 3.056.235
Numero de Variables 8 variables
Periodo de los Datos 2018-2024
Unidad de Análisis Evento Epidemiológico
Variable Objetivo, si aplica Nombre del Evento
Variables Principales Semana epidemiológica, departamento, año.
## Datos Faltantes 0
## Duplicados
Valores atípicos/ inconsistencias
¿los datos permiten responder los objetivos? Si
Próximo tratamiento que realizaré EDA (Análisis exploratorio de los datos),
ETL(Extracción, Transformación y carga de los datos)



## 33





## Terridata
Fuentes de los Datos DNP-Terridata
Numero de Registros 47.771
Numero de Variables 7 variables
Periodo de los Datos 2018-2024
Unidad de Análisis Pobreza
Variable Objetivo, si aplica Índice de pobreza
Variables Principales Departamento, año, mes
## Datos Faltantes
## Duplicados
Valores atípicos/ inconsistencias
¿los datos permiten responder los objetivos? Si
Próximo tratamiento que realizaré EDA (Análisis exploratorio de los datos),
ETL(Extracción, Transformación y carga de los datos)

Ministerio de Educación
Fuentes de los Datos Ministerio de Educación
Numero de Registros 7.853
Numero de Variables 4 variables
Periodo de los Datos 2018-2024
Unidad de Análisis Tasas de deserción
Variable Objetivo, si aplica Deserción Escolar
Variables Principales Departamento, año.
## Datos Faltantes
## Duplicados
Valores atípicos/ inconsistencias
¿los datos permiten responder los objetivos? Si
Próximo tratamiento que realizaré EDA (Análisis exploratorio de los datos),
ETL(Extracción, Transformación y carga de los datos)









## 34




-      Referencias bibliográficas
Ministerio   de   Educación   Nacional.   (2022). Deserción   escolar   en   Colombia:   Análisis,
determinantes y política de acogida, bienestar y permanencia.
https://www.mineducacion.gov.co/1780/articles-363488_recurso_34.pdf
Observatorio  de  Realidades  Educativas.  (2025). Informe  cobertura  y  abandono  escolar  en
educación    media    en    Colombia. Universidad     Icesi. https://www.icesi.edu.co/wp-
content/uploads/2025/09/informe-cobertura-y-abandono-escolar-en-educacion-media-
agosto-2025-1.pdf
Andrea, P. C. M., & Margarita, B. T. M. (2022). Condiciones sociales, económicas y académicas
relacionadas  con  el  ausentismo  estudiantil  en  los  estudiantes  de  prescolar,  primaria  y
básica secundaria, que pertenecen a la Escuela Normal Superior de Cartagena de Indias
en el año 2020.
Bourdieu, P. (1977). Outline of a Theory of Practice (R. Nice, Trad.; 1.
a
ed.). Cambridge University
Press. https://doi.org/10.1017/CBO9780511812507
Budi  Suharto,  R.,  Hasanuddin,  H.,  Jiuhardi,  J.,  &  Lestari,  D.  (2025).  Education,  Health,  and
Economic  Factors  Affecting  Secondary  School  Participation  and  Dropout  Rates  in
Indonesia. The Es Economics and Entrepreneurship, 3(03).
https://doi.org/10.58812/esee.v3i03.479
Chapman, P. (2000). CRISP-DM 1.0: Step-by-step data mining guide.
https://www.semanticscholar.org/paper/CRISP-DM-1.0%3A-Step-by-step-data-mining-
guide-
Chapman/54bad20bbc7938991bf34f86dde0babfbd2d5a72?sort=relevance&queryString=
CRISP-DM%201.0%3A%20Step-by-
step%20data%20mining%20guide.%20SPSS%20Inc.

## 35

Constitución_Política_1_de_1991_Asamblea_Nacional_Constituyente. (s. f.).
Estrategia, Acogida , Bienestar y Permanencia. (s. f.).
Gómez Martínez, G. P. (2023). La deserción escolar en la Institución Educativa Don Alonso Patía,
de la Vereda Don Alonso Patía, de Cauca: Causas y formas de mitigación [PhD Thesis].
Universidad Autónoma de Bucaramanga UNAB.
Gómez-Restrepo, C., Padilla Muñoz, A., & Rincón, C. J. (2016). Deserción escolar de adolescentes
a partir de un estudio de corte transversal: Encuesta Nacional de Salud Mental Colombia
- Revista Colombiana de Psiquiatría, 45, 105-112.
https://doi.org/10.1016/j.rcp.2016.09.003
Guzmán Rincón, A., Barragán, S., & Cala Vitery, F. (2021). Rurality and Dropout in Virtual Higher
Education Programmes in Colombia. Sustainability, 13(9), 4953.
https://doi.org/10.3390/su13094953
Lundberg, S., & Lee, S.-I. (2017). A Unified Approach to Interpreting Model Predictions (Versión
2). arXiv. https://doi.org/10.48550/ARXIV.1705.07874
Ministerio de Educación Nacional. (2022).
Moran,  M.  (s. f.-a).  Educación. Desarrollo  Sostenible.  Recuperado  10  de  junio  de  2026,  de
https://www.un.org/sustainabledevelopment/es/education/
Moran,   M.   (s. f.-b).   Salud. Desarrollo   Sostenible.   Recuperado   10   de   junio   de   2026,   de
https://www.un.org/sustainabledevelopment/es/health/
Quinto, F. A. (2020). Perfil epidemiológico y social de las adolescentes embarazadas atendidas
en la Maternidad Lucrécia Paim en Luanda–Angola [PhD Thesis].
Robinson,  W.  S.  (1950).  Ecological  Correlations  and  the  Behavior  of  Individuals. American
Sociological Review, 15(3), 351. https://doi.org/10.2307/2087176

## 36

Ruiz, J., & Navia, S. (2025). Informe-cobertura-y-abandono-escolar-en-educacion-media-agosto-
2025-1 (No. 1; p. 14). Universidad ICESI.
Solís  Ventura,  J.  C.,  Quiroz  Fernández,  S.,  &  Fosado  Téllez,  O.  (2022).  MODELO  DE
## REGRESIÓN LOGÍSTICA PARA LA ESTIMACIÓN DE LA DESERCIÓN ESCOLAR
## DEL  POSGRADO  EN  LA  UNIVERSIDAD  TÉCNICA  DE  MANABÍ,  ECUADOR.
Revista Bases de la Ciencia, 7(3), 1-14.
https://doi.org/10.33936/revbasdelaciencia.v7i3.5197
Tinto,  V.  (1994). Leaving  College:  Rethinking  the  Causes  and  Cures  of  Student  Attrition.
University of Chicago Press. https://doi.org/10.7208/chicago/9780226922461.001.0001
Valavi, R., Elith, J., Lahoz‐Monfort, J. J., & Guillera‐Arroita, G. (2019). BLOCK CV: An R package
for generating spatially or environmentally separated folds for k ‐fold cross‐validation of
species   distribution   models. Methods   in   Ecology   and   Evolution, 10(2),   225-232.
https://doi.org/10.1111/2041-210X.13107
Verbel, V. M., Delegada, P., Ramírez, L. C. S., & González, S. L. O. (2024). Informe Seguimiento
## Deserción Escolar. Informe Seguimiento Deserción Escolar, (15).

Constitución  Política  1  de  1991  Asamblea  Nacional  Constituyente - Gestor  Normativo.  (s/f).
Gov.co. Recuperado el 2 de abril de 2026, de
https://www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=4125

https://www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=56882
Constitución Política de Colombia. (1991). Artículo 44,67, 68,69, 70.