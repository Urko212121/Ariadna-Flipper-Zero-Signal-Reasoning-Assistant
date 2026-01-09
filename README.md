Ariadna – Flipper Zero Signal Reasoning Assistant

Ariadna es una aplicación (FAP) para Flipper Zero que analiza, clasifica y documenta señales de forma determinista y reproducible. No ejecuta ataques ni emulaciones automáticas: razona y explica.

Características

Clasificación determinista (Sub-GHz / NFC / IR)

Métricas reales: entropía y estabilidad

Memoria histórica persistente

Detección de señales ya observadas

Exportación automática de informes


Requisitos

Flipper Zero con firmware oficial o compatible con FAPs

SDK de Flipper (fbt)

Tarjeta SD


Instalación paso a paso

1. Clona el repositorio del firmware de Flipper.


2. Copia la carpeta ariadna dentro de applications_user/.


3. Desde la raíz del firmware ejecuta:

./fbt fap_ariadna


4. Copia el .fap generado a la SD del Flipper (carpeta apps).


5. Reinicia el dispositivo.



Uso

1. Abre Ariadna desde el menú de aplicaciones.


2. Selecciona el tipo de análisis (Sub-GHz, NFC o IR).


3. Observa el informe generado:

Clasificación

Razonamiento

Recomendación

Estado (nuevo / conocido)



4. Al finalizar el análisis, el informe se guarda automáticamente en:

/ext/ariadna_report.txt



Flujo recomendado

Ejecuta Ariadna antes de intentar clonar o emular.

Usa el diagnóstico para decidir si continuar o descartar.

Adjunta el informe exportado a tus notas o informes de auditoría.


Notas técnicas

No se almacenan datos crudos de señales.

La persistencia está limitada para proteger la flash.

Todas las decisiones son reproducibles.


Licencia

Uso educativo y profesional en contextos autorizados. 
