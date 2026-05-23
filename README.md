 # Laboratorio 5: Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas

## Universidad Militar Nueva Granada

### Ingeniería Biomédica – Instrumentación Biomédica y Biosensores

---

## Integrantes

- Shesly Colorado 5600756
- Santiago Mora 5600775
- Daniel Herrera 5600588

---

# INTRODUCCIÓN

En el entorno clínico hospitalario, el monitoreo continuo de signos vitales constituye una de las herramientas más importantes para evaluar el estado fisiológico de un paciente. Variables como la frecuencia cardíaca (BPM), la saturación periférica de oxígeno (SpO₂), la frecuencia respiratoria y la presión arterial permiten detectar alteraciones hemodinámicas que pueden representar un riesgo para la vida del paciente.

Actualmente, los monitores multiparámetro son ampliamente utilizados en unidades de cuidados intensivos (UCI), salas de cirugía, urgencias y hospitalización. Estos equipos deben ser capaces de detectar cambios fisiológicos de manera rápida y precisa, además de generar alarmas visuales y sonoras cuando los parámetros salen de los límites fisiológicos configurados.

Para garantizar el correcto funcionamiento de estos dispositivos biomédicos, se utilizan simuladores de parámetros fisiológicos, como el Pronk OxSim OX-1, el cual permite recrear condiciones clínicas controladas sin necesidad de utilizar pacientes reales. Este tipo de simuladores son fundamentales en procesos de mantenimiento biomédico, metrología, calibración y verificación funcional.

En esta práctica se trabajó con el monitor de signos vitales uMEC 100 y el simulador Pronk OxSim OX-1, con el propósito de evaluar el comportamiento del monitor ante diferentes condiciones fisiológicas y patológicas simuladas, como:

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

| Condición   | BPM          |
| ----------- | ------------ |
| Bradicardia | < 60 BPM     |
| Normal      | 60 – 100 BPM |
| Taquicardia | > 100 BPM    |

---

## Fotopletismografía (PPG)

La fotopletismografía es una técnica óptica utilizada para detectar cambios en el volumen sanguíneo.

La señal PPG observada en el monitor depende de:

* Perfusión sanguínea
* Frecuencia cardíaca
* Calidad de la señal óptica

Cuando existe baja perfusión, la onda puede distorsionarse o disminuir su amplitud.

---

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

| Variable                | Descripción                      |
| ----------------------- | -------------------------------- |
| BPM                     | Simula frecuencia cardíaca       |
| SpO₂                    | Simula saturación periférica     |
| Baja perfusión          | Reduce amplitud de señal PPG     |
| Condiciones patológicas | Simula alteraciones fisiológicas |

---

## c. Tolerancias o errores máximos permitidos (EMP)

| Parámetro | Error máximo permitido         |
| --------- | ------------------------------ |
| BPM       | ±3 BPM                         |
| SpO₂      | ±2%                            |
| Alarmas   | Activación rápida y detectable |

---

# PARTE B — PROCEDIMIENTO Y RESULTADOS

## Caso 1 — Bradicardia

### Configuración

* BPM simulado: 40
* SpO₂ simulado: 95%

### Resultados

| Tiempo | BPM Simulado | BPM Monitor | Error BPM | SpO₂ Simulada | SpO₂ Monitor | Error SpO₂ |
| ------ | ------------ | ----------- | --------- | ------------- | ------------ | ---------- |
| 1s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 2s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 3s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 4s     | 40           | 40          | 0         | 95            | 96           | -1         |
| 5s     | 40           | 40          | 0         | 95            | 96           | -1         |

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

| Tiempo | BPM Simulado | BPM Monitor | Error BPM | SpO₂ Simulada | SpO₂ Monitor | Error SpO₂ |
| ------ | ------------ | ----------- | --------- | ------------- | ------------ | ---------- |
| 1s     | 80           | 80          | 0         | 85            | 85           | 0          |
| 2s     | 80           | 80          | 0         | 85            | 85           | 0          |
| 3s     | 80           | 80          | 0         | 85            | 85           | 0          |
| 4s     | 80           | 80          | 0         | 85            | 85           | 0          |
| 5s     | 80           | 80          | 0         | 85            | 85           | 0          |

### Explicación de la tabla

El monitor respondió correctamente ante una condición de hipoxemia.

La alarma de saturación baja se activó debido a que el valor configurado fue inferior al límite establecido (90%).

No se evidenciaron errores significativos.

---

## Caso 3 — Baja Perfusión

### Configuración

* Modo: Low Perfusion
* SpO₂: 99%

### Resultados

| Tiempo | BPM Monitor | SpO₂ Monitor |
| ------ | ----------- | ------------ |
| 1s     | 80          | 100          |
| 2s     | 80          | 100          |
| 3s     | 80          | 100          |
| 4s     | 80          | 100          |
| 5s     | 80          | 100          |

### Explicación de la tabla

Durante la baja perfusión se observó una ligera alteración en la onda fotopletismográfica.

Aunque la SpO₂ permaneció cercana al valor esperado, la señal PPG presentó menor estabilidad debido a la disminución de amplitud simulada por el OxSim.

---

## Caso 4 — Taquicardia

### Configuración

* BPM: 140
* SpO₂: 98%

### Resultados

| Tiempo | BPM Simulado | BPM Monitor | Error BPM | SpO₂ Simulada | SpO₂ Monitor | Error SpO₂ |
| ------ | ------------ | ----------- | --------- | ------------- | ------------ | ---------- |
| 1s     | 140          | 140         | 0         | 98            | 99           | -1         |
| 2s     | 140          | 140         | 0         | 98            | 99           | -1         |
| 3s     | 140          | 140         | 0         | 98            | 98           | 0          |
| 4s     | 140          | 140         | 0         | 98            | 98           | 0          |
| 5s     | 140          | 140         | 0         | 98            | 99           | -1         |

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

La onda fotopletismográfica depende directamente del flujo sanguíneo y de la perfusión periférica.

Durante:

* Bradicardia → la onda aparece más lenta.
* Taquicardia → la onda aumenta su frecuencia.
* Baja perfusión → la amplitud disminuye y la señal puede distorsionarse.

Esto demuestra que la señal PPG refleja el comportamiento hemodinámico del paciente.

---

# CONCLUSIONES

* El monitor uMEC 100 respondió correctamente frente a todas las condiciones simuladas.
* El OxSim OX-1 permitió recrear condiciones fisiológicas y patológicas de manera segura.
* Los errores obtenidos fueron bajos y clínicamente aceptables.
* Las alarmas visuales y sonoras funcionaron adecuadamente.
* La condición de baja perfusión afectó principalmente la estabilidad de la onda fotopletismográfica.
* La práctica permitió comprender la importancia de la calibración y verificación de equipos biomédicos.

---

# PREGUNTAS PARA LA DISCUSIÓN

## 1. ¿Cuál es el principio de operación del Pronk OxSim OX-1 para simular una onda pulsátil?

El OxSim OX-1 funciona mediante la generación de señales ópticas controladas que imitan la absorción de luz producida por la sangre humana.

El simulador reproduce cambios periódicos similares al pulso arterial utilizando LEDs y sistemas electrónicos internos, permitiendo que el sensor SpO₂ interprete la señal como si proviniera de un paciente real.

---

## 2. ¿Por qué la SpO₂ baja puede ser un falso positivo en una situación de mala perfusión?

En condiciones de baja perfusión, la amplitud de la señal fotopletismográfica disminuye considerablemente.

Esto ocasiona que el sensor tenga dificultades para detectar correctamente el pulso arterial, generando lecturas inestables o falsas alarmas de saturación baja.

Por esta razón, una mala perfusión puede provocar falsos positivos aunque la oxigenación del paciente sea normal.

---

# REFERENCIAS



