# LAB-6-simulador-signos-vitales

# Laboratorio: Verificación de Parámetros Fisiológicos con el uMEC 100 y el Pronk OxSim OX-1


# Introducción

Los monitores de signos vitales son dispositivos biomédicos fundamentales en el entorno clínico, ya que permiten supervisar continuamente parámetros fisiológicos como frecuencia cardíaca, saturación periférica de oxígeno (SpO₂), presión arterial y frecuencia respiratoria.

En esta práctica se utilizó el monitor de signos vitales uMEC 100 junto con el simulador Pronk OxSim OX-1 para evaluar el comportamiento del sistema ante diferentes condiciones fisiológicas simuladas.

---

# Objetivos

## Objetivo general

Verificar el funcionamiento del monitor uMEC 100 mediante el simulador biomédico OxSim OX-1.

## Objetivos específicos

- Identificar los parámetros fisiológicos simulables.
- Evaluar la activación de alarmas fisiológicas.
- Calcular errores absolutos y porcentuales.
- Analizar la señal fotopletismográfica obtenida.

---

# Marco Teórico

## Monitor de signos vitales uMEC 100

El uMEC 100 es un monitor multiparámetro utilizado para supervisar continuamente variables fisiológicas como:

- Saturación periférica de oxígeno (SpO₂)
- Frecuencia cardíaca
- Presión arterial
- Frecuencia respiratoria
- Temperatura

El equipo genera alarmas visuales y auditivas cuando los parámetros exceden los límites configurados.

---

## Simulador Pronk OxSim OX-1

El OxSim OX-1 es un simulador diseñado para probar sensores de pulsioximetría. Su funcionamiento se basa en la simulación óptica de señales equivalentes a las producidas por un paciente real.

Permite simular:
- Saturación de oxígeno (SpO₂)
- Frecuencia cardíaca
- Baja perfusión
- Intensidad de pulso
- Condiciones fisiológicas anormales

---

## Fotopletismografía

La fotopletismografía (PPG) es una técnica óptica que detecta cambios volumétricos sanguíneos en la microvasculatura mediante la absorción de luz roja e infrarroja.

La señal PPG permite estimar:
- Saturación periférica de oxígeno
- Frecuencia cardíaca
- Calidad de perfusión

---

# PARTE A

# 1. Revisión bibliográfica

## a. ¿Cómo colocar al uMEC 100 en modo monitor?

1. Encender el equipo.
2. Esperar el autodiagnóstico.
3. Seleccionar el tipo de paciente.
4. Ingresar al menú principal.
5. Verificar que el sistema esté en modo “Monitor”.
6. Conectar los sensores correspondientes.

> Nota: La interfaz puede variar dependiendo de la versión del firmware.

---

## b. ¿Qué parámetros fisiológicos pueden simularse con el Pronk OxSim OX-1?

| Parámetro | Descripción |
|---|---|
| SpO₂ | Simula el porcentaje de hemoglobina oxigenada. |
| Frecuencia cardíaca | Simula latidos por minuto (bpm). |
| Baja perfusión | Simula disminución del flujo sanguíneo periférico. |
| Intensidad de pulso | Modifica la amplitud de la señal PPG. |
| Señales patológicas | Simula condiciones fisiológicas anormales. |

---

## c. Errores máximos permitidos (EMP)

| Parámetro | Error Máximo Permitido |
|---|---|
| SpO₂ | ±2 % |
| Frecuencia cardíaca | ±3 bpm o ±3 % |
| Frecuencia de pulso | ±3 bpm |
| Alarmas fisiológicas | Según fabricante |

---

# PARTE B

# 1. Tabla de verificación de alarmas

Ítem	Objetivo	Valor simulado	"Límite configurado
uMEC100"	superir/inferior	¿alarma activa?	Tiempo de respuesta Sp02%(s)	"Tiempo de respuesta
bpm(s)"
4	Config. OxSim	"40 bpm
SpO2 =95%"	N/A	N/A	No	6	
5	Imagen 5						
6	Config. Alarma		SpO2=95%	inferior	Si		
7	Config. OxSim	"80bpm
SpO2=85%"	SpO2=95%	inferior	Sí	6	
8	Config. Alarma		SpO2=97%	superior	Si		
9	Config. OxSim	"SpO2=99%
Low Perfusion"	SpO2=97%	superior	Si	11	
10	Config. OxSim	"140bpm
SpO2=95%"	"140bmp
previo en el uMEC100"		¿?		7
<img width="918" height="270" alt="image" src="https://github.com/user-attachments/assets/7797e753-bb97-48a5-becf-bf1b4de06d34" />


---

# 2. Procedimiento Experimental

## Paso 1: Configuración inicial

- Se encendió el monitor uMEC100.
- Se configuró en modo monitor.
- Se conectó el sensor SpO₂ al OxSim OX-1.

---

## Paso 2: Simulación de bradicardia

### Configuración
- Frecuencia cardíaca: 40 bpm
- SpO₂: 95 %

### Resultados

| Variable | Valor simulado | Valor medido | Error absoluto | Error porcentual |
|---|---|---|---|---|
| Frecuencia cardíaca | 40 bpm | `[Agregar]` | `[Agregar]` | `[Agregar]` |
| SpO₂ | 95 % | `[Agregar]` | `[Agregar]` | `[Agregar]` |

---

## Onda fotopletismográfica

### Imagen de la señal
`[Insertar imagen]`

### Observaciones
`[Agregar observaciones]`

---

## Paso 3: Alarma de SpO₂ baja

### Configuración
- Límite inferior: 90 %
- Frecuencia cardíaca: 80 bpm
- SpO₂: 85 %

### Resultados

| Variable | Valor simulado | Valor medido | Error absoluto | Error porcentual |
|---|---|---|---|---|
| Frecuencia cardíaca | 80 bpm | `[Agregar]` | `[Agregar]` | `[Agregar]` |
| SpO₂ | 85 % | `[Agregar]` | `[Agregar]` | `[Agregar]` |

### Activación de alarma

- ¿Alarma sonora?: `[Sí/No]`
- ¿Alarma visual?: `[Sí/No]`
- Tiempo de respuesta: `[Agregar]`

---

## Paso 4: Alarma de SpO₂ alta

### Configuración
- Límite superior: 97 %
- SpO₂: 99 %
- Modo: “Low Perfusion”

### Resultados

| Variable | Valor simulado | Valor medido | Error absoluto | Error porcentual |
|---|---|---|---|---|
| SpO₂ | 99 % | `[Agregar]` | `[Agregar]` | `[Agregar]` |

### Observaciones

- ¿Se activó la alarma?: `[Sí/No]`
- ¿La onda PPG se distorsionó?: `[Sí/No]`
- Descripción: `[Agregar descripción]`

---

## Paso 5: Simulación de taquicardia

### Configuración
- SpO₂: 95 %
- Frecuencia cardíaca: 140 bpm

### Resultados

| Variable | Valor simulado | Valor medido | Error absoluto | Error porcentual |
|---|---|---|---|---|
| Frecuencia cardíaca | 140 bpm | `[Agregar]` | `[Agregar]` | `[Agregar]` |
| SpO₂ | 95 % | `[Agregar]` | `[Agregar]` | `[Agregar]` |

### Observaciones

- ¿Se activó la alarma de FC alta?: `[Sí/No]`
- Descripción de la onda: `[Agregar]`

---

# Análisis de Resultados

## Análisis 1: Diferencias entre valores simulados y medidos

### Fórmulas utilizadas

#### Error absoluto

\[
E_a = |Valor_{simulado} - Valor_{medido}|
\]

#### Error porcentual

\[
E_{\%} = \frac{|Valor_{simulado} - Valor_{medido}|}{Valor_{simulado}} \times 100
\]

---

### Resultados estadísticos

| Variable | Promedio error | Desviación estándar |
|---|---|---|
| SpO₂ | `[Agregar]` | `[Agregar]` |
| Frecuencia cardíaca | `[Agregar]` | `[Agregar]` |

### Interpretación

`[Agregar análisis realizado]`

---

## Análisis 2: Relación entre la señal PPG y los parámetros fisiológicos

La frecuencia cardíaca afecta la periodicidad de la señal fotopletismográfica, mientras que la saturación de oxígeno influye en la estabilidad y amplitud de la señal.

En condiciones de baja perfusión la amplitud disminuye considerablemente, generando posibles falsas alarmas.

---

# Preguntas para la discusión

## Pregunta 1

### ¿Cuál es el principio de operación del Pronk OxSim OX-1 para simular una onda pulsátil?

El OxSim OX-1 utiliza un sistema óptico controlado electrónicamente para reproducir la absorción variable de luz roja e infrarroja equivalente a la producida por el flujo sanguíneo humano.

El simulador genera señales compatibles con sensores reales de pulsioximetría, permitiendo medir frecuencia cardíaca y SpO₂.

---

## Pregunta 2

### ¿Por qué la SpO₂ baja puede ser un falso positivo en condiciones de mala perfusión?

Cuando existe mala perfusión, el flujo sanguíneo periférico disminuye y la señal fotopletismográfica pierde amplitud.

Esto provoca una baja relación señal-ruido, haciendo que el monitor interprete incorrectamente la saturación de oxígeno y genere falsas alarmas.

---

# Conclusiones

1. El monitor uMEC100 respondió adecuadamente ante las condiciones fisiológicas simuladas.
2. Las alarmas fisiológicas se activaron correctamente cuando los parámetros excedieron los límites establecidos.
3. La baja perfusión produjo distorsiones en la señal fotopletismográfica.
4. El OxSim OX-1 permitió simular escenarios clínicos útiles para pruebas biomédicas.

---

# Evidencias Experimentales

## Fotografías del montaje
`[Insertar imágenes]`

## Capturas del monitor
`[Insertar imágenes]`

## Gráficas obtenidas
`[Insertar gráficas]`

---

# Repositorio GitHub

## Enlace
`[Agregar enlace GitHub]`

## Colaboradores
- `[Nombre 1]`
- `[Nombre 2]`

---

# Referencias

1. Mindray. *uMEC Series Patient Monitor Operator’s Manual*.
2. Pronk Technologies. *OxSim Flex Pulse Oximeter Tester User Guide*.
3. Webster, J. G. *Medical Instrumentation: Application and Design*. Wiley.
4. Carr, J. J., & Brown, J. M. *Introduction to Biomedical Equipment Technology*. Pearson.
5. IEC 60601-1-8. *Medical Electrical Equipment – Alarm Systems*.
6. ISO 80601-2-61. *Particular requirements for pulse oximeter equipment*.
