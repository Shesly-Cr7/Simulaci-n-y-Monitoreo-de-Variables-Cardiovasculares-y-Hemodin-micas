 # Laboratorio 6: Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas

## Universidad Militar Nueva Granada

### Ingeniería Biomédica – Instrumentación Biomédica y Biosensores

---

## Integrantes

- Shesly Colorado 5600756
- Santiago Mora 5600775
- Daniel Herrera 5600588

---


# INTRODUCCIÓN

En el entorno clínico hospitalario, el monitoreo continuo de signos vitales es fundamental para evaluar el estado fisiológico de un paciente. Variables como la frecuencia cardíaca, la saturación periférica de oxígeno, la presión arterial y la frecuencia respiratoria permiten identificar alteraciones que pueden representar un riesgo clínico si no se detectan oportunamente [2], [5].

Actualmente, los monitores multiparámetro son ampliamente utilizados en servicios como urgencias, cirugía, hospitalización y unidades de cuidado intensivo. Estos equipos permiten visualizar variables fisiológicas en tiempo real y activar alarmas cuando los parámetros salen de los límites configurados [5], [6].

Para garantizar el correcto funcionamiento de estos dispositivos se emplean simuladores biomédicos, como el Pronk OxSim OX-1, el cual permite recrear condiciones clínicas controladas sin necesidad de utilizar pacientes reales. Esto resulta útil en procesos de mantenimiento biomédico, metrología y verificación funcional [4].

En esta práctica se trabajó con el monitor de signos vitales uMEC 100 y el simulador Pronk OxSim OX-1, con el propósito de evaluar el comportamiento del monitor frente a diferentes condiciones fisiológicas y patológicas simuladas, como bradicardia, taquicardia, hipoxemia y baja perfusión.

* Bradicardia
* Taquicardia
* Hipoxemia
* Baja perfusión

Además, se verificó la precisión de las mediciones, la activación de alarmas y la visualización de la onda fotopletismográfica.

---

# MARCO TEÓRICO

## Monitor de signos vitales uMEC 100

El uMEC 100 es un monitor multiparámetro diseñado para el monitoreo continuo de pacientes. Este equipo permite visualizar variables fisiológicas en tiempo real, entre ellas:

* Frecuencia cardíaca (BPM)
* Saturación de oxígeno (SpO₂)
* Presión arterial
* Temperatura
* Frecuencia respiratoria

El equipo posee alarmas configurables de límite superior e inferior, las cuales permiten alertar al personal médico cuando los parámetros fisiológicos se encuentran fuera del rango normal.

---

## Saturación periférica de oxígeno (SpO₂)

La saturación periférica de oxígeno representa el porcentaje de hemoglobina oxigenada en la sangre arterial.

Los valores normales suelen encontrarse entre:

* 95% y 100% → Normal
* 90% – 94% → Hipoxemia leve
* < 90% → Hipoxemia significativa

La medición se realiza mediante pulsioximetría, utilizando sensores ópticos que emplean luz roja e infrarroja.

---

## Frecuencia cardíaca (BPM)

La frecuencia cardíaca corresponde al número de latidos del corazón por minuto.

Valores normales en adultos:

<div align="center">

| Condición   | BPM          |
|:-----------:|:------------:|
| Bradicardia | < 60 BPM     |
| Normal      | 60 – 100 BPM |
| Taquicardia | > 100 BPM    |

</div>
---

## Fotopletismografía (PPG)

La fotopletismografía es una técnica óptica utilizada para detectar cambios en el volumen sanguíneo.

La señal PPG observada en el monitor depende de:

* Perfusión sanguínea
* Frecuencia cardíaca
* Calidad de la señal óptica

Cuando existe baja perfusión, la onda puede distorsionarse o disminuir su amplitud.

---

## Principio de la pulsioximetría

La pulsioximetría es una técnica óptica no invasiva que permite estimar la saturación periférica de oxígeno en sangre arterial. Su funcionamiento se basa en la emisión de luz roja e infrarroja a través del tejido, generalmente en un dedo, y en la medición de la luz absorbida por la hemoglobina oxigenada y desoxigenada [1].

La señal medida tiene dos componentes: una componente continua, asociada a tejidos, piel, hueso y sangre venosa, y una componente pulsátil, relacionada con los cambios de volumen sanguíneo arterial durante cada ciclo cardíaco. A partir de esta componente pulsátil, el monitor estima la SpO₂ y la frecuencia de pulso [1], [2].

En condiciones de baja perfusión periférica, movimiento del paciente, mala colocación del sensor o interferencia lumínica, la amplitud de la señal PPG puede disminuir o distorsionarse. Esto puede producir lecturas inestables o alarmas falsas, especialmente en pacientes con mala perfusión periférica [1], [3].

<p align="center">
  <img width="450" height="350" alt="image" src="https://github.com/user-attachments/assets/03b5b56c-e855-4820-b78b-03cf828dc6d5" />
</p>


## Simulador Pronk OxSim OX-1

El Pronk OxSim OX-1 es un simulador biomédico diseñado para verificar el funcionamiento de monitores de signos vitales y sensores de SpO₂.

Permite simular:

* Frecuencia cardíaca
* Saturación de oxígeno
* Baja perfusión
* Diferentes condiciones fisiológicas y patológicas

El simulador genera señales ópticas equivalentes a las producidas por el tejido humano y la circulación sanguínea.

---

# IMPORTANCIA DE LA PRÁCTICA

La importancia de esta práctica radica en que permitió comprender el funcionamiento de los sistemas de monitoreo biomédico y verificar la respuesta de un monitor clínico frente a diferentes condiciones simuladas.

Esta práctica también permitió:

* Comprender el principio de funcionamiento de la pulsioximetría.
* Analizar la respuesta de las alarmas clínicas.
* Evaluar la precisión de las mediciones.
* Relacionar señales fisiológicas con estados patológicos.
* Comprender la importancia de la metrología biomédica.
* Fortalecer habilidades de documentación técnica mediante GitHub.

---

# OBJETIVOS

## Objetivo General

Operar con el simulador Pronk OxSim (OX-1) y el monitor de signos vitales uMEC 100 para pruebas funcionales.

## Objetivos Específicos

• Identificar los modos de operación de un simulador de parámetros hemodinámicos (Pronk OxSim).
• Verificar los límites de medición de un monitor de signos vitales mediante simulación de variables hemodinámicas.
• Interpretar variaciones en los parámetros hemodinámicos asociadas a estados fisiológicos y patológicos.

---

# PARTE A — REVISIÓN BIBLIOGRÁFICA

## a. ¿Cómo colocar el uMEC 100 en modo “monitor”?

Para colocar el uMEC 100 en modo monitor se debe:

1. Encender el equipo.
2. Esperar el proceso de autoverificación.
3. Acceder al menú principal.
4. Seleccionar el perfil de monitoreo.
5. Configurar alarmas y parámetros.
6. Conectar el sensor SpO₂.
7. Verificar que aparezcan las señales fisiológicas en pantalla.

---

## b. ¿Qué variables puede simular el Pronk OxSim OX-1?

El Pronk OxSim OX-1 es un simulador óptico de SpO₂ utilizado para verificar el funcionamiento de pulsioxímetros, sensores de SpO₂, cables de extensión y monitores de signos vitales. Este equipo permite simular señales ópticas similares a las generadas por un paciente real, de manera que el sensor del monitor pueda interpretar valores de saturación, frecuencia de pulso y perfusión [4].

<div align="center">

| Variable simulada | Descripción |
| ----------------- | ----------- |
| SpO₂ | Simula diferentes valores de saturación periférica de oxígeno. En la práctica se utilizaron valores como 85%, 95%, 98% y 99%. |
| Frecuencia cardíaca / pulso | Simula diferentes frecuencias de pulso, como 40 bpm para bradicardia, 80 bpm como condición normal y 140 bpm para taquicardia. |
| Índice de perfusión | Permite simular condiciones de perfusión normal o baja perfusión. En baja perfusión, la amplitud de la señal PPG disminuye y el monitor puede presentar lecturas menos estables. |
| Condiciones fisiológicas y patológicas | A partir de la combinación de SpO₂, frecuencia de pulso y perfusión, se pueden representar escenarios como hipoxemia, bradicardia, taquicardia y baja perfusión periférica. |

</div>

---

## c. Tolerancias o errores máximos permitidos (EMP)


En esta práctica, los errores se evaluaron comparando el valor configurado en el simulador OxSim OX-1 con el valor mostrado por el monitor uMEC 100. Esta comparación permite verificar funcionalmente si el monitor responde de forma adecuada ante condiciones simuladas.

<div align="center">

| Parámetro evaluado | Criterio usado en la práctica | Interpretación |
| :--- | :--- | :--- |
| Frecuencia cardíaca / pulso | Diferencias pequeñas, cercanas a ±3 bpm | Aceptable si no cambia la interpretación de bradicardia, normalidad o taquicardia |
| SpO₂ | Diferencias aproximadas de ±2% | Aceptable para una verificación funcional de pulsioximetría |
| Alarmas | Activación visual y/o sonora ante valores fuera de límite | Deben activarse cuando el valor simulado supera el límite configurado |
| Onda PPG | Observación cualitativa de amplitud, estabilidad y distorsión | Permite analizar la calidad de la señal y el efecto de la perfusión |

</div>

La evaluación realizada corresponde a una verificación funcional del monitor, no a una calibración metrológica completa. Por esta razón, los errores se interpretaron como diferencias entre el valor simulado y el valor mostrado por el equipo [1], [4], [5].

---

# PARTE B — PROCEDIMIENTO Y RESULTADOS
<p align="center">
 <img width="750" height="450" alt="image" src="https://github.com/user-attachments/assets/aeac141e-c77e-426a-af9a-25873d7c9cc6" />
</p>


## Tabla general de verificación de alarmas

<div align="center">

| Prueba | Límite configurado | Valor simulado | ¿Alarma activa? | Tiempo de respuesta | Observación |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Bradicardia | Límite inferior de FC configurado en el monitor | 40 bpm, SpO₂ 95% | No registrado | No registrado | Se observó frecuencia cardíaca baja en el monitor |
| Hipoxemia | SpO₂ baja: 90% | 80 bpm, SpO₂ 85% | Sí | 5 s | Se activó la alarma por saturación baja |
| SpO₂ alta / baja perfusión | SpO₂ alta: 97% | SpO₂ 99% en modo Low Perfusion | Sí | 5 s | Se observó alteración o disminución de la estabilidad de la onda PPG |
| Taquicardia | Límite superior de FC configurado en el monitor | 140 bpm | Sí | No registrado | Se activó la alarma por frecuencia cardíaca elevada |

</div>

## Caso 1 — Bradicardia



### Configuración

<p align="center">
<img width="750" height="450" alt="image" src="https://github.com/user-attachments/assets/41725158-61f1-426e-b0eb-331e0307aec6" />
</p>

* BPM simulado: 40
* SpO₂ simulado: 95%



### Resultados
<div align="center">

| Tiempo | BPM Simulado | BPM Monitor | Error BPM | SpO₂ Simulada | SpO₂ Monitor | Error SpO₂ |
| ------ | ------------ | ----------- | --------- | ------------- | ------------ | ---------- |
| 1s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 2s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 3s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 4s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 5s     | 40           | 40          | 0         | 95            | 96           | -1         |

</div>

### Explicación de la tabla

Se observa que el monitor detectó correctamente la bradicardia simulada.
La frecuencia cardíaca coincidió exactamente con el valor configurado.

La saturación presentó una diferencia mínima de 1%, lo cual se encuentra dentro del margen clínicamente aceptable.

---

## Caso 2 — Hipoxemia (SpO₂ baja)

### Configuración

* BPM: 80
* SpO₂: 85%

### Resultados

<div align="center">

| Tiempo | BPM Simulado | BPM Monitor | Error BPM | SpO₂ Simulada | SpO₂ Monitor | Error SpO₂ |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 1s | 80 | 80 | 0 | 85 | 85 | 0 |
| 2s | 80 | 80 | 0 | 85 | 85 | 0 |
| 3s | 80 | 80 | 0 | 85 | 85 | 0 |
| 4s | 80 | 80 | 0 | 85 | 85 | 0 |
| 5s | 80 | 80 | 0 | 85 | 85 | 0 |

</div>

### Explicación de la tabla

El monitor respondió correctamente ante una condición de hipoxemia.

La alarma de saturación baja se activó debido a que el valor configurado fue inferior al límite establecido (90%).

No se evidenciaron errores significativos.

---

## Caso 3 — Baja Perfusión

### Configuración

<p align="center">
<img width="400" height="450" alt="image" src="https://github.com/user-attachments/assets/670504a6-4f29-4dc3-af3c-4a4e7bf87168" />
</p>

* Modo: Low Perfusion
* SpO₂ simulada: 99%
* BPM monitor: 80
* Límite superior de alarma SpO₂: 97%

<p align="center">
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/6a48081a-1ebe-41c1-bae1-a038271adb44" />
</p>

### Resultados

<div align="center">

| Tiempo | SpO₂ Simulada | SpO₂ Monitor | Error absoluto SpO₂ | BPM Monitor | ¿Alarma activa? |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 1s | 99 | 100 | 1 | 80 | Sí |
| 2s | 99 | 100 | 1 | 80 | Sí |
| 3s | 99 | 100 | 1 | 80 | Sí |
| 4s | 99 | 100 | 1 | 80 | Sí |
| 5s | 99 | 100 | 1 | 80 | Sí |

</div>

### Explicación de la tabla

Durante la baja perfusión se observó una ligera alteración en la onda fotopletismográfica. Aunque la SpO₂ permaneció cercana al valor esperado, la señal puede presentar menor estabilidad debido a la disminución de amplitud simulada por el OxSim OX-1.

La alarma se activó porque el límite superior de SpO₂ estaba configurado en 97% y el valor simulado fue de 99%. Esta condición permite evidenciar cómo una señal de baja perfusión puede afectar la estabilidad de la lectura y generar posibles falsas alarmas o lecturas inestables [1], [3], [4].

---

## Caso 4 — Taquicardia

### Configuración

* BPM: 140
* SpO₂: 98%

### Resultados

<div align="center">

| Tiempo | BPM Simulado | BPM Monitor | Error BPM | SpO₂ Simulada | SpO₂ Monitor | Error SpO₂ |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 1s | 140 | 140 | 0 | 98 | 99 | -1 |
| 2s | 140 | 140 | 0 | 98 | 99 | -1 |
| 3s | 140 | 140 | 0 | 98 | 98 | 0 |
| 4s | 140 | 140 | 0 | 98 | 98 | 0 |
| 5s | 140 | 140 | 0 | 98 | 99 | -1 |

</div>

### Explicación de la tabla

El monitor identificó correctamente la condición de taquicardia.

La alarma de frecuencia cardíaca elevada se activó adecuadamente debido a que el valor superó el límite establecido.

---

# PARTE C — ANÁLISIS DE RESULTADOS

## Análisis 1 — Precisión de las mediciones

Los resultados obtenidos muestran que el monitor uMEC 100 presentó una alta precisión frente a los valores simulados por el OxSim OX-1.

Los errores encontrados fueron mínimos:

* Error BPM ≈ 0
* Error SpO₂ ≈ ±1%

Estos errores se encuentran dentro de los límites clínicamente aceptables.

---

## Análisis 2 — Relación entre la onda PPG y las variables fisiológicas


<p align="center">
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/5e197319-fbcc-4b45-8695-98224d8404c7" />
</p>

La onda fotopletismográfica, también conocida como onda PPG, representa los cambios de volumen sanguíneo arterial detectados por el sensor de pulsioximetría. A partir de esta señal, el monitor puede estimar variables como la frecuencia de pulso y la saturación periférica de oxígeno SpO₂ [1], [3].

Durante la práctica se observó que la frecuencia de la onda PPG cambia de acuerdo con la frecuencia cardíaca simulada. En el caso de bradicardia, con una frecuencia de 40 bpm, la onda presentó ciclos más separados entre sí, debido a que el pulso era más lento. En cambio, durante la simulación de taquicardia, con una frecuencia de 140 bpm, los ciclos de la onda se visualizaron más cercanos, ya que el pulso simulado era más rápido.

En relación con la SpO₂, el valor de saturación no depende únicamente de la forma visual de la onda, sino del procesamiento interno que realiza el monitor a partir de la señal óptica recibida por el sensor. Sin embargo, la calidad de la onda PPG sí influye en la confiabilidad de la medición, porque una señal estable y con buena amplitud facilita una lectura más precisa de la saturación y de la frecuencia de pulso [1], [2].

En el modo de baja perfusión, la onda PPG puede presentar menor amplitud, inestabilidad o distorsión. Esto ocurre porque se simula una condición en la que la señal pulsátil arterial es débil, lo que dificulta que el monitor identifique correctamente los cambios de volumen sanguíneo. Por esta razón, en condiciones de baja perfusión pueden presentarse lecturas inestables, errores en la SpO₂ o falsas alarmas [1], [3].

En general, la onda PPG permitió relacionar visualmente el comportamiento del monitor con las condiciones fisiológicas simuladas. Una frecuencia cardíaca baja produjo una onda más lenta, una frecuencia cardíaca alta produjo una onda más rápida y la baja perfusión afectó principalmente la estabilidad y amplitud de la señal.

---

# CONCLUSIONES

* El monitor uMEC 100 respondió adecuadamente frente a las condiciones simuladas de bradicardia, hipoxemia, baja perfusión y taquicardia.

* El simulador Pronk OxSim OX-1 permitió generar escenarios fisiológicos y patológicos controlados, facilitando la evaluación funcional del monitor sin necesidad de utilizar pacientes reales.

* Los errores obtenidos entre los valores simulados y los valores mostrados por el monitor fueron bajos, especialmente en la medición de frecuencia cardíaca, donde se obtuvo coincidencia directa en la mayoría de las pruebas.

* Las alarmas visuales y sonoras se activaron correctamente cuando los valores simulados superaron los límites configurados, lo cual demuestra la importancia de una configuración adecuada de alarmas en el entorno clínico.

* La baja perfusión afectó principalmente la estabilidad de la onda fotopletismográfica, evidenciando que la calidad de la señal es un factor importante para la confiabilidad de la medición de SpO₂.

* La práctica permitió relacionar conceptos de instrumentación biomédica, pulsioximetría, simulación fisiológica, análisis de error y seguridad del paciente.

---

# PREGUNTAS PARA LA DISCUSIÓN

## 1. ¿Cuál es el principio de operación del Pronk OxSim OX-1 para simular una onda pulsátil?

El OxSim OX-1 funciona mediante la generación de señales ópticas controladas que imitan la absorción de luz producida por la sangre humana.

El simulador reproduce cambios periódicos similares al pulso arterial utilizando LEDs y sistemas electrónicos internos, permitiendo que el sensor SpO₂ interprete la señal como si proviniera de un paciente real.

---

## 2. ¿Por qué la SpO₂ baja puede ser un falso positivo en una situación de mala perfusión?

En condiciones de baja perfusión, la amplitud de la señal fotopletismográfica disminuye porque llega menos volumen sanguíneo pulsátil a la zona donde está ubicado el sensor. Esto dificulta que el monitor diferencie correctamente la componente arterial pulsátil de otros componentes de la señal [1], [3].

Como consecuencia, el equipo puede generar lecturas inestables, valores erróneos de SpO₂ o falsas alarmas de saturación baja, aunque la oxigenación real del paciente no necesariamente esté alterada. Por esta razón, una alarma de SpO₂ debe interpretarse junto con la calidad de la onda PPG, el estado clínico del paciente y la correcta ubicación del sensor [1], [3], [5].

---


# REFERENCIAS

[1] ISO, “ISO 80601-2-61:2017 Medical electrical equipment — Particular requirements for basic safety and essential performance of pulse oximeter equipment,” International Organization for Standardization, 2017. [En línea]. Disponible: https://www.iso.org/standard/67963.html

[2] J. G. Webster, Medical Instrumentation: Application and Design, 4th ed. Hoboken, NJ: John Wiley & Sons, 2010.

[3] J. G. Webster, Design of Pulse Oximeters. Boca Raton, FL: CRC Press, 1997.

[4] Pronk Technologies, “OX-1 OxSim Optical SpO₂ Pulse Oximeter Simulator,” Pronk Technologies. [En línea]. Disponible: https://www.pronktech.com/product/ox-1-oxsim-miniaturized-optical-spo2-pulse-oximeter-tester/

[5] Mindray, “uMEC 100/120/150 Patient Monitor Datasheet,” Mindray. [En línea]. Disponible: https://healthtechghana.com/wp-content/uploads/2024/07/Datasheet_uMEC-100-120-150_20230628.pdf

[6] Mindray, “uMEC Series Patient Monitor Safety and Performance Information,” Mindray. [En línea]. Disponible: https://www.mindray.com/content/dam/xpace/en/site/mdr-sscp/patient-monitor/umec-series-60-70-80-100-120-150-safety-and-performance-information.pdf

[7] Universidad Militar Nueva Granada, “Guía de Preparación Práctica de Laboratorio: Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas,” Laboratorio de Instrumentación Biomédica y Biosensores, 2025.
