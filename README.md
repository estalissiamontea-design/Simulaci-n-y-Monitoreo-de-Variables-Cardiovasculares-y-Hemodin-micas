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

<p align="center">
<img width="1280" height="960" alt="Prueba1_1" src="https://github.com/user-attachments/assets/d9379b1f-ebe8-4a0c-8790-f78256014470" />
</p>
<p align="center">
  <strong>Figura 5.</strong> Lectura del monitor durante la simulación de bradicardia (40 bpm y SpO2 de 95 %).
</p>

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 40 | 40 |
| SpO2 (%) | 95 | 95 |

La señal fotopletismográfica presenta oscilaciones periódicas y relativamente uniformes, en correspondencia con la frecuencia cardíaca de 40 bpm configurada en el simulador. Se observa una mayor separación entre los pulsos consecutivos, característica asociada con una frecuencia cardíaca reducida, ya que transcurre más tiempo entre cada ciclo pulsátil. A pesar de esta disminución en la frecuencia, la onda conserva una morfología reconocible y una periodicidad estable, lo que indica que el monitor logró identificar adecuadamente la señal pulsátil y representar el comportamiento esperado durante la condición de bradicardia. Asimismo, la saturación de oxígeno se mantuvo en el valor de referencia del 95 %, sin que se evidenciaran alteraciones importantes en la forma de onda.

### 5.1.2. Simulación de disminución de SpO2

<p align="center">
  <img width="1280" height="960" alt="Limite_Inferior" src="https://github.com/user-attachments/assets/e19e14be-37eb-484a-a56b-0c30aa13e960" />
</p>

<p align="center">
  <strong>Figura 6.</strong> Configuración del límite inferior de alarma de SpO2: límite superior de 97 % e inferior de 90 %.
</p>

Se estableció el límite inferior de alarma de SpO2 en 90 %. Posteriormente, se configuró el simulador con una frecuencia cardíaca de 80 bpm y una saturación de oxígeno del 85 %. Se observó la respuesta del monitor ante una condición inferior al límite establecido.

<p align="center">
<img width="1280" height="960" alt="Pureba1_2" src="https://github.com/user-attachments/assets/ce77d08e-0d6d-4e34-bafd-40b8cc1ff8be" />

</p>
<p align="center">
  <strong>Figura 7.</strong> Lectura del monitor ante una saturación de oxígeno del 85 %.
</p>


| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 80 | 80 |
| SpO2 (%) | 85 | 85 |

Durante la condición de desaturación se observa una señal fotopletismográfica con oscilaciones periódicas, cuya frecuencia corresponde a los 80 bpm establecidos en el simulador. En comparación con la condición anterior, los pulsos aparecen más próximos entre sí, lo que refleja el incremento de la frecuencia cardíaca. Aunque la saturación de oxígeno disminuyó hasta el 85 %, la señal conserva un patrón pulsátil definido, lo que permite observar que la reducción de la SpO₂ no necesariamente produce una disminución proporcional de la amplitud de la onda. Esto se debe a que la fotopletismografía representa las variaciones del volumen sanguíneo periférico, mientras que la saturación corresponde a la proporción de hemoglobina que transporta oxígeno. Por tanto, ambas variables están relacionadas con la actividad cardiovascular, pero describen fenómenos diferentes.

### 5.1.3. Simulación de baja perfusión

<p align="center">
  <img width="1280" height="960" alt="Limite_superior" src="https://github.com/user-attachments/assets/a7440337-7f49-42dc-bc56-da92c8bdf172" />

</p>

<p align="center">
  <strong>Figura 8.</strong> Ajuste del límite superior de SpO2 a 100 %, manteniendo el límite inferior en 90 %.
</p>

Para esta condición, se configuró el límite superior de alarma de SpO2 en 97 %, manteniendo el límite inferior en 90 %, con el propósito de evaluar la respuesta del monitor ante una saturación superior al umbral establecido. Posteriormente, se seleccionó el modo *Low Perfusion* del simulador Pronk OxSim OX-1, correspondiente a una SpO2 de referencia del 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2.

<p align="center">
<img width="1280" height="960" alt="Prueba1_3" src="https://github.com/user-attachments/assets/d0545bbe-dd9f-4a43-ba42-aa0418c6f95a" />


</p>
<p align="center">
  <strong>Figura 9.</strong> Lectura del monitor durante la simulación de baja perfusión.
</p>

| Variable | Valor de referencia |
|---|---:|
| Frecuencia cardíaca (bpm) | 80 |
| SpO2 (%) | 99 |
| Índice de perfusión | 0.2 |

En esta condición, el simulador se configuró en modo Low Perfusion para representar una disminución de la perfusión periférica. En la pantalla del monitor se observa que la señal fotopletismográfica presenta cambios en su morfología y una apariencia menos uniforme en comparación con las condiciones anteriores. Este comportamiento se relaciona con la reducción de la componente pulsátil de la señal, que puede dificultar la identificación de las variaciones de volumen sanguíneo utilizadas por el pulsioxímetro para estimar la saturación de oxígeno. A pesar de estas condiciones, durante esta primera prueba el monitor logró proporcionar una lectura de SpO₂ del 100 %, frente al 99 % configurado en el simulador. La diferencia observada fue de un punto porcentual, lo que evidencia que el equipo pudo obtener una medición numérica, aunque bajo una condición de adquisición menos favorable. Además, se había establecido un límite superior de alarma del 97 %, por lo que la lectura obtenida superaba dicho umbral.

### 5.1.4. Simulación de taquicardia

Se configuró el simulador para generar una frecuencia cardíaca de 140 bpm y una SpO2 del 98 %. Se registraron los valores mostrados por el monitor y se observó el comportamiento de la señal fotopletismográfica ante el incremento de la frecuencia cardíaca.

<p align="center">
  <img width="1280" height="960" alt="Prueba1_4" src="https://github.com/user-attachments/assets/3ee4f8c5-82aa-476d-91fb-85cee5472066" />

</p>
<p align="center">
  <strong>Figura 10.</strong> Lectura del monitor durante la simulación de taquicardia (140 bpm y SpO2 de 98 %).
</p>

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 140 | 140 |
| SpO2 (%) | 98 | 98 |

La señal fotopletismográfica muestra un aumento evidente en la frecuencia de sus oscilaciones, con pulsos más cercanos entre sí en comparación con las condiciones de bradicardia y desaturación. Este comportamiento corresponde al incremento de la frecuencia cardíaca hasta 140 bpm, debido a que el intervalo de tiempo entre cada pulso disminuye a medida que aumenta el número de latidos por minuto. A pesar de la mayor frecuencia, la onda conserva un patrón periódico y una morfología relativamente uniforme, lo que permite reconocer los ciclos pulsátiles de manera continua. Por otra parte, la saturación de oxígeno se mantuvo en el 98 %, sin presentar una variación relevante respecto al valor configurado. En esta condición también se observó la activación de la alarma de frecuencia cardíaca elevada, en concordancia con el valor simulado y los límites de alarma establecidos en el monitor.

#### Resultados stadísticos de los valores de referencia y los registrados en la prueba 1

Para evaluar el comportamiento del monitor BeneHeart D30 durante la primera prueba, se compararon los valores configurados en el simulador Pronk OxSim OX-1 con las mediciones registradas en el monitor. Se calcularon el error absoluto y el error porcentual para la frecuencia cardíaca (FC) y la saturación periférica de oxígeno (SpO₂).

El error absoluto se determinó mediante la diferencia entre el valor medido y el valor de referencia, mientras que el error porcentual permitió establecer la magnitud de dicha diferencia respecto al valor configurado.

| Condición | Variable | Referencia | Monitor | Error absoluto | Error porcentual |
|---|---|---:|---:|---:|---:|
| Bradicardia | FC (bpm) | 40 | 40 | 0 | 0 % |
| Bradicardia | SpO₂ (%) | 95 | 95 | 0 | 0 % |
| Desaturación | FC (bpm) | 80 | 80 | 0 | 0 % |
| Desaturación | SpO₂ (%) | 85 | 85 | 0 | 0 % |
| Baja perfusión | FC (bpm) | 80 | 80 | 0 | 0 % |
| Baja perfusión | SpO₂ (%) | 99 | 100 | 1 | 1,01 % |
| Taquicardia | FC (bpm) | 140 | 140 | 0 | 0 % |
| Taquicardia | SpO₂ (%) | 98 | 98 | 0 | 0 % |

A partir de los resultados, se observa que el monitor presentó coincidencia con los valores de referencia en las condiciones de bradicardia, desaturación y taquicardia. En estos escenarios, los errores absolutos y porcentuales fueron iguales a cero para ambas variables.
Por otra parte, durante la simulación de baja perfusión se registró una diferencia de un punto porcentual en la SpO₂, debido a que el monitor indicó 100 %, mientras que el simulador estaba configurado en 99 %. Esto representa un error porcentual aproximado del 1,01 %. La frecuencia cardíaca, por su parte, coincidió con el valor de referencia de 80 bpm.
Considerando los cuatro escenarios, el error absoluto medio fue de 0 bpm para la frecuencia cardíaca y de 0,25 puntos porcentuales para la SpO₂. Esto indica que las diferencias numéricas fueron reducidas y que la mayor variación se presentó durante la condición de baja perfusión.

---

## 5.2. Resultados de la prueba 2

### 5.2.1. Simulación de bradicardia

Se repitió la configuración de bradicardia utilizando una frecuencia cardíaca de 40 bpm y una SpO2 del 95 %. Se registraron las mediciones presentadas por el monitor para comparar su comportamiento con respecto a la primera prueba.

<p align="center">
  <img width="1280" height="960" alt="Prueba2_1" src="https://github.com/user-attachments/assets/af24da72-e20b-4168-b30f-68bbf22df2e1" />

</p>
<p align="center">
  <strong>Figura 11.</strong> Lectura del monitor durante la simulación de bradicardia durante la prueba 2.
</p>

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 40 | 40 |
| SpO2 (%) | 95 | 95 |

La onda fotopletismográfica presenta un patrón periódico, con pulsos ampliamente separados y una morfología relativamente uniforme. Esta separación se relaciona con la disminución de la frecuencia cardíaca, debido a que el intervalo entre cada ciclo pulsátil aumenta cuando se reduce el número de latidos por minuto. A pesar de esta condición, el monitor conserva una señal claramente identificable y registra correctamente los valores de frecuencia cardíaca y saturación de oxígeno configurados en el simulador. También se observa el aviso de derivación de ECG desconectada; sin embargo, el equipo indica que el origen de la frecuencia cardíaca es SpO2, por lo que la medición se obtiene a través de la señal del pulsioxímetro.

### 5.2.2. Simulación de disminución de SpO2

Se configuró nuevamente el límite inferior de alarma de SpO2 en 90 % y se generó una frecuencia cardíaca de 80 bpm con una saturación del 85 %. Se documentó la respuesta del monitor y el comportamiento de la señal.

<p align="center">
  <img width="1280" height="960" alt="Prueba2_2" src="https://github.com/user-attachments/assets/a236ce88-7c4e-4198-a195-9680d6799e69" />
  
</p>
<p align="center">
  <strong>Figura 12.</strong> Lectura del monitor durante la simulación de desaturación durante la prueba 2.
</p>

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 80 | 80 |
| SpO2 (%) | 85 | 85 |

La onda fotopletismográfica conserva una secuencia de pulsos periódicos y definidos, aunque estos se encuentran más próximos entre sí en comparación con la condición de bradicardia. Este comportamiento corresponde al aumento de la frecuencia cardíaca, ya que el intervalo entre los ciclos pulsátiles disminuye. Adicionalmente, se observa la activación de la alarma de saturación baja, identificada mediante el mensaje «SpO2 bajo menor de 90 %», lo cual concuerda con el límite inferior configurado en el monitor. La conservación de una señal pulsátil reconocible, a pesar de la disminución de la saturación, permite observar que la desaturación no necesariamente produce una alteración evidente en la periodicidad o morfología de la onda fotopletismográfica.

### 5.2.3. Simulación de baja perfusión

Se seleccionó el modo Low Perfusion del OxSim OX-1, estableciendo una SpO2 del 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2. Se observó la respuesta del monitor y las características de la señal fotopletismográfica.

<p align="center">
  <img width="1280" height="960" alt="Prueba2_3_1" src="https://github.com/user-attachments/assets/275af680-2ee1-4b5a-b641-73cf9686ab07" />

</p>
<p align="center">
  <strong>Figura 13.</strong> Primera captura de la señal fotopletismográfica durante la simulación de baja perfusión en la prueba 2.
</p>

En la primera captura se observa que el monitor continúa mostrando una onda fotopletismográfica periódica, con oscilaciones reconocibles y una morfología relativamente estable. Sin embargo, el equipo presenta los mensajes «Sin pulso» y «Exceso de luz para SpO2», sin proporcionar valores numéricos válidos de frecuencia cardíaca y saturación de oxígeno. Esto evidencia que la presencia visual de una onda en pantalla no garantiza que el monitor pueda identificarla y procesarla correctamente para calcular las variables fisiológicas. Por tanto, aunque se conserva una representación gráfica de las oscilaciones, el equipo no logra validar la señal para realizar las mediciones correspondientes.

**Figura 8. Segunda captura de la señal fotopletismográfica durante la simulación de baja perfusión en la prueba 2.**

<p align="center">
  <img width="1280" height="960" alt="Prueba2_3_2" src="https://github.com/user-attachments/assets/00783af0-4f19-41fe-882b-fb53d8dd0636" />

</p>
<p align="center">
  <strong>Figura 14.</strong> Segunda captura de la señal fotopletismográfica durante la simulación de baja perfusión en la prueba 2.
</p>

En la segunda captura se aprecia un cambio en la apariencia de la onda fotopletismográfica respecto al registro anterior. Las oscilaciones presentan una forma más marcada y continua, con picos y valles visualmente más pronunciados. No obstante, esta variación no se acompaña de una recuperación de las mediciones, ya que el monitor mantiene los mensajes «Sin pulso» y «Exceso de luz para SpO2», sin proporcionar valores numéricos válidos de frecuencia cardíaca ni saturación de oxígeno. Este comportamiento demuestra que la representación gráfica de la señal y la capacidad del equipo para obtener una medición válida no son necesariamente equivalentes. La variación de la onda podría estar relacionada con las características de la señal simulada y las condiciones de adquisición; sin embargo, no es posible establecer una causa específica únicamente a partir de las fotografías.

| Variable | Valor de referencia | Resultado del monitor |
|---|---:|---|
| Frecuencia cardíaca (bpm) | 80 | Sin pulso |
| SpO2 (%) | 99 | Exceso de luz |
| Índice de perfusión | 0.2 | Sin lectura válida |

### 5.2.4. Simulación de taquicardia

Finalmente, se configuró una frecuencia cardíaca de 140 bpm y una SpO2 del 98 %. Se registraron las lecturas del monitor y se observó la señal fotopletismográfica generada durante esta condición.

**Figura 9. Simulación de taquicardia durante la prueba 2.**

<p align="center">
  <img width="1280" height="960" alt="Prueba2__4" src="https://github.com/user-attachments/assets/6e72ac52-977d-4882-9900-d3da7e8f556a" />

</p>
<p align="center">
  <strong>Figura 15.</strong> Lectura del monitor durante la simulación de taquicardia durante la prueba 2.
</p>

| Variable | Valor de referencia | Valor del monitor |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 140 | 140 |
| SpO2 (%) | 98 | 98 |

La onda fotopletismográfica presenta oscilaciones más frecuentes y próximas entre sí, con una sucesión continua de pulsos que refleja la disminución del intervalo entre ciclos debido al incremento de la frecuencia cardíaca. A pesar de la mayor frecuencia, la señal conserva una morfología periódica y permite distinguir los pulsos de manera consecutiva. Por otra parte, la saturación de oxígeno permanece en el valor de referencia del 98 %, sin presentar una variación apreciable durante la simulación. En la captura no se distingue claramente un mensaje de alarma por frecuencia cardíaca elevada, por lo que su activación no puede confirmarse únicamente con este registro visual.

### Resultados estadísticos de los valores de referencia y los registrados en la prueba 2

Para evaluar el comportamiento del monitor uMEC 100 durante la segunda prueba, se compararon los valores configurados en el simulador Pronk OxSim OX-1 con las mediciones registradas en el monitor. Se analizaron las variables de frecuencia cardíaca (FC) y saturación periférica de oxígeno (SpO2) para las cuatro condiciones experimentales. Para establecer las diferencias entre ambas mediciones, se calcularon el error absoluto y el error porcentual.

El error absoluto se determinó mediante la diferencia en valor absoluto entre el valor registrado por el monitor y el valor de referencia. El error porcentual permitió expresar esta diferencia en relación con el valor configurado en el simulador.

| Condición | Variable | Referencia | Monitor | Error absoluto | Error porcentual |
|---|---|---:|---:|---:|---:|
| Bradicardia | FC (bpm) | 40 | 40 | 0 | 0 % |
| Bradicardia | SpO2 (%) | 95 | 95 | 0 | 0 % |
| Desaturación | FC (bpm) | 80 | 80 | 0 | 0 % |
| Desaturación | SpO2 (%) | 85 | 85 | 0 | 0 % |
| Baja perfusión | FC (bpm) | 80 | Sin pulso | NAN | NAN |
| Baja perfusión | SpO2 (%) | 99 | Exceso de luz | NAN | NAN |
| Taquicardia | FC (bpm) | 140 | 140 | 0 | 0 % |
| Taquicardia | SpO2 (%) | 98 | 98 | 0 | 0 % |

A partir de los registros disponibles, se observa que el monitor presentó coincidencia con los valores de referencia en las condiciones de bradicardia, desaturación y taquicardia. En estos tres escenarios, los errores absolutos y porcentuales fueron iguales a cero para ambas variables.

Por otra parte, durante la simulación de baja perfusión (Low Perfusion), configurada con una SpO2 de referencia del 99 % y una frecuencia cardíaca de 80 bpm, el monitor no logró proporcionar una lectura válida. En la pantalla se visualizaron los mensajes «Exceso de luz para SpO2» y «Sin pulso», lo que evidenció dificultades en la detección y procesamiento de la señal de pulsioximetría.

Debido a esta condición, no fue posible establecer una comparación numérica entre los valores de referencia y los registrados por el monitor, por lo que no se calcularon los errores absoluto ni porcentual para este escenario. Este comportamiento pudo estar relacionado con las condiciones de adquisición de la señal, la configuración del equipo o la detección de la señal durante la simulación. Sin embargo, no se cuenta con evidencia suficiente para determinar la causa exacta.

Considerando únicamente los tres escenarios con mediciones numéricas válidas, el error absoluto medio fue de 0 bpm para la frecuencia cardíaca y de 0 puntos porcentuales para la SpO2. Estos resultados muestran una correspondencia entre las mediciones del monitor y los valores de referencia en las condiciones que pudieron verificarse. No obstante, la falla presentada durante la baja perfusión evidencia una limitación en la adquisición de la señal, que debe tenerse en cuenta al evaluar el desempeño del equipo.

---


## 5.3  Comparación entre las pruebas

Al comparar los resultados de las dos pruebas experimentales, se observa que el monitor BeneHeart D30 presentó un comportamiento similar en las condiciones de bradicardia, desaturación y taquicardia. En ambos ensayos, las mediciones de frecuencia cardíaca y saturación periférica de oxígeno coincidieron con los valores configurados en el simulador Pronk OxSim OX-1, por lo que los errores absoluto y porcentual fueron iguales a cero en estos tres escenarios.

La principal diferencia se presentó durante la simulación de baja perfusión (Low Perfusion). En la primera prueba, el monitor registró una frecuencia cardíaca de 80 bpm y una SpO₂ de 100 %, frente a los valores de referencia de 80 bpm y 99 %, respectivamente. Esto representó un error absoluto de 0 bpm para la frecuencia cardíaca y de 1 punto porcentual para la saturación de oxígeno, equivalente a un error porcentual aproximado del 1,01 %.

En contraste, durante la segunda prueba, el monitor no proporcionó una lectura válida para esta misma condición. En la pantalla aparecieron los mensajes "Exceso de luz" para SpO₂ y "Sin pulso" para la frecuencia cardíaca, lo que impidió realizar los cálculos de error correspondientes. Por tanto, mientras que en el primer ensayo se obtuvo una lectura numérica, en el segundo se presentó una dificultad en la adquisición de las señales.

Esta diferencia evidencia que el comportamiento del monitor no fue completamente reproducible entre ambos ensayos bajo la condición de baja perfusión. Aunque se sospecha que una configuración inadecuada del equipo pudo influir en el resultado de la segunda prueba, no se cuenta con información suficiente para confirmar esta causa.

En general, los resultados muestran una respuesta consistente del monitor en las condiciones de bradicardia, desaturación y taquicardia. Sin embargo, la diferencia observada en baja perfusión evidencia la importancia de verificar la configuración del equipo y las condiciones de adquisición antes de interpretar las mediciones. Asimismo, demuestra que la evaluación del monitor debe considerar tanto la coincidencia de los valores numéricos como su capacidad para detectar y procesar adecuadamente las señales fisiológicas.

# VI. Análisis de resultados

### 6.1. Análisis 1. Evaluación estadística de las diferencias entre los valores de referencia y los registrados por el monitor

La comparación estadística de los resultados de las dos pruebas experimentales permitió determinar las diferencias entre los valores configurados en el simulador Pronk OxSim OX-1 y los registrados por el monitor. En las condiciones de bradicardia, desaturación y taquicardia se obtuvo una coincidencia exacta entre ambas mediciones, tanto para la frecuencia cardíaca como para la saturación periférica de oxígeno. Esto representa diferencias absolutas de 0 bpm para la frecuencia cardíaca y de 0 puntos porcentuales para la SpO₂ en dichos escenarios.

En la primera prueba, la única diferencia numérica se presentó durante la simulación de baja perfusión. El simulador se encontraba configurado con una SpO₂ del 99 %, mientras que el monitor registró un valor del 100 %, lo que corresponde a una diferencia absoluta de un punto porcentual y un error relativo aproximado del 1,01 %. Para la frecuencia cardíaca no se presentó diferencia respecto al valor de referencia de 80 bpm. Al considerar los cuatro escenarios evaluados, el error absoluto medio fue de 0 bpm para la frecuencia cardíaca y de 0,25 puntos porcentuales para la SpO₂. Estos resultados reflejan una diferencia promedio reducida entre los valores simulados y los registrados durante esta prueba.

En la segunda prueba, las tres condiciones en las que se obtuvieron mediciones numéricas presentaron diferencias absolutas iguales a cero para ambas variables. Sin embargo, durante la simulación de baja perfusión no fue posible calcular el error, debido a que el monitor no proporcionó valores válidos de frecuencia cardíaca ni de SpO₂. Por esta razón, el error absoluto medio se calculó únicamente con los tres escenarios disponibles, obteniendo 0 bpm para la frecuencia cardíaca y 0 puntos porcentuales para la SpO₂. Es importante señalar que estos promedios no incluyen la condición de baja perfusión y, por tanto, no representan la totalidad de los escenarios evaluados.

Al comparar ambas pruebas, se observa que la frecuencia cardíaca presentó coincidencia con los valores de referencia en todos los escenarios donde se obtuvieron lecturas válidas. Para la SpO₂, la primera prueba presentó una diferencia de un punto porcentual en baja perfusión, mientras que en la segunda no fue posible establecer una diferencia numérica para esta condición. Esta variación entre ensayos podría estar relacionada con las condiciones de adquisición de la señal o con una posible interferencia óptica durante la segunda prueba. No obstante, al no contar con verificaciones adicionales, no es posible determinar el origen específico de esta diferencia.

En términos generales, los resultados estadísticos evidencian una baja diferencia entre los valores de referencia y los registrados por el monitor en las condiciones donde se obtuvieron mediciones válidas. Sin embargo, la ausencia de datos durante la segunda prueba de baja perfusión limita la comparación estadística completa y pone de manifiesto que la evaluación del equipo también debe considerar su capacidad para obtener mediciones válidas, además de la exactitud de los valores que logra registrar.

### 6.2. Análisis 2. Relación entre la forma de onda visualizada en el monitor y la frecuencia cardíaca/saturación periférica de oxígeno

El comportamiento de las ondas fotopletismográficas permitió reconocer la relación entre la frecuencia cardíaca y la periodicidad de la señal, así como la influencia de las condiciones de perfusión sobre su adquisición. En términos generales, los cambios en la frecuencia cardíaca se reflejaron en la separación temporal de los pulsos, mientras que las variaciones de saturación de oxígeno no produjeron necesariamente modificaciones equivalentes en la morfología de la onda. Esto se debe a que la señal fotopletismográfica representa las variaciones del volumen sanguíneo periférico, mientras que la SpO₂ corresponde a la proporción de hemoglobina oxigenada estimada por el pulsioxímetro. Por otra parte, la condición de baja perfusión permitió identificar una situación particular: aunque el monitor continuó mostrando una representación gráfica de la señal, presentó dificultades para proporcionar mediciones válidas. Además, las dos capturas obtenidas durante esta condición mostraron diferencias visuales en la morfología de la onda, sin que se recuperara la lectura de las variables fisiológicas. Este comportamiento indica que la visualización de una señal pulsátil no garantiza por sí sola que el equipo pueda procesarla adecuadamente para obtener resultados confiables. En conjunto, los hallazgos permiten reconocer que la frecuencia cardíaca influye principalmente en la periodicidad de la señal, mientras que las condiciones de perfusión pueden afectar su calidad y la capacidad del monitor para realizar la medición.

### 6.3. Discusión general de los resultados

Uno de los resultados más relevantes de la práctica se presentó durante la simulación de baja perfusión, debido a que el comportamiento del monitor fue diferente entre los dos ensayos. En la primera prueba, el equipo logró registrar una SpO₂ del 100 %, aunque el simulador estaba configurado en 99 %. En cambio, durante la segunda prueba aparecieron los mensajes "Exceso de luz" y "Sin pulso", impidiendo obtener una medición válida.

Una posible explicación de esta diferencia está relacionada con las condiciones de adquisición de la señal de pulsioximetría. El funcionamiento de este sistema depende de la detección de las variaciones de luz transmitida o reflejada a través del tejido, las cuales permiten identificar el componente pulsátil de la sangre arterial. Cuando existe una perfusión periférica reducida, la amplitud de este componente puede disminuir y dificultar su diferenciación respecto a otros componentes de la señal. Esto puede afectar la identificación del pulso y la estimación de la saturación de oxígeno.

Adicionalmente, el mensaje "Exceso de luz" sugiere que el monitor detectó una condición que interfería con la adquisición óptica. Por esta razón, también es posible que factores relacionados con la posición del sensor, la iluminación externa, la conexión o la configuración del equipo hayan influido en el resultado. Sin embargo, estas posibilidades no pudieron comprobarse durante la práctica, por lo que no es posible establecer una causa definitiva.

Por otra parte, la coincidencia de las mediciones de frecuencia cardíaca y SpO₂ durante las condiciones de bradicardia, desaturación y taquicardia muestra que el monitor pudo identificar adecuadamente las variables simuladas en esos escenarios. Esto contrasta con la dificultad presentada durante la baja perfusión y evidencia que la calidad de la señal constituye un factor importante para obtener mediciones confiables.

En consecuencia, los resultados permiten reconocer que el desempeño de un monitor de signos vitales no depende únicamente de su capacidad para mostrar valores numéricos, sino también de las condiciones de adquisición y procesamiento de las señales. Por ello, ante una lectura inválida o un mensaje de error, es necesario verificar el sensor, sus conexiones y la configuración del equipo antes de interpretar los resultados como una alteración fisiológica.

---

# VII. Discusión
### 7.1. ¿Cuál es el principio de operación del simulador Pronk OxSim OX-1 para simular una onda pulsátil?

El simulador Pronk OxSim OX-1 funciona mediante un sistema óptico que reproduce las condiciones de medición de un pulsioxímetro sin necesidad de utilizar un paciente real. Para ello, interactúa directamente con el sensor del monitor, interceptando los destellos de luz roja e infrarroja emitidos por sus LED y bloqueándolos para generar nuevos destellos ópticos mediante mecanismos electrónicos, ópticos y mecánicos. De esta manera, el simulador produce una señal que representa el comportamiento de la luz al atravesar el tejido de un dedo humano durante la medición de la saturación de oxígeno [2].

El funcionamiento del pulsioxímetro se basa en la diferencia de absorción de la luz roja e infrarroja por parte de la oxihemoglobina y la desoxihemoglobina. Durante el ciclo cardíaco, el volumen de sangre arterial aumenta en la sístole y disminuye en la diástole, generando variaciones en la cantidad de luz absorbida. Estas variaciones constituyen el componente pulsátil de la señal, conocido como componente AC, mientras que la absorción relativamente constante de los tejidos y otros componentes sanguíneos corresponde al componente DC [6]. A partir de la relación entre ambos componentes para las dos longitudes de onda, el equipo calcula un índice de modulación que utiliza para estimar la SpO₂ [7].

El OxSim reproduce estas condiciones mediante diferentes configuraciones que permiten evaluar la respuesta del monitor ante distintos valores de frecuencia cardíaca, saturación de oxígeno y perfusión. Durante la práctica se utilizaron los modos de bradicardia, desaturación, baja perfusión y taquicardia, con valores de referencia de 40, 80 y 140 bpm, y saturaciones de 85 %, 95 %, 98 % y 99 %, según el escenario. En particular, el modo de baja perfusión establece una SpO₂ de 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0,2 [2].

Por lo tanto, el simulador permite comprobar el comportamiento del monitor frente a señales ópticas controladas y reproducibles, facilitando la evaluación de sus mediciones, alarmas y capacidad para procesar señales pulsátiles bajo diferentes condiciones de funcionamiento [2].

### 7.2. ¿Por qué una SpO₂ baja puede ser una falsa alarma cuando existe mala perfusión?

La medición de la saturación de oxígeno mediante pulsioximetría depende de la detección de los cambios de volumen de sangre arterial que se producen con cada latido cardíaco. Cuando existe una perfusión periférica deficiente, disminuye la cantidad de sangre pulsátil que llega al sitio donde se encuentra ubicado el sensor, lo que reduce la amplitud del componente AC de la señal fotopletismográfica [6]. Como consecuencia, disminuye la relación señal-ruido y se dificulta la identificación de la señal arterial frente a otros componentes ópticos y al ruido presente durante la adquisición [7].

Esta condición puede ocasionar lecturas inestables, interrupciones en la medición o la imposibilidad de obtener un valor de SpO₂. En determinadas circunstancias, el procesamiento de una señal de baja calidad también puede producir valores de saturación inferiores a los reales y generar falsas alarmas de desaturación [6], [7]. Por esta razón, una lectura baja no debe interpretarse de manera aislada como evidencia definitiva de hipoxemia, sino que debe considerarse junto con la calidad de la señal, la intensidad del pulso y las condiciones del paciente. La FDA también reconoce la mala circulación como uno de los factores que pueden afectar la precisión de los pulsioxímetros [1].

En la segunda prueba de la práctica, esta situación se evidenció durante la simulación de baja perfusión. Aunque el OxSim se configuró con una saturación de referencia del 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0,2, el monitor Mindray uMEC 100 no logró proporcionar valores numéricos válidos de frecuencia cardíaca ni de SpO₂. En su lugar, presentó los mensajes "Sin pulso" y "Exceso de luz para SpO₂". Este comportamiento muestra que, bajo condiciones de perfusión reducida, el equipo puede tener dificultades para reconocer y procesar adecuadamente la señal óptica, incluso cuando se observa una onda en pantalla. El manual del OxSim advierte que su modo de baja perfusión está diseñado para representar una condición exigente y que algunos monitores pueden presentar dificultades para obtener mediciones en este escenario [2].

En consecuencia, una SpO₂ baja o una alarma de desaturación durante una condición de mala perfusión podría estar relacionada con una limitación en la adquisición de la señal y no necesariamente con una disminución real de la oxigenación sanguínea. Sin embargo, esto no significa que todas las lecturas bajas en pacientes con mala perfusión sean falsas, ya que la hipoxemia también puede estar presente. Por ello, es necesario verificar la calidad de la señal y contrastar la medición con otras evaluaciones clínicas cuando exista incertidumbre [6], [7].


---

# VIII. Conclusión
La práctica permitió comprobar el funcionamiento del monitor de signos vitales al someterlo a diferentes condiciones cardiovasculares simuladas. Al comparar los valores configurados en el simulador con las mediciones del equipo, se encontró que, tanto en la primera como en la segunda prueba, las lecturas de frecuencia cardíaca y saturación de oxígeno fueron cercanas a los valores de referencia durante la bradicardia, la desaturación y la taquicardia. No obstante, los resultados fueron diferentes durante la baja perfusión. En la primera prueba, el monitor registró una saturación de oxígeno del 100 %, frente al 99 % establecido en el simulador, mientras que en la segunda aparecieron los mensajes «Exceso de luz» y «Sin pulso», lo que impidió obtener una lectura válida. Esta diferencia puede estar relacionada con la dificultad del sensor para detectar adecuadamente la señal pulsátil cuando la perfusión es baja, aunque también es posible que hayan influido su posición o las condiciones de conexión. Por otra parte, durante la práctica se identificó la importancia de configurar correctamente las alarmas y prestar atención a los mensajes que presenta el equipo, ya que no solo indican cambios en las variables medidas, sino también posibles dificultades en la adquisición de las señales. Finalmente, se considera necesario repetir la prueba de baja perfusión, revisar la ubicación y conexión del sensor y realizar más ensayos que permitan comprobar si este comportamiento se mantiene bajo las mismas condiciones.


---

# REFERENCIAS

[1] U.S. Food and Drug Administration (FDA), "Pulse Oximeters," FDA, 2025. [En línea]. Disponible en: https://www.fda.gov/medical-devices/products-and-medical-procedures/pulse-oximeters.

[2] Pronk Technologies, "OxSim SpO2 Simulator: Operator's Manual," Rev. O, Jul. 18, 2017. [En línea]. Disponible en: https://www.pronktech.com/wp-content/uploads/2015/02/501-0603-OX-1-Op-Manual-Rev-O.pdf.

[3] Shenzhen Mindray Bio-Medical Electronics Co., Ltd., "uMEC 60/uMEC 70/uMEC 80/uMEC 100/uMEC 120/uMEC 150 Patient Monitor: Operator's Manual," Rev. 2.0, Jul. 2023. [En línea]. Disponible en: https://www.mindray.com/content/dam/xpace/en/site/mdr-sscp/patient-monitor/umec-series-60-70-80-100-120-150-safety-and-performance-information.pdf.

[4] OpenOximetry, "Does low perfusion impact pulse oximeter accuracy?," OpenOximetry Project. [En línea]. Disponible en: https://openoximetry.org/faq/does-low-perfusion-impact-pulse-oximeter-accuracy/.

[5] U.S. Food and Drug Administration (FDA), "Pulse Oximeters - Premarket Notification Submissions (510(k)s): Guidance for Industry and Food and Drug Administration Staff," FDA. [En línea]. Disponible en: https://www.fda.gov/regulatory-information/search-fda-guidance-documents/pulse-oximeters-premarket-notification-submissions-510ks-guidance-industry-and-food-and-drug.

[6] E. D. Chan, M. M. Chan y M. M. Chan, “Pulse oximetry: Understanding its basic principles facilitates appreciation of its limitations,” Respiratory Medicine, vol. 107, n.º 6, pp. 789–799, Jun. 2013. doi: 10.1016/j.rmed.2013.02.004. [En línea]. Disponible en: https://www.resmedjournal.com/article/S0954-6111(13)00053-X/fulltext. 

[7] A. Jubran, “Pulse oximetry,” Critical Care, vol. 19, art. 272, 2015. doi: 10.1186/s13054-015-0984-8. [En línea]. Disponible en: https://pmc.ncbi.nlm.nih.gov/articles/PMC4504215/.
