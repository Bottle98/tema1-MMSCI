# 2. Componentes electrónicos ⚡

Los **componentes electrónicos** son los elementos que forman los circuitos eléctricos. Cada uno tiene una **función diferente**, como controlar el paso de corriente, almacenar energía o modificar señales.

---

## 2.1. Resistencias 🌀

El **componente eléctrico encargado de limitar o reducir la corriente eléctrica** en un circuito se llama **resistencia** o **resistor**. Sirve para **proteger los demás componentes**, controlar la **intensidad** y **dividir tensiones**.

---

### Código de colores 🎨

Cada resistencia tiene unas **bandas de colores** que indican su valor en ohmios (Ω), su **tolerancia** y, a veces, su **coeficiente térmico** (en resistencias de alta precisión).

| Color | Cifra | Multiplicador | Tolerancia | Coef. térmico (ppm/°C) |
|:------|:------|:--------------|:-----------|:------------------------|
| **Negro** | 0 | ×1 | — | — |
| **Marrón** | 1 | ×10 | ±1% | 100 |
| **Rojo** | 2 | ×100 | ±2% | 50 |
| **Naranja** | 3 | ×1 000 | — | 15 |
| **Amarillo** | 4 | ×10 000 | — | 25 |
| **Verde** | 5 | ×100 000 | ±0,5% | — |
| **Azul** | 6 | ×1 000 000 | ±0,25% | 10 |
| **Violeta** | 7 | ×10 000 000 | ±0,1% | 5 |
| **Gris** | 8 | — | — | — |
| **Blanco** | 9 | — | — | 1 |
| **Dorado** | — | ×0,1 | ±5% | — |
| **Plateado** | — | ×0,01 | ±10% | — |
| **Ninguno** | — | — | ±20% | — |

!!! tip "💡 Cómo leer una resistencia"
    - **4 bandas:** 2 cifras + multiplicador + tolerancia  
    - **5 bandas:** 3 cifras + multiplicador + tolerancia  
    - **6 bandas:** 3 cifras + multiplicador + tolerancia + coeficiente térmico  

<p align="center">
  <img src="../Images/resistencias-bandas.png" alt="Tabla de colores y ejemplos de resistencias de 4, 5 y 6 bandas" width="420">
</p>

<p align="center"><em>Ejemplo de resistencias de 4, 5 y 6 bandas con su respectiva codificación de colores.</em></p>

!!! example "Ejemplo práctico"
    - **Resistencia de 4 bandas:** Marrón, Rojo, Naranja, Dorado → 12 × 1 000 = **12 000 Ω = 12 kΩ**, tolerancia ±5%.  
    - **Resistencia de 5 bandas:** Marrón, Rojo, Negro, Rojo, Dorado → 120 × 100 = **12 000 Ω**, tolerancia ±5%.  
    - **Resistencia de 6 bandas:** Igual que la de 5, pero con una sexta banda que indica el **coeficiente térmico**.

!!! note "Representación en esquemas"
    En los circuitos eléctricos, la resistencia se representa con este símbolo:

    <p align="center">
      <img src="../Images/simbolo-resistencia.png" alt="Símbolo de resistencia eléctrica en esquemas" width="180">
    </p>

    <p align="center"><em>Símbolo eléctrico internacional utilizado para representar una resistencia.</em></p>

---

### 2.1.1. Resistencias SMD (Surface Mount Device) ⚙️

Las **resistencias SMD** son resistencias de **montaje superficial**, utilizadas en placas electrónicas modernas. En lugar de colores, usan **números o letras** impresos directamente sobre su superficie.

| Ejemplo | Explicación | Valor resultante |
|----------|-------------|------------------|
| **212** | 21 × 10² | **2 100 Ω (2,1 kΩ)** |
| **3R4** | 3,4 Ω (la "R" marca la coma decimal) | **3,4 Ω** |
| **R56** | 0,56 Ω | **0,56 Ω** |
| **1283** | 128 × 10³ | **128 000 Ω (128 kΩ)** |

<p align="center">
  <img src="../Images/resistencias-smd.png" alt="Ejemplo de resistencia SMD con código numérico" width="300">
</p>

<p align="center"><em>Ejemplo real de resistencia SMD con código numérico impreso.</em></p>

!!! info "📘 Ayuda de vocabulario"
    - **SMD:** *Surface Mount Device* → *Componente de montaje superficial*.  
    - **Ω (Ohm):** unidad de medida de la resistencia.  
    - **kΩ / MΩ:** kiloohmios / megaohmios (1 000 y 1 000 000 Ω).

---

### 2.1.2. Codificación EIA-96 🔢

En resistencias de **alta precisión**, se usa la **codificación EIA-96**, que combina un **número de tres cifras** con una **letra**. Cada número corresponde a un valor base, y la letra indica el multiplicador.

📍 **Ejemplo:**

- Código **01C** → valor base “01” y multiplicador “C”.  
- Según la tabla EIA-96, corresponde a **100 × 100 = 10 000 Ω (10 kΩ)**.

<p align="center">
  <img src="../Images/codificacion-eia96.png" alt="Tabla de codificación EIA-96 con ejemplo de resistencia SMD" width="350">
</p>

<p align="center"><em>Tabla EIA-96: resistencias SMD de precisión con 1% de tolerancia y ejemplo del código 01C.</em></p>

!!! note "Recuerda"
    - Cuantas **más bandas** o **más dígitos**, **mayor precisión**.  
    - Las **SMD** y **EIA-96** se usan sobre todo en equipos electrónicos modernos por su pequeño tamaño.

---

## 2.2. Potenciómetros 🎚️

Los **potenciómetros** son resistencias especiales cuyo valor **no es fijo**, sino **variable**. Esto significa que pueden **aumentar o disminuir la resistencia** según se gire o desplace su eje.

Un ejemplo muy común es el **regulador de volumen** de una radio o un altavoz: al girarlo, cambia la resistencia y con ello **la cantidad de corriente que pasa**, controlando así el volumen o la intensidad de luz en una lámpara.

<p align="center">
  <img src="../Images/potenciometros.png" alt="Estructura interna y ejemplo de potenciómetro real" width="380">
</p>

<p align="center"><em>Partes de un potenciómetro y su representación física. Se utiliza en reguladores de volumen, brillo o velocidad.</em></p>

!!! tip "💡 En resumen"
    - Un potenciómetro **regula la corriente** mediante una resistencia variable.  
    - Se usa en **reguladores de volumen, brillo o velocidad**.  
    - Internamente funciona como una resistencia con un contacto móvil que se desliza sobre ella.

---

## 2.3. Condensadores ⚡

Un **condensador** (también llamado *capacitor*) es un componente que **almacena corriente eléctrica** durante un breve periodo de tiempo. Su función principal es **acumular y liberar energía eléctrica** cuando se necesita.

La cantidad de carga que puede almacenar se llama **capacitancia** o **capacidad**, y se mide en **faradios (F)**, aunque normalmente se usan valores más pequeños como **microfaradios (µF)**, **nanofaradios (nF)** o **picofaradios (pF)**.

!!! note "📘 Código de colores"
    Algunos condensadores utilizan un **código de colores** similar al de las resistencias, donde las bandas indican:
    
    - **1ª banda:** primer dígito  
    - **2ª banda:** segundo dígito  
    - **3ª banda:** multiplicador  
    - **4ª banda (opcional):** tolerancia  
    - **5ª banda (opcional):** tensión máxima de trabajo  

<p align="center">
  <img src="../Images/codigo-colores-condensador.png" alt="Código de colores para identificar el valor de los condensadores" width="430">
</p>

<p align="center"><em>Ejemplo de código de colores en condensadores, indicando valor, tolerancia y tensión máxima de trabajo.</em></p>

---

### Tipos de condensadores 🔋

Los condensadores se clasifican según su **material, forma y función**. Los más comunes son:

| Tipo | Características | Ejemplo de uso |
|------|------------------|----------------|
| **Cerámico** | Pequeños, no polarizados. Baratos y precisos. | Circuitos digitales y osciladores. |
| **Electrolítico** | Polarizados, mayor capacidad. | Fuentes de alimentación. |
| **Tántalo (SMD)** | Estables y compactos, algo más caros. | Dispositivos portátiles y placas electrónicas. |
| **Variables** | Permiten ajustar su capacidad. | Sintonizadores de radio o antenas. |

<p align="center">
  <img src="../Images/condensadores.png" alt="Ejemplos de condensadores: tántalo, axial y radial" width="420">
</p>

<p align="center"><em>Condensadores más comunes: de tántalo (SMD), electrolítico axial y electrolítico radial.</em></p>

---

### Representación en esquemas 📈

El **símbolo del condensador** depende de su tipo:

<p align="center">
  <img src="../Images/simbolos-condensadores.png" alt="Símbolos eléctricos de los condensadores" width="330">
</p>

<p align="center"><em>Símbolos eléctricos de condensadores: no polarizado, electrolítico, variable y ajustable.</em></p>

!!! info "💬 Vocabulario útil"
    - **Capacitancia / Capacidad:** cantidad de carga que puede almacenar.  
    - **Polarizado:** tiene un polo positivo (+) y otro negativo (−), como los electrolíticos.  
    - **No polarizado:** se puede conectar en cualquier sentido.  
    - **Tolerancia:** margen de error en la capacidad real del condensador.

---

## 2.4. Diodos 🔺

Un **diodo** es un **dispositivo semiconductor** que permite el paso de la corriente eléctrica **en una sola dirección** cuando se aplica una diferencia de potencial. Su función principal es **dejar pasar la corriente en un sentido y bloquearla en el contrario**, lo que lo convierte en un componente esencial en los circuitos electrónicos.

Una de sus aplicaciones más comunes es **transformar la corriente alterna (CA)** en **corriente continua (CC)**, proceso conocido como **rectificación**.

<p align="center">
  <img src="../Images/simbolos-diodos.png" alt="Símbolos eléctricos de diferentes tipos de diodos" width="500">
</p>

<p align="center"><em>Símbolos eléctricos de los principales tipos de diodos: rectificador, Zener, LED, fotodiodo, Schottky, túnel, varicap y láser.</em></p>

!!! tip "💡 Tipos y usos más comunes"
    - **Diodo rectificador:** convierte la corriente alterna en continua.  
    - **Diodo Zener:** regula el voltaje en los circuitos.  
    - **LED (Light Emitting Diode):** emite luz.  
    - **Fotodiodo:** detecta la luz.  
    - **Diodo Schottky:** ofrece conmutación rápida y baja caída de tensión.  
    - **Diodo láser:** genera luz láser en lectores y sensores.

---

## 2.5. Leds 💡

El **LED** (*Light-Emitting Diode*) o **diodo emisor de luz**, es un tipo especial de diodo que **emite luz** cuando la corriente eléctrica **circula a través de él**. El color de la luz depende del **material semiconductor** utilizado.

Los **LED** se han vuelto muy populares por su **bajo consumo**, **larga duración** y su uso en **pantallas, iluminación y decoración**.

<p align="center">
  <img src="../Images/leds.png" alt="Diodos LED de diferentes formas y colores" width="500">
</p>

<p align="center"><em>Ejemplos de diodos LED: distintos tamaños, colores y encapsulados.</em></p>

!!! note "📘 Vocabulario"
    - **LED:** *Light-Emitting Diode* → diodo emisor de luz.  
    - **OLED:** *Organic Light-Emitting Diode* → diodo orgánico.  
    - **AMOLED:** versión activa usada en pantallas modernas.  

!!! info "🔆 Tipos de LED"
    - **Estándar:** pequeños, usados en indicadores luminosos.  
    - **Alta potencia:** para iluminación general.  
    - **RGB:** combinan rojo, verde y azul para emitir distintos colores.  
    - **OLED:** diodos orgánicos empleados en pantallas y televisores.

---

## 2.6. Transistores ⚙️

Un **transistor** es un **componente semiconductor** que puede **amplificar** o **interrumpir** la corriente eléctrica. Gracias a ellos, fue posible el desarrollo de los **ordenadores personales** y de toda la **electrónica moderna**.

Existen diferentes tipos de transistores, como los **NPN**, **PNP**, **Darlington** o **MOSFET**, y se utilizan en infinidad de aparatos: radios, teléfonos, ordenadores o televisores.

<p align="center">
  <img src="../Images/encapsulados-transistores.png" alt="Ejemplos de encapsulados de transistores" width="450">
</p>

<p align="center"><em>Ejemplos de encapsulados de transistores: TO-3, TO-18, TO-92, TO-220, DIL y muchos más.</em></p>

!!! note "🔎 Tipos principales"
    - **NPN y PNP:** los más comunes en electrónica básica.  
    - **Darlington:** dos transistores unidos para aumentar la ganancia.  
    - **MOSFET:** usados en circuitos de potencia o control de motores.  
    - **FET:** controlados por tensión, empleados en amplificadores analógicos.

---

### Representación en esquemas 📈

<p align="center">
  <img src="../Images/simbolo-transistor.png" alt="Símbolo del transistor NPN" width="180">
</p>

<p align="center"><em>Símbolo eléctrico del transistor NPN, con sus tres terminales: base (B), colector (C) y emisor (E).</em></p>

!!! tip "💡 Curiosidad"
    El **transistor** fue inventado en 1947 por el equipo de **Bell Labs**. Su creación sustituyó las válvulas de vacío, reduciendo el tamaño y consumo de los equipos electrónicos. Hoy, un microprocesador puede contener **millones de transistores** en un solo chip.