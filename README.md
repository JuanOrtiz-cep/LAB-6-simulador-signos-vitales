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

# 2. Procedimiento Experimental

1. Despúes de encender el uMEC100, se configura en modo monitor y se conecta el sensor SpO₂ al OxSim OX-1. Una vez allí se realizan los ítems del 4-10 cuyos resultados se ven en la tabla, siendo los tiempos de respuesta en segundos aquel tiempo que tardó el monitor en mostrar el resultado correcto hasta la activación de la alarma respectiva propuesta por la guía.


<img width="918" height="270" alt="image" src="https://github.com/user-attachments/assets/ad6a26f3-f572-48ae-89d8-9882518687e7" />


<img width="953" height="161" alt="image" src="https://github.com/user-attachments/assets/e41bca0d-f7dd-4370-8183-5c7dbb9843bb" />


4.Configure el OxSim para simular un paciente bradicárdico (40 bpm, SpO2 =
95%) y calcule los errores absoluto y porcentual para cada variable en relación
con los mostrados en el uMEC100.
5. Observe y registre la forma de onda de la señal fotopletismográfica que
aparece en la pantalla del uMEC100.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/835c551e-8274-474b-8394-d9eab8d30a7a" />
Fotopletismografía 40bpm, SpO2=95%

En este paso, desde el momento que se puso la opción 40 bpm, SpO2 =
95% en el OxSim, el uMEC100 tardó aproxímadamente 6 segundos en mostrar en el monitor ambas variables correctamente. 

En este ítem no se utilizó ningún tiempo para comparar, siendo así que no se calcula el error, más allá de tener en cuenta que se llegó al valor esperado en aproxímadamente 6 segundos.


6. En el uMEC100, establezca el límite inferior de alarma de SpO2 a 90%.
   
7. Ajuste el OxSim hasta poder simular una frecuencia cardíaca de 80 bpm y
SPO2 = 85%. A partir de ese instante, cuente 5 segundos y, al cabo de ese
tiempo, verifique y registre la activación de la alarma sonora/visual en el
uMEC100. Nuevamente, calcule los errores absoluto y porcentual para cada
variable en relación con los mostrados en el uMEC100.

Desde el momento que se puso la opción 80 bpm y SPO2 = 85% en el OxSim, el uMEC100 tardó aproxímadamente 6 segundos en mostrar la correctamente la variable a medir (SPO2 = 85%), mismo tiempo que tardó la respectiva alarma en activarse. A los 5 segundos el SpO2 estaba en: 82%. 

SpO2:

Error absoluto: 85-82= 3

Error porcentual: ((85-82)/85)*100 = 3.529%

Bmp

Error absoluto: 80-64 = 16

Error porcentual: ((80-64)/80)*100 = 20%

8. Configure la alarma de límite superior en el uMEC100 a 97%.
 
9. Ajuste el OxSim hasta poder simular una SPO2 = 99% (modo “Low Perfusion”).
A partir de ese instante, cuente 5 segundos y, al cabo de ese tiempo, verifique
y registre la activación de la alarma sonora/visual en el uMEC100.
Nuevamente, calcule los errores absoluto y porcentual para cada variable en
relación con los mostrados en el uMEC100. ¿La onda fotopletismográfica se
distorsiona?

Desde el momento que se puso la opción SPO2 = 99% (modo “Low Perfusion”) en el OxSim, el uMEC100 tardó aproxímadamente 13 segundos en mostrar la correctamente la variable a medir (SPO2 = 99%), y la alarma tardó 11 más en activarse despúes de mostrar el valor. A los 5 segundos de poner el respectivo modo el SpO2 estaba en: 87%. 

SpO2:

Error absoluto: 99- 87 = 12

Error porcentual: ((99-87)/99)*100 = 12.121%

En el momento exacto que la alarma se activó para Low Perfusion (SpO2 alto<97) la onda fotopletismográfica se veía así, se vé que cambia respecto al modo anterior, sin embargo al menos para ese instante no se ve "distorsionada".

<img width="1080" height="567" alt="image" src="https://github.com/user-attachments/assets/af4dbdcf-631a-4ad4-9e48-8e51657b90ce" />


10. Con un valor de SpO2 = 95%, genere una taquicardia (140 bpm) con el OxSim
y registre la onda en el uMEC100. ¿Se dispara la alarma de frecuencia
cardíaca elevada? Nuevamente, calcule los errores absoluto y porcentual para
cada variable en relación con los mostrados en el uMEC100.

Al poner la opción de SpO2 = 95% y 140 bpm, lo esperable es que aparezca la alarma para taquicardia, el uMEC100 tardó aproxímadamente 14 segundos en pasar de 80bpm a 140bpm, y la alarma tardó 8 segundos más en activarse despúes de mostrar el valor de 140bmp. A los 5 segundos de poner el respectivo modo el SpO2 estaba en: 87%. 

SpO2:

Error absoluto: 95-98 = -3, valor absoluto = 3

Error porcentual: ((95-98)/95)*100 = 3.157%

Bmp

Error absoluto: 140-87 = 53

Error porcentual: ((140-87)/140)*100 = 37.85%

---

### FIN PARTE BBBBBBBBBBBBBBBB

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
