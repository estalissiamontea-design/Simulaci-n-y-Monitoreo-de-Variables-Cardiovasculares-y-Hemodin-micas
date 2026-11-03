# Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas

Alissia Montealegre Quintero. 
Raul Alexander Peñuela Jimenez.
Silvia Lorena Vargas Rueda.

Instrumentación Biomédica y Biosensores  
Facultad de Ingeniería, Universidad Militar Nueva Granada, VII Semestre  


---

## I. Resumen
En esta práctica de laboratorio se evaluó el funcionamiento de un monitor de signos vitales Mindray uMEC 100 mediante el uso de un simulador de parámetros hemodinámicos Pronk OxSim OX-1. El propósito fue verificar la respuesta del monitor ante diferentes condiciones de frecuencia cardíaca y saturación periférica de oxígeno (SpO2), así como observar el comportamiento de las alarmas y las señales fotopletismográficas.

Se realizaron dos pruebas experimentales en las que se configuraron diferentes escenarios de simulación: bradicardia, disminución de la saturación de oxígeno, baja perfusión y taquicardia. Para cada condición se registraron los parámetros configurados en el simulador y los valores presentados en el monitor, junto con las observaciones de las señales y las alarmas.

Los resultados permitieron observar la respuesta del monitor ante diferentes condiciones simuladas y reconocer la importancia de los límites de alarma en la vigilancia de variables cardiovasculares. Asimismo, se identificó la relevancia de las condiciones de perfusión en la adquisición de la señal de oximetría de pulso.

**Palabras clave:** pulsioximetría, frecuencia cardíaca, SpO2, fotopletismografía, monitor de signos vitales, simulación hemodinámica.

---

# II. Introducción

El monitoreo de variables cardiovasculares constituye una herramienta fundamental en la atención clínica, debido a que permite observar continuamente diferentes parámetros fisiológicos relacionados con el funcionamiento del sistema circulatorio y la oxigenación del organismo. Entre las variables más utilizadas se encuentran la frecuencia cardíaca y la saturación periférica de oxígeno (SpO2), cuyos cambios pueden proporcionar información importante sobre el estado fisiológico del paciente. Los pulsioxímetros permiten estimar estos parámetros de manera no invasiva mediante la interacción de la luz con los tejidos y la sangre [1].

En los entornos hospitalarios, los monitores de signos vitales permiten visualizar estas mediciones y establecer límites de alarma para identificar situaciones que requieren atención. Sin embargo, el funcionamiento de estos equipos debe verificarse mediante procedimientos que permitan evaluar su respuesta ante diferentes condiciones de operación. La Administración de Alimentos y Medicamentos de los Estados Unidos (FDA) señala que los pulsioxímetros pueden presentar limitaciones en sus mediciones debido a factores como la circulación periférica, la temperatura de la piel y otras condiciones que afectan la calidad de la señal [1].

Para realizar este tipo de verificaciones se emplean simuladores de parámetros fisiológicos que permiten generar señales ópticas controladas y evaluar el comportamiento de los sistemas de pulsioximetría. El Pronk OxSim OX-1 es un simulador diseñado para comprobar el funcionamiento de los monitores de oximetría mediante diferentes configuraciones de saturación de oxígeno, frecuencia cardíaca e índice de perfusión [2].

En esta práctica se utilizó el simulador Pronk OxSim OX-1 junto con el monitor de signos vitales Mindray uMEC 100, con el propósito de evaluar la respuesta del monitor ante diferentes escenarios fisiológicos simulados. Se realizaron dos pruebas experimentales en las que se configuraron condiciones de bradicardia, disminución de SpO2, baja perfusión y taquicardia. Además, se modificaron los límites de alarma del monitor para observar su comportamiento ante valores que superaban los umbrales establecidos.

De esta manera, la práctica permitió relacionar los fundamentos de la pulsioximetría con el funcionamiento de los equipos biomédicos, reconociendo la importancia de verificar tanto la precisión de las mediciones como la respuesta de los sistemas de alarma.

---

# III. Marco teórico

## 3.1. Monitor de signos vitales

Un monitor de signos vitales es un equipo biomédico utilizado para adquirir, procesar y visualizar diferentes variables fisiológicas de un paciente. Dependiendo de su configuración, puede presentar parámetros como frecuencia cardíaca, frecuencia respiratoria, saturación periférica de oxígeno y presión arterial.

El monitor Mindray uMEC 100 pertenece a la serie uMEC de monitores de pacientes y permite visualizar los parámetros medidos mediante una interfaz que integra valores numéricos, formas de onda y sistemas de alarma [3].

Su funcionamiento permite al personal clínico realizar un seguimiento de las variables fisiológicas y reconocer posibles alteraciones mediante límites de alarma configurables. Estas alarmas pueden proporcionar indicaciones visuales y sonoras cuando una medición alcanza condiciones que requieren atención [3].

## 3.2. Simulador de parámetros hemodinámicos Pronk OxSim OX-1

El Pronk OxSim OX-1 es un simulador óptico de pulsioximetría utilizado para verificar el funcionamiento de monitores y sensores de SpO2. Su operación permite reproducir diferentes combinaciones de saturación de oxígeno, frecuencia cardíaca e índice de perfusión, sin necesidad de utilizar un paciente real [2].

El dispositivo cuenta con botones de selección que permiten cambiar entre los modos de simulación disponibles. Además, utiliza un sistema óptico sobre el cual se coloca el sensor de pulsioximetría del monitor que se desea evaluar [2].

Los cinco modos principales de simulación del OxSim OX-1 son:

| Modo | SpO2 | Frecuencia cardíaca | Índice de perfusión aproximado |
|---|---:|---:|---:|
| 85 % | 85 % | 80 bpm | 2.0 |
| 95 % | 95 % | 40 bpm | 2.0 |
| 98 % | 98 % | 80 bpm | 2.0 |
| 140 bpm | 98 % | 140 bpm | 2.0 |
| Low Perfusion | 99 % | 80 bpm | 0.2 |

Estos valores corresponden a las configuraciones descritas por el fabricante en el manual de operación del simulador [2].

## 3.3. Frecuencia cardíaca

La frecuencia cardíaca corresponde al número de latidos que realiza el corazón durante un minuto y se expresa en latidos por minuto (bpm). Es una variable utilizada para evaluar el comportamiento del sistema cardiovascular.

De acuerdo con las condiciones de operación del simulador OxSim OX-1, es posible reproducir diferentes frecuencias cardíacas para evaluar la respuesta del monitor. Entre estas condiciones se encuentran la bradicardia simulada a 40 bpm y la taquicardia simulada a 140 bpm [2].

La bradicardia y la taquicardia representan condiciones de frecuencia cardíaca anormalmente baja o elevada, respectivamente, cuya interpretación clínica depende del contexto del paciente.

## 3.4. Saturación periférica de oxígeno (SpO2)

La saturación periférica de oxígeno representa una estimación del porcentaje de hemoglobina que transporta oxígeno en la sangre arterial. Su medición se realiza mediante pulsioximetría, una técnica no invasiva que utiliza luz para estimar la oxigenación sanguínea [1].

Los pulsioxímetros utilizan principalmente dos longitudes de onda: luz roja e infrarroja. La hemoglobina oxigenada y la desoxigenada presentan diferentes características de absorción óptica, lo que permite estimar la saturación mediante el procesamiento de la señal recibida por el sensor [2].

La SpO2 es una variable importante para el monitoreo de pacientes, aunque su medición puede verse afectada por factores como la perfusión periférica deficiente, el movimiento, la temperatura y las características del tejido donde se ubica el sensor [1].

## 3.5. Fotopletismografía

La fotopletismografía (PPG) es una técnica óptica que permite detectar variaciones en el volumen sanguíneo de los tejidos mediante la interacción de la luz con la sangre circulante.

En los pulsioxímetros, la señal fotopletismográfica representa las variaciones pulsátiles asociadas con el flujo sanguíneo arterial. El manual del Pronk OxSim explica que la señal óptica contiene una componente pulsátil (AC), relacionada con los cambios producidos por el pulso, y una componente continua (DC), asociada con las propiedades ópticas generales del tejido [2].

La forma de onda obtenida permite observar el comportamiento de las pulsaciones y proporciona información sobre la calidad de la señal adquirida por el monitor.

## 3.6. Índice de perfusión y baja perfusión

El índice de perfusión (PI) representa la relación entre el componente pulsátil y el componente no pulsátil de la señal fotopletismográfica. Se utiliza como indicador de la intensidad de la señal pulsátil detectada por el sensor [3].

Cuando existe una perfusión periférica reducida, la amplitud de la componente pulsátil puede disminuir, dificultando la detección de la señal por parte del pulsioxímetro. Esta condición puede generar dificultades en la adquisición de la señal y afectar la estabilidad de las mediciones [1], [4].

El modo Low Perfusion del OxSim OX-1 reproduce una condición de baja perfusión mediante una configuración de SpO2 de 99 %, frecuencia cardíaca de 80 bpm e índice de perfusión aproximado de 0.2 [2].

## 3.7. Sistemas de alarma

Los sistemas de alarma de los monitores de signos vitales permiten identificar mediciones que superan los límites establecidos por el operador. Para ello, se configuran valores superiores e inferiores que funcionan como umbrales de vigilancia.

Durante la práctica se utilizaron límites de alarma de SpO2 de 90 % para el límite inferior y 97 % para el límite superior. Estas configuraciones permitieron evaluar la respuesta del monitor ante condiciones de desaturación y saturación elevada.

La verificación de alarmas debe considerar tanto la indicación visual como la sonora, además del tiempo transcurrido entre la generación de la condición simulada y la respuesta del equipo. La FDA contempla la evaluación de los indicadores y alarmas visuales y audibles dentro de las pruebas de desempeño de los pulsioxímetros [5].

## 3.8. Error absoluto y error porcentual

Para evaluar las diferencias entre los valores configurados en el simulador y los valores presentados por el monitor, se utilizan indicadores de error.

El error absoluto representa la diferencia en magnitud entre el valor medido y el valor de referencia:

\[
E_a = |V_m - V_r|
\]

Donde:

- \(E_a\): error absoluto.
- \(V_m\): valor mostrado por el monitor.
- \(V_r\): valor de referencia configurado en el simulador.

El error porcentual expresa el error absoluto en relación con el valor de referencia:

\[
E_p = \frac{|V_m-V_r|}{|V_r|}\times 100
\]

Este indicador permite expresar la diferencia como porcentaje y facilita la comparación entre mediciones de diferentes magnitudes.

---

# IV. Metodología

## 4.1. Materiales y equipos

Para el desarrollo de la práctica se utilizaron los siguientes equipos:

- Monitor de signos vitales Mindray uMEC 100.
- Simulador de parámetros hemodinámicos Pronk OxSim OX-1.
- Sensor de pulsioximetría compatible con el simulador.
- Registro fotográfico de las mediciones realizadas.

## 4.2. Preparación de los equipos

Inicialmente, se encendió el monitor de signos vitales Mindray uMEC 100 y se verificó su disponibilidad para realizar las mediciones. Posteriormente, se conectó el sensor de pulsioximetría al simulador Pronk OxSim OX-1, ubicándolo sobre la zona óptica destinada para la simulación.

Una vez establecida la conexión, se verificó el funcionamiento de los dispositivos y se seleccionaron los diferentes modos de simulación disponibles en el OxSim.

## 4.3. Desarrollo de las pruebas

Se realizaron dos pruebas experimentales siguiendo el procedimiento establecido en la guía de laboratorio. En ambas se evaluaron cuatro condiciones de simulación.

### Prueba 1

**Condición 1. Bradicardia**

<p align="center">
<img width="1280" height="960" 
  alt="40_95" 
  src="https://github.com/user-attachments/assets/d8efe648-14ba-4c04-b0bf-80873fd5e466" />

</p>

<p align="center">
  <strong>Figura 1.</strong> Configuración del simulador para la condición de bradicardia (40 bpm y SpO2 de 95 %).
</p>


Se configuró el simulador para representar una frecuencia cardíaca de 40 bpm y una SpO2 de 95 %. Se registraron los valores presentados por el monitor y se observó la señal fotopletismográfica.

**Condición 2. Disminución de SpO2**

<p align="center">
<img width="1280" height="960" alt="80_85" src="https://github.com/user-attachments/assets/f036ff8f-cbb9-4324-aa3c-9103891fc298" />

</p>
<p align="center">
  <strong>Figura 2.</strong> Configuración del simulador para la condición de desaturación (80 bpm y SpO2 de 85 %).
</p>

Se estableció el límite inferior de alarma de SpO2 en 90 %. Posteriormente, se configuró el simulador para generar una frecuencia cardíaca de 80 bpm y una saturación de oxígeno de 85 %. Después de esperar cinco segundos, se verificó la respuesta visual y sonora del monitor.

**Condición 3. Baja perfusión**

<p align="center">
<img width="960" height="1280" alt="Low_99" src="https://github.com/user-attachments/assets/9a5ffb4b-9668-4fd9-9034-806b1179b36f" />

</p>
<p align="center">
  <strong>Figura 3.</strong> Selección del modo Low Perfusion en el simulador Pronk OxSim OX-1.
</p>

Se configuró el límite superior de alarma de SpO2 en 97 %. A continuación, se seleccionó el modo Low Perfusion del OxSim, correspondiente a una SpO2 de 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2. Se observó el comportamiento de la señal fotopletismográfica y la respuesta del monitor después de cinco segundos.

**Condición 4. Taquicardia**

<p align="center">
<img width="1280" height="960" alt="140_98" src="https://github.com/user-attachments/assets/fdc33db4-1f87-403b-b076-deffc17c9491" />

</p>
<p align="center">
  <strong>Figura 4.</strong> Configuración del simulador para la condición de taquicardia (140 bpm y SpO2 de 98 %).
</p>


Finalmente, se configuró el simulador para representar una frecuencia cardíaca de 140 bpm y una SpO2 de 98 %. Se registró la respuesta del monitor y se observó el comportamiento de la señal y las alarmas.

### Prueba 2

Se repitió el procedimiento experimental anterior, utilizando las mismas configuraciones del simulador y los mismos límites de alarma.

Se registraron nuevamente los valores presentados por el monitor Mindray uMEC 100 y se documentaron las condiciones observadas mediante fotografías.

La repetición del procedimiento permitió comparar el comportamiento del monitor entre las dos pruebas realizadas.

## 4.4. Procesamiento de los datos

Los valores de referencia configurados en el simulador se compararon con las mediciones presentadas en el monitor.

Para cada variable se planteó el cálculo del error absoluto y porcentual mediante las ecuaciones presentadas en el marco teórico.

Adicionalmente, se organizaron los resultados en tablas para facilitar la comparación entre las dos pruebas, considerando la respuesta de las alarmas y el comportamiento de las señales fotopletismográficas.

---


# V. Resultados

Los resultados obtenidos durante la práctica se organizaron de acuerdo con las cuatro condiciones de simulación evaluadas en cada una de las dos pruebas experimentales. Para cada condición se presentan los parámetros configurados en el simulador Pronk OxSim OX-1, las lecturas registradas en el monitor Mindray uMEC 100 y la evidencia fotográfica correspondiente.

## 5.1. Resultados de la prueba 1

### 5.1.1. Simulación de bradicardia

Se configuró el simulador para generar una frecuencia cardíaca de 40 bpm y una saturación periférica de oxígeno del 95 %. Se registraron los valores presentados por el monitor Mindray uMEC 100, con el propósito de comparar las mediciones obtenidas con los parámetros de referencia.

**Figura 1. Simulación de bradicardia durante la prueba 1.**

![Prueba 1 - Bradicardia](../evidencias/prueba_1/bradicardia.jpg)

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 40 | 40 |
| SpO2 (%) | 95 | 95 |

### 5.1.2. Simulación de disminución de SpO2

Se estableció el límite inferior de alarma de SpO2 en 90 %. Posteriormente, se configuró el simulador con una frecuencia cardíaca de 80 bpm y una saturación de oxígeno del 85 %. Se observó la respuesta del monitor ante una condición inferior al límite establecido.

**Figura 2. Simulación de desaturación durante la prueba 1.**

![Prueba 1 - Desaturación](../evidencias/prueba_1/desaturacion.jpg)

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 80 | 80 |
| SpO2 (%) | 85 | 85 |

### 5.1.3. Simulación de baja perfusión

Se seleccionó el modo Low Perfusion del simulador, correspondiente a una SpO2 de 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2. Se observó la señal fotopletismográfica presentada en el monitor y su comportamiento durante esta condición.

**Figura 3. Simulación de baja perfusión durante la prueba 1.**

![Prueba 1 - Baja perfusión](../evidencias/prueba_1/baja_perfusion.jpg)

| Variable | Valor de referencia |
|---|---:|
| Frecuencia cardíaca (bpm) | 80 |
| SpO2 (%) | 99 |
| Índice de perfusión | 0.2 |

### 5.1.4. Simulación de taquicardia

Se configuró el simulador para generar una frecuencia cardíaca de 140 bpm y una SpO2 del 98 %. Se registraron los valores mostrados por el monitor y se observó el comportamiento de la señal fotopletismográfica ante el incremento de la frecuencia cardíaca.

**Figura 4. Simulación de taquicardia durante la prueba 1.**

![Prueba 1 - Taquicardia](../evidencias/prueba_1/taquicardia.jpg)

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 140 | 140 |
| SpO2 (%) | 98 | 98 |

---

## 5.2. Resultados de la prueba 2

### 5.2.1. Simulación de bradicardia

Se repitió la configuración de bradicardia utilizando una frecuencia cardíaca de 40 bpm y una SpO2 del 95 %. Se registraron las mediciones presentadas por el monitor para comparar su comportamiento con respecto a la primera prueba.

**Figura 5. Simulación de bradicardia durante la prueba 2.**

![Prueba 2 - Bradicardia](../evidencias/prueba_2/bradicardia.jpg)

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 40 | 40 |
| SpO2 (%) | 95 | 95 |

### 5.2.2. Simulación de disminución de SpO2

Se configuró nuevamente el límite inferior de alarma de SpO2 en 90 % y se generó una frecuencia cardíaca de 80 bpm con una saturación del 85 %. Se documentó la respuesta del monitor y el comportamiento de la señal.

**Figura 6. Simulación de desaturación durante la prueba 2.**

![Prueba 2 - Desaturación](../evidencias/prueba_2/desaturacion.jpg)

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 80 | 80 |
| SpO2 (%) | 85 | 85 |

### 5.2.3. Simulación de baja perfusión

Se seleccionó el modo Low Perfusion del OxSim OX-1, estableciendo una SpO2 del 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2. Se observó la respuesta del monitor y las características de la señal fotopletismográfica.

**Figura 7. Simulación de baja perfusión durante la prueba 2.**

![Prueba 2 - Baja perfusión](../evidencias/prueba_2/baja_perfusion.jpg)

| Variable | Valor de referencia |
|---|---:|
| Frecuencia cardíaca (bpm) | 80 |
| SpO2 (%) | 99 |
| Índice de perfusión | 0.2 |

### 5.2.4. Simulación de taquicardia

Finalmente, se configuró una frecuencia cardíaca de 140 bpm y una SpO2 del 98 %. Se registraron las lecturas del monitor y se observó la señal fotopletismográfica generada durante esta condición.

**Figura 8. Simulación de taquicardia durante la prueba 2.**

![Prueba 2 - Taquicardia](../evidencias/prueba_2/taquicardia.jpg)

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 140 | 140 |
| SpO2 (%) | 98 | 98 |

---

## 5.3. Comparación general de las pruebas

Una vez presentados los resultados individuales, se realiza una comparación de las mediciones obtenidas durante las dos pruebas, considerando las diferencias entre los valores de referencia y las lecturas del monitor.

En esta sección se presentan los errores absolutos y porcentuales, así como la respuesta de las alarmas y las observaciones relacionadas con las señales fotopletismográficas.

# VI. Análisis de resultados

## 6.1. Comportamiento durante la simulación de bradicardia

En ambas pruebas se configuró el simulador para representar una frecuencia cardíaca de 40 bpm y una SpO2 de 95 %. Los registros fotográficos muestran que el monitor presentó los mismos valores configurados en el simulador.

Esta correspondencia indica que, durante esta condición, el monitor logró identificar los parámetros simulados sin evidenciar diferencias numéricas en las lecturas registradas.

Es importante considerar que la frecuencia cardíaca de 40 bpm corresponde a una condición de baja frecuencia que permite evaluar la capacidad del sistema para detectar pulsaciones lentas. El fabricante del OxSim señala que este modo se encuentra cerca del límite de desempeño de algunos pulsioxímetros [2].

## 6.2. Comportamiento durante la disminución de SpO2

En la segunda condición se configuró una frecuencia cardíaca de 80 bpm y una SpO2 de 85 %, mientras que el límite inferior de alarma del monitor se estableció en 90 %.

Las lecturas identificadas en las fotografías corresponden a 80 bpm y 85 % de SpO2, coincidiendo con los valores configurados en el simulador.

Desde el punto de vista de la verificación de alarmas, esta condición permite evaluar si el monitor identifica una saturación inferior al límite establecido. Debido a que el valor simulado de 85 % se encuentra por debajo del umbral de 90 %, se esperaba la activación de la alarma correspondiente.

La evaluación de esta respuesta debe considerar tanto la señal visual como la sonora, ya que la presencia de una lectura numérica no garantiza por sí misma que el sistema de alarmas esté funcionando correctamente.

## 6.3. Comportamiento durante la simulación de baja perfusión

El modo Low Perfusion permitió evaluar el comportamiento del sistema de pulsioximetría ante una reducción de la componente pulsátil de la señal.

En esta condición, el simulador genera una SpO2 de 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2 [2].

La reducción del índice de perfusión representa una condición de adquisición más exigente para el monitor, debido a que disminuye la intensidad relativa de la señal pulsátil detectada por el sensor.

La calidad de la señal fotopletismográfica resulta especialmente importante en este escenario, puesto que una señal de menor amplitud puede dificultar la identificación de las pulsaciones. La FDA reconoce que una circulación deficiente puede afectar la precisión de las mediciones de pulsioximetría [1].

Por esta razón, el análisis de esta condición debe considerar no solamente el valor numérico de SpO2, sino también la estabilidad de la lectura y las características de la onda presentada por el monitor.

## 6.4. Comportamiento durante la simulación de taquicardia

En la última condición se configuró una frecuencia cardíaca de 140 bpm y una SpO2 de 98 %.

Las fotografías de ambas pruebas muestran que el monitor presentó los valores correspondientes a la configuración del simulador.

La frecuencia cardíaca elevada permitió observar el comportamiento de la señal fotopletismográfica ante un aumento de la frecuencia de las pulsaciones. Como consecuencia, se esperaba una mayor cantidad de ciclos de la señal durante el mismo intervalo de tiempo.

Esta condición también permitió evaluar la respuesta del sistema de alarmas frente a una frecuencia cardíaca elevada. Sin embargo, para establecer si se activó correctamente la alarma, es necesario considerar los límites de frecuencia cardíaca que estaban configurados en el monitor.

## 6.5. Comparación entre las dos pruebas

La comparación de las dos pruebas permite identificar una correspondencia entre los valores simulados y las lecturas numéricas del monitor en los escenarios de bradicardia, desaturación y taquicardia que pudieron verificarse visualmente.

La repetición de estas condiciones permitió comprobar que el monitor presentó respuestas numéricas consistentes frente a las configuraciones utilizadas.

No obstante, esta correspondencia no permite establecer por sí sola la exactitud metrológica del equipo, debido a que las pruebas se realizaron con un simulador y no mediante una comparación con mediciones de referencia independientes.

Por lo tanto, los resultados deben interpretarse como una verificación funcional del monitor bajo condiciones simuladas y no como una certificación completa de su desempeño clínico.

---

# VII. Discusión

Los resultados obtenidos durante las dos pruebas permiten analizar la importancia de utilizar simuladores de parámetros fisiológicos para verificar el comportamiento de los monitores de signos vitales.

En primer lugar, la correspondencia entre los valores configurados en el OxSim OX-1 y los presentados en el uMEC 100 durante los escenarios de bradicardia, desaturación y taquicardia evidencia una respuesta numérica consistente del sistema de medición. Esto resulta importante porque permite comprobar que el monitor reconoce diferentes condiciones de frecuencia cardíaca y saturación de oxígeno.

Sin embargo, es necesario diferenciar entre la coincidencia de las lecturas y la exactitud real del equipo. El simulador permite generar condiciones controladas, pero sus resultados están sujetos a las características y tolerancias del sensor y del sistema de medición utilizado [2].

Uno de los aspectos más relevantes de la práctica fue la evaluación del modo Low Perfusion. Esta condición permite reconocer que el funcionamiento de un pulsioxímetro no depende únicamente de la saturación de oxígeno configurada, sino también de la calidad de la señal óptica que recibe el sensor. Cuando la perfusión es baja, la componente pulsátil disminuye y puede dificultar el procesamiento de la señal [1], [4].

Por otra parte, la configuración de los límites de alarma permitió relacionar las mediciones con los mecanismos de vigilancia del monitor. La programación de un límite inferior de SpO2 de 90 % y uno superior de 97 % permitió establecer condiciones para evaluar la respuesta del equipo ante valores fuera del intervalo configurado.

No obstante, la evaluación completa de estos sistemas requiere comprobar tanto las alarmas visuales como las sonoras, así como registrar los tiempos de respuesta. Estos aspectos son importantes porque un monitor puede presentar correctamente una medición y, aun así, tener un comportamiento inadecuado en su sistema de alarmas.

Finalmente, la realización de dos pruebas permitió repetir las mismas configuraciones y observar la consistencia de las lecturas. Aunque se identificaron coincidencias entre los valores de referencia y los presentados por el monitor, sería necesario realizar pruebas adicionales, registrar sistemáticamente los tiempos de respuesta y verificar las alarmas para obtener una evaluación funcional más completa.

---

# VIII. Conclusión

La práctica permitió evaluar el funcionamiento del monitor de signos vitales Mindray uMEC 100 mediante el uso del simulador Pronk OxSim OX-1, utilizando diferentes condiciones de frecuencia cardíaca, saturación periférica de oxígeno e índice de perfusión.

A partir de los registros fotográficos de las dos pruebas, se identificó una correspondencia entre los valores configurados en el simulador y las lecturas presentadas por el monitor en los escenarios de bradicardia, desaturación y taquicardia. Esto permitió reconocer la capacidad del equipo para visualizar diferentes condiciones fisiológicas simuladas.

Asimismo, la evaluación del modo Low Perfusion permitió comprender la importancia de la calidad de la señal fotopletismográfica en el proceso de medición de SpO2, debido a que una reducción de la perfusión puede dificultar la detección de la componente pulsátil.

Por otra parte, la configuración de los límites de alarma permitió comprender la importancia de establecer umbrales de vigilancia para identificar condiciones que se encuentran fuera de los valores definidos. Sin embargo, la verificación completa de estos sistemas requiere documentar la activación sonora y visual, además de los tiempos de respuesta.

En general, la práctica permitió relacionar los principios de funcionamiento de la pulsioximetría con la operación de los equipos de monitoreo biomédico, destacando la importancia de verificar tanto las mediciones como el comportamiento de los sistemas de alarma antes de considerar su desempeño en un entorno clínico.

---

# REFERENCIAS

[1] U.S. Food and Drug Administration (FDA), "Pulse Oximeters," FDA, 2025. [En línea]. Disponible en: https://www.fda.gov/medical-devices/products-and-medical-procedures/pulse-oximeters. [Consultado: 3-nov-2026].

[2] Pronk Technologies, "OxSim SpO2 Simulator: Operator's Manual," Rev. O, Jul. 18, 2017. [En línea]. Disponible en: https://www.pronktech.com/wp-content/uploads/2015/02/501-0603-OX-1-Op-Manual-Rev-O.pdf. [Consultado: 3-nov-2026].

[3] Shenzhen Mindray Bio-Medical Electronics Co., Ltd., "uMEC 60/uMEC 70/uMEC 80/uMEC 100/uMEC 120/uMEC 150 Patient Monitor: Operator's Manual," Rev. 2.0, Jul. 2023. [En línea]. Disponible en: https://www.mindray.com/content/dam/xpace/en/site/mdr-sscp/patient-monitor/umec-series-60-70-80-100-120-150-safety-and-performance-information.pdf. [Consultado: 3-nov-2026].

[4] OpenOximetry, "Does low perfusion impact pulse oximeter accuracy?," OpenOximetry Project. [En línea]. Disponible en: https://openoximetry.org/faq/does-low-perfusion-impact-pulse-oximeter-accuracy/. [Consultado: 3-nov-2026].

[5] U.S. Food and Drug Administration (FDA), "Pulse Oximeters - Premarket Notification Submissions (510(k)s): Guidance for Industry and Food and Drug Administration Staff," FDA. [En línea]. Disponible en: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/pulse-oximeters-premarket-notification-submissions-510ks-guidance-industry-and-food-and-drug. [Consultado: 3-nov-2026].
