---
title: "Unidad 2: Actuadores Avanzados"
layout: post
permalink: /unidad-2-actuadores-avanzados/
background: '#1a5'

slides:
  - title: "Unidad 2: Actuadores Avanzados"
    slide-data: |
      Los actuadores son dispositivos capaces de transformar diversas formas de energía en movimiento. Se clasifican en tres grandes grupos:
      - Actuadores Eléctricos
      - Actuadores Mecánicos
      - Actuadores Hidráulicos
      También existen variantes como los actuadores neumáticos y piezoeléctricos.

  - title: "2.1 Actuadores Eléctricos"
    slide-data: "Los actuadores eléctricos convierten la energía eléctrica en movimiento mecánico, siendo ideales para aplicaciones donde se requiere precisión y control avanzado."

  - title: "2.1.1 Tipos de Actuadores Eléctricos"
    slide-data: |
      - **Motores DC**: Motores de corriente continua que ofrecen control de velocidad mediante variación de voltaje.
      - **Motores paso a paso**: Dividen el movimiento en pasos discretos, lo que proporciona un control preciso de la posición.
      - **Servomotores**: Actuadores controlados por retroalimentación para aplicaciones que requieren alta precisión en posición y velocidad.
      - **Actuadores lineales eléctricos**: Convierte el movimiento rotatorio de un motor en movimiento lineal.

  - title: "2.1.2 Principio de Funcionamiento"
    slide-data: "Los actuadores eléctricos convierten la energía eléctrica en energía mecánica a través de campos electromagnéticos, creando movimiento rotativo o lineal."

  - title: "2.1.3 Características de los Actuadores Eléctricos"
    slide-data: |
      - **Alta precisión**: Especialmente en servomotores y motores paso a paso.
      - **Control avanzado**: Posibilidad de ajustar velocidad, aceleración y posición.
      - **Eficiencia energética**: Consumo moderado de energía.

  - title: "2.1.4 Modos de Comunicación"
    slide-data: |
      - **PWM (Modulación por Ancho de Pulso)**: Común en servomotores y motores DC para controlar velocidad y posición.
      - **Comunicación serial**: Utilizado en sistemas más complejos para transmitir comandos de control.

  - title: "2.2 Actuadores Mecánicos"
    slide-data: "Los actuadores mecánicos convierten fuerzas mecánicas en movimiento, siendo ideales para sistemas que requieren simplicidad y robustez."

  - title: "2.2.1 Tipos de Actuadores Mecánicos"
    slide-data: |
      - **Engranajes**: Transmiten movimiento rotatorio entre ejes mediante la interacción de dientes.
      - **Resortes**: Almacenan energía mecánica y liberan movimiento bajo compresión o tensión.
      - **Poleas y correas**: Transforman el movimiento rotativo en lineal o para cambiar la dirección del movimiento.
      - **Levas**: Convertir movimiento rotatorio en un movimiento alternante o oscilante.

  - title: "2.2.2 Principio de Funcionamiento"
    slide-data: "El movimiento se genera mediante la interacción física de los componentes mecánicos, como engranajes o resortes."

  - title: "2.2.3 Características de los Actuadores Mecánicos"
    slide-data: |
      - **Durabilidad**: Los componentes mecánicos son resistentes y adecuados para aplicaciones de larga duración.
      - **Bajo costo**: Generalmente más económicos que otros tipos de actuadores.
      - **Fiabilidad**: Ideales para aplicaciones donde no se requiere precisión extrema.

  - title: "2.2.4 Modos de Comunicación"
    slide-data: "Los actuadores mecánicos generalmente se controlan de forma manual o mediante mecanismos automáticos simples."

  - title: "2.3 Actuadores Hidráulicos"
    slide-data: "Los actuadores hidráulicos utilizan fluidos presurizados para generar fuerzas muy grandes, adecuados para aplicaciones industriales pesadas."

  - title: "2.3.1 Tipos de Actuadores Hidráulicos"
    slide-data: |
      - **Cilindros hidráulicos**: Generan movimiento lineal a partir de la presión de un fluido.
      - **Motores hidráulicos**: Convierte la presión del fluido en movimiento rotativo.

  - title: "2.3.2 Principio de Funcionamiento"
    slide-data: "La presión de un fluido empuja un pistón dentro de un cilindro, generando un movimiento lineal o rotativo dependiendo del diseño."

  - title: "2.3.3 Características de los Actuadores Hidráulicos"
    slide-data: |
      - **Fuerza extrema**: Los actuadores hidráulicos pueden generar fuerzas mucho mayores que los eléctricos o mecánicos.
      - **Precisión limitada**: No son tan precisos como otros tipos de actuadores debido a la compresibilidad del fluido.
      - **Requiere mantenimiento**: Los sistemas hidráulicos pueden tener fugas y requieren monitoreo constante.

  - title: "2.3.4 Modos de Comunicación"
    slide-data: |
      - **Válvulas y controladores de flujo**: Controlan la presión y el flujo del fluido para regular el movimiento.
      - **Sistemas automatizados**: Utilizan sensores para retroalimentar el control del actuador.

  - title: "2.4 Actuadores Neumáticos"
    slide-data: "Utilizan aire comprimido para generar movimiento, ideales para aplicaciones que requieren respuesta rápida y fuerza moderada."

  - title: "2.4.1 Tipos de Actuadores Neumáticos"
    slide-data: |
      - **Cilindros neumáticos**: Generan movimiento lineal con aire comprimido.
      - **Motores neumáticos**: Generan movimiento rotativo a partir de aire comprimido.

  - title: "2.4.2 Principio de Funcionamiento"
    slide-data: "El aire comprimido mueve un pistón dentro de un cilindro, generando un movimiento rápido y eficiente."

  - title: "2.4.3 Características de los Actuadores Neumáticos"
    slide-data: |
      - **Rápida respuesta**: El aire comprimido permite movimientos rápidos y eficientes.
      - **Mediana fuerza**: Generan menos fuerza que los hidráulicos, pero más que los eléctricos.
      - **Menor precisión**: Similar a los hidráulicos, los actuadores neumáticos tienen una precisión limitada.

  - title: "2.4.4 Modos de Comunicación"
    slide-data: |
      - **Válvulas y reguladores de presión**: Controlan el flujo de aire comprimido.
      - **Sistemas automatizados**: Utilizan sensores para regular el movimiento.

  - title: "Fin de la Presentación"
    slide-data: "¡Gracias por su atención! ¿Preguntas?"
---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
  <h1>{{slide.title}}</h1>
  <p>{{ slide.slide-data | markdownify }}</p>
</section>               
{% endfor %}
