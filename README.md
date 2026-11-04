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

## 3.1. Monitor de signos vitales Mindray uMEC 100

El monitor de signos vitales Mindray uMEC 100 es un equipo biomédico destinado a la vigilancia de diferentes variables fisiológicas mediante la adquisición, el procesamiento y la visualización de parámetros como la frecuencia cardíaca y la saturación periférica de oxígeno. Su interfaz permite visualizar valores numéricos, formas de onda y alarmas asociadas con los parámetros monitorizados [3].

El equipo dispone de límites de alarma configurables para identificar valores que superen los umbrales establecidos. Estas alarmas pueden proporcionar indicaciones visuales y sonoras, además de mensajes relacionados con las condiciones de adquisición de las señales. Por esta razón, durante su evaluación es importante diferenciar entre las alarmas fisiológicas y las indicaciones que advierten posibles dificultades en la medición [3].

## 3.2. Simulador de parámetros hemodinámicos Pronk OxSim OX-1

El Pronk OxSim OX-1 es un simulador óptico utilizado para comprobar el funcionamiento de sensores y monitores de pulsioximetría. Su operación permite reproducir diferentes condiciones mediante configuraciones específicas de saturación de oxígeno, frecuencia cardíaca e índice de perfusión, sin necesidad de utilizar un paciente real [2].

El dispositivo cuenta con diferentes modos de simulación que permiten evaluar la respuesta de los monitores ante condiciones fisiológicas determinadas. Para realizar la prueba, se selecciona el modo correspondiente y se coloca el sensor de pulsioximetría sobre la zona óptica del simulador, siguiendo las indicaciones del fabricante [2].

Los modos utilizados durante la práctica permitieron representar condiciones de bradicardia, desaturación, baja perfusión y taquicardia. Es importante considerar que las mediciones obtenidas dependen también de las características y tolerancias del sensor utilizado, por lo que los resultados deben interpretarse dentro de las condiciones de la prueba experimental [2].

## 3.3. Frecuencia cardíaca

La frecuencia cardíaca corresponde al número de ciclos cardíacos que se producen durante un minuto y se expresa en latidos por minuto (bpm). Es una variable utilizada para evaluar el comportamiento del sistema cardiovascular.

Durante la práctica se utilizaron diferentes configuraciones de frecuencia cardíaca en el simulador Pronk OxSim OX-1. Para representar la condición de bradicardia se estableció un valor de 40 bpm, mientras que para la condición de taquicardia se configuró una frecuencia de 140 bpm. Estos valores corresponden a los escenarios seleccionados para evaluar la respuesta del monitor durante el procedimiento experimental [2].

## 3.4. Saturación periférica de oxígeno (SpO₂)

La saturación periférica de oxígeno (SpO₂) representa una estimación del porcentaje de hemoglobina arterial que se encuentra unida al oxígeno. Su medición se realiza mediante la pulsioximetría, una técnica no invasiva que utiliza luz roja e infrarroja para estimar la oxigenación sanguínea [6], [7].

El principio de funcionamiento se basa en las diferencias de absorción óptica de la oxihemoglobina y la hemoglobina desoxigenada. A partir de la luz emitida y recibida por el sensor, el pulsioxímetro procesa las variaciones de intensidad para estimar la saturación de oxígeno [6].

Aunque la pulsioximetría permite realizar mediciones de manera continua y no invasiva, su precisión puede verse afectada por diferentes condiciones, entre ellas la perfusión periférica deficiente, el movimiento y otros factores que alteran la adquisición de la señal. Por esta razón, los valores obtenidos deben interpretarse considerando la calidad de la señal y las condiciones de medición [1], [6], [7].

## 3.5. Fotopletismografía

La fotopletismografía (PPG) es una técnica óptica que permite identificar variaciones en el volumen sanguíneo de los tejidos mediante la detección de cambios en la luz transmitida o reflejada.

En los sistemas de pulsioximetría, la señal fotopletismográfica presenta dos componentes principales:

- **Componente AC:** corresponde a la variación pulsátil asociada principalmente con los cambios de volumen sanguíneo arterial durante el ciclo cardíaco.
- **Componente DC:** representa la contribución relativamente constante de los tejidos y de los componentes sanguíneos no pulsátiles.

El pulsioxímetro analiza las variaciones de absorción de la luz roja e infrarroja y utiliza la relación entre sus componentes pulsátiles y no pulsátiles para estimar la saturación periférica de oxígeno mediante un proceso de calibración [6], [7].

La forma de onda obtenida permite observar las variaciones pulsátiles y proporciona información sobre la calidad de la señal adquirida. Sin embargo, la presencia de una onda visible no garantiza por sí sola que el equipo pueda calcular valores numéricos válidos de frecuencia cardíaca o saturación de oxígeno [7].

## 3.6. Índice de perfusión y baja perfusión

El índice de perfusión (PI) es un parámetro derivado de la señal fotopletismográfica que permite estimar la intensidad relativa del componente pulsátil con respecto al componente no pulsátil. Se utiliza como indicador de la intensidad de la señal pulsátil detectada por el sensor.

Cuando existe una perfusión periférica reducida, la amplitud del componente pulsátil puede disminuir, dificultando su diferenciación respecto a otros componentes de la señal y al ruido presente durante la adquisición. Esta situación puede ocasionar lecturas inestables, valores inexactos o ausencia de medición [4], [7].

Durante la práctica se utilizó el modo *Low Perfusion* del simulador Pronk OxSim OX-1, configurado con una SpO₂ de referencia del 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2. Esta condición permitió evaluar la respuesta del monitor ante una señal óptica de baja intensidad pulsátil [2].

## 3.7. Sistemas de alarma

Los sistemas de alarma de los monitores de signos vitales permiten advertir al operador cuando una variable fisiológica alcanza o supera los límites establecidos. Para ello, se configuran valores superiores e inferiores que funcionan como umbrales de vigilancia.

Durante la práctica se modificaron los límites de alarma del monitor Mindray uMEC 100 para evaluar su respuesta ante diferentes condiciones simuladas de frecuencia cardíaca y saturación periférica de oxígeno. La verificación de estos sistemas debe considerar las indicaciones visuales, las señales audibles y el tiempo transcurrido entre la generación de la condición simulada y la respuesta del equipo [3], [5].

La evaluación de las alarmas debe diferenciar entre una condición que supera un límite configurado y la confirmación de que el monitor efectivamente generó una indicación visual o sonora. La FDA contempla la evaluación de los indicadores y las alarmas visuales y audibles dentro de las pruebas de desempeño de los pulsioxímetros [5].

## 3.8. Error absoluto y error porcentual

Para evaluar las diferencias entre los valores configurados en el simulador y los valores presentados por el monitor, se utilizan indicadores de error que permiten cuantificar la discrepancia entre una medición y su valor de referencia [8].

El error absoluto representa la magnitud de la diferencia entre el valor medido y el valor de referencia:

\[
E_a = |V_m - V_r|
\]

El error relativo relaciona el error absoluto con la magnitud del valor de referencia:

\[
E_r = \frac{|V_m - V_r|}{|V_r|}
\]

Para expresar esta diferencia en porcentaje se utiliza:

\[
E_p = \frac{|V_m - V_r|}{|V_r|}\times 100
\]

Donde:

- \(E_a\): error absoluto.
- \(E_r\): error relativo.
- \(E_p\): error porcentual.
- \(V_m\): valor registrado por el monitor.
- \(V_r\): valor de referencia configurado en el simulador.

El error absoluto permite expresar la magnitud de la diferencia entre los valores comparados, mientras que el error porcentual facilita su interpretación en relación con el valor de referencia [8].

En esta práctica, el error absoluto de la frecuencia cardíaca se expresa en bpm, mientras que para la saturación de oxígeno se expresa en puntos porcentuales. El error porcentual, por su parte, representa la diferencia relativa respecto al valor de referencia.

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
  <strong>Figura 6.</strong> Configuración del límite inferior de alarma de SpO2 en 90 %.
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
  <strong>Figura 8.</strong> Ajuste del límite superior de SpO2 a 97 %, manteniendo el límite inferior en 90 %.
</p>

Para esta condición, se configuró el límite superior de alarma de SpO2 en 97 %, manteniendo el límite inferior en 90 %, con el propósito de evaluar la respuesta del monitor ante una saturación superior al umbral establecido. Posteriormente, se seleccionó el modo *Low Perfusion* del simulador Pronk OxSim OX-1, correspondiente a una SpO2 de referencia del 99 %, una frecuencia cardíaca de 80 bpm y un índice de perfusión aproximado de 0.2.

<p align="center">
<img width="1280" height="960" alt="Prueba1_3" src="https://github.com/user-attachments/assets/d0545bbe-dd9f-4a43-ba42-aa0418c6f95a" />


</p>
<p align="center">
  <strong>Figura 9.</strong> Lectura del monitor durante la simulación de baja perfusión.
</p>

| Variable | Valor de referencia del OxSim | Valor presentado por el uMEC 100 |
|---|---:|---:|
| Frecuencia cardíaca (bpm) | 80 | 80 |
| SpO₂ (%) | 99 | 100 |
| Índice de perfusión (PI) | 0,2 | 0,45 |

La onda fotopletismográfica muestra variaciones cíclicas del volumen sanguíneo arterial periférico, con un ascenso pronunciado asociado a la llegada de sangre durante la sístole y un descenso progresivo durante la diástole. Aunque se conserva un patrón pulsátil reconocible, la condición de baja perfusión se refleja en una menor contribución del componente pulsátil respecto a la señal óptica total. En este caso, el índice de perfusión configurado en el simulador fue de 0,2, mientras que el monitor indicó 0,45. Esta diferencia muestra que ambos equipos presentaron valores distintos para este parámetro durante la simulación.

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

Para evaluar el comportamiento del monitor Mindray uMEC 100 durante la primera prueba, se compararon los valores configurados en el simulador Pronk OxSim OX-1 con las mediciones registradas en el monitor. Se calcularon el error absoluto y el error porcentual para la frecuencia cardíaca (FC) y la saturación periférica de oxígeno (SpO₂).

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
| Baja perfusión | FC (bpm) | 80 | Sin pulso | -- | -- |
| Baja perfusión | SpO2 (%) | 99 | Exceso de luz | -- | -- |
| Taquicardia | FC (bpm) | 140 | 140 | 0 | 0 % |
| Taquicardia | SpO2 (%) | 98 | 98 | 0 | 0 % |

A partir de los registros disponibles, se observa que el monitor presentó coincidencia con los valores de referencia en las condiciones de bradicardia, desaturación y taquicardia. En estos tres escenarios, los errores absolutos y porcentuales fueron iguales a cero para ambas variables.

Por otra parte, durante la simulación de baja perfusión (Low Perfusion), configurada con una SpO2 de referencia del 99 % y una frecuencia cardíaca de 80 bpm, el monitor no logró proporcionar una lectura válida. En la pantalla se visualizaron los mensajes «Exceso de luz para SpO2» y «Sin pulso», lo que evidenció dificultades en la detección y procesamiento de la señal de pulsioximetría.

Debido a esta condición, no fue posible establecer una comparación numérica entre los valores de referencia y los registrados por el monitor, por lo que no se calcularon los errores absoluto ni porcentual para este escenario. Este comportamiento pudo estar relacionado con las condiciones de adquisición de la señal, la configuración del equipo o la detección de la señal durante la simulación. Sin embargo, no se cuenta con evidencia suficiente para determinar la causa exacta.

Considerando únicamente los tres escenarios con mediciones numéricas válidas, el error absoluto medio fue de 0 bpm para la frecuencia cardíaca y de 0 puntos porcentuales para la SpO2. Estos resultados muestran una correspondencia entre las mediciones del monitor y los valores de referencia en las condiciones que pudieron verificarse. No obstante, la falla presentada durante la baja perfusión evidencia una limitación en la adquisición de la señal, que debe tenerse en cuenta al evaluar el desempeño del equipo.

---

### 5.3. Verificación de alarmas del monitor

La siguiente tabla corresponde a la verificación de las alarmas solicitada en la Parte B de la guía. Las condiciones fisiológicas se establecieron en el simulador Pronk OxSim OX-1, mientras que en el monitor Mindray uMEC 100 se configuraron los límites de alarma correspondientes. Una vez establecidos los valores simulados, se esperó el intervalo de cinco segundos indicado en el procedimiento para comprobar la respuesta del equipo.

| Condición evaluada | Límite configurado en el uMEC 100 | Valor simulado en el OxSim | ¿Alarma activa? | Tiempo de verificación |
|---|---|---:|---|---|
| SpO₂ baja | Inferior: 90 % | 85 % | Sí. Se observó la indicación visual "SpO₂ bajo menor de 90 %" en ambas pruebas. | 5 s |
| SpO₂ alta (Low Perfusion) | Superior: 97 % | 99 % | En la primera prueba se observó la indicación visual "SpO₂ alto > 97". En la segunda no se confirmó la activación de esta alarma; aparecieron los mensajes "Sin pulso" y "Exceso de luz para SpO₂". | 5 s |
| Taquicardia | Superior: 120 bpm | 140 bpm | Sí, según el registro de la primera prueba. En la segunda no se confirmó visualmente. | 4 s |

Los resultados evidencian que el monitor Mindray uMEC 100 respondió de manera adecuada ante la disminución de la saturación de oxígeno, al generar la indicación visual correspondiente en ambas pruebas. En cambio, durante la condición de baja perfusión se observó una diferencia entre los ensayos: en el primero se presentó la alarma por SpO₂ elevada, mientras que en el segundo la ausencia de una lectura válida impidió verificar su activación. Esto muestra que la disponibilidad y la calidad de la señal pueden influir en la evaluación del sistema de alarmas.

En cuanto a la taquicardia, la activación visual se registró únicamente en la primera prueba, por lo que no se cuenta con evidencia suficiente para establecer que la respuesta del monitor fue reproducible en ambos ensayos. En general, los resultados permiten identificar respuestas satisfactorias en algunas condiciones, pero también muestran limitaciones en la verificación de las alarmas cuando el equipo no logra obtener mediciones válidas. Cabe señalar que los tiempos consignados corresponden a los intervalos de verificación utilizados durante la práctica y no necesariamente al tiempo real de activación de las alarmas.

---

## 5.4  Comparación entre las pruebas

La evaluación estadística se realizó mediante el cálculo del error absoluto, el error porcentual y el error absoluto medio (EAM), con el propósito de cuantificar las diferencias entre los valores configurados en el simulador Pronk OxSim OX-1 y los registrados por el monitor Mindray uMEC 100. Estos indicadores permitieron analizar la correspondencia de las mediciones para la frecuencia cardíaca (FC) y la saturación periférica de oxígeno (SpO₂) en los escenarios evaluados.

En la primera prueba, la frecuencia cardíaca presentó una diferencia absoluta de cero en las cuatro condiciones, lo que demuestra una coincidencia entre los valores de referencia y los registrados por el monitor. Para la SpO₂, se obtuvo el mismo comportamiento en tres escenarios; sin embargo, durante la baja perfusión se presentó una diferencia de un punto porcentual, debido a que el simulador estaba configurado en 99 % y el monitor indicó 100 %. Esta diferencia corresponde a un error porcentual aproximado del 1,01 %. Al considerar los cuatro escenarios, el EAM fue de 0 bpm para la frecuencia cardíaca y de 0,25 puntos porcentuales para la SpO₂.

En la segunda prueba, los tres escenarios con mediciones válidas presentaron diferencias absolutas de cero para ambas variables. Por consiguiente, se obtuvo un EAM de 0 bpm para la frecuencia cardíaca y de 0 puntos porcentuales para la SpO₂. No obstante, estos resultados corresponden únicamente a tres condiciones, ya que durante la baja perfusión el monitor no proporcionó valores numéricos válidos debido a los mensajes «Sin pulso» y «Exceso de luz para SpO₂». En consecuencia, no fue posible calcular los errores para este escenario.

Al comparar los resultados, se observa que la frecuencia cardíaca presentó una correspondencia exacta con los valores de referencia en todas las condiciones que permitieron obtener mediciones. En la SpO₂, la diferencia registrada durante la primera prueba fue reducida; sin embargo, la ausencia de datos en la segunda prueba impide establecer una comparación estadística completa para la condición de baja perfusión. También es importante señalar que el EAM de cero obtenido en el segundo ensayo no representa necesariamente un mejor desempeño, puesto que se calculó con un escenario menos que en la primera prueba.

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
