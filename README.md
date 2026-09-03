[README.md](https://github.com/user-attachments/files/31424671/README.md)
# 🥤 Análisis Funcional y Arquitectura de Interfaces: Licuadora Oster® (All-Metal Drive)

Este repositorio contiene el desglose técnico, análisis de sistemas y modelado de **interfaces de entrada y salida (I/O)** aplicados al diseño industrial y funcional de una licuadora electrodoméstica clásica de alto rendimiento (**Oster® All-Metal Drive**).

---

## 📌 Tabla de Contenidos
1. [Descripción del Proyecto](#-descripción-del-proyecto)
2. [Lámina Visual del Sistema](#-lámina-visual-del-sistema)
3. [Desglose Detallado de Interfaces](#-desglose-detallado-de-interfaces)
   - [1. Interfaces de Entrada (Input)](#1-interfaces-de-entrada-input)
   - [2. Interfaces de Salida (Output)](#2-interfaces-de-salida-output)
4. [Mecanismos Internos y Acople Tecnológico](#-mecanismos-internos-y-acople-tecnológico)
5. [Estructura del Repositorio](#-estructura-del-repositorio)
6. [Autores y Licencia](#-autores-y-licencia)

---

## 📖 Descripción del Proyecto

El objetivo de este proyecto es desglosar un electrodoméstico de uso cotidiano bajo la óptica de la **Teoría General de Sistemas**, **Ingeniería Mecánica/Eléctrica** y **Diseño de Interacción (HCI)**. Se analizan los flujos de materia, energía e información que cruzan las fronteras del sistema.

```
       ┌─────────────────────────────────────────────────────────┐
       │                   SISTEMA: LICUADORA                    │
ENTRADAS                                                       SALIDAS
───────► [Alimentos/Líquidos] ──► [ Transformación ] ──────────► [Mezcla / Emulsión]
───────► [Energía Eléctrica]  ──► [ Mecánica/Corte ] ──────────► [Calor Disipado]
───────► [Control de Usuario] ──► [ Transmisión    ] ──────────► [Ruido y Vibración]
       └─────────────────────────────────────────────────────────┘
```

---

## 🖼 Lámina Visual del Sistema

El proyecto cuenta con una infografía/lámina técnica representativa:


## ⚙ Desglose Detallado de Interfaces

### 1. Interfaces de Entrada (Input)

Las entradas corresponden a todos los insumos de materia, energía y comandos de usuario requeridos para el funcionamiento del equipo:

* **1.1 Entrada de Materia / Ingredientes (Mecánica):**
  * **Vaso / Jarra de Vidrio Refractario (Borosilicato):** Capacidad volumétrica graduada de hasta 6 tazas / 1.4 L. Resistente a choque térmico.
  * **Tapa Superior con Sobre-tapa Dosificadora:** Permite la alimentación continua o adición de líquidos/ingredientes secundarios durante el ciclo sin salpicaduras.
* **1.2 Entrada de Energía (Eléctrica):**
  * **Cable de Alimentación y Enchufe:** Entrada de corriente alterna ($120\text{V} / 220\text{V} - 50/60\text{Hz}$).
  * **Potencia Nominal:** Motor universal con un consumo/potencia pico entre $450\text{W}$ y $700\text{W}$.
* **1.3 Interfaz de Usuario / Panel de Control (Operativa - HMI):**
  * **Potonera / Interruptores Táctiles:** Botones mecánicos tipo basculante o pulsador (Apagado `O`, Velocidades continuas `1 - Sopas`, `2 - Jugos`, `3 - Salsas`, y Modos de `Pulso Bajo / Pulso Alto`).
  * **Feedback Táctil:** Retorno mecánico háptico (clic) que confirma el enclave de la velocidad seleccionada.
* **1.4 Mecanismo de Acople y Seguridad (Mecánica):**
  * Encastre base-vaso con guías de alineación para garantizar la concentricidad del rotor y evitar desacoples dinámicos.

---

### 2. Interfaces de Salida (Output)

Las salidas representan las transformaciones físicas finales, así como las pérdidas y respuestas del sistema hacia el entorno:

* **2.1 Salida de Producto Procesado (Materia/Fluídica):**
  * **Pico Vertedor (Jarra):** Geometría optimizada para el flujo laminar y servido sin goteo.
  * **Producto Final:** Emulsiones homogéneas, purés, jugos, trituración de hielo y mezclas consistentes.
* **2.2 Sistema de Corte y Vórtice (Mecánica / Hidrodinámica):**
  * **Cuchillas de Acero Inoxidable:** 4 aspas helicoidales multifunción de alta resistencia a la corrosión y desgaste.
  * **Generación de Vórtice:** El diseño interior de la jarra redirige los sólidos continuamente hacia la zona de corte inferior.
* **2.3 Salidas Térmicas y Acústicas (Energéticas/Parásitas):**
  * **Disipación Térmica:** Rejillas de ventilación forzada en la base del motor para evacuar el calor por convección.
  * **Emisión Sonora y Vibratoria:** Ruido operativo en rango de $75 - 85\text{ dB(A)}$, amortiguado parcialmente por topes de goma antideslizantes.
* **2.4 Estabilidad y Soporte Estructural:**
  * **Patas Antideslizantes de Elastómero:** Transmisión y absorción de vibraciones dinámicas hacia la superficie de apoyo.

---

## 🔩 Mecanismos Internos y Acople Tecnológico

* **Sistema All-Metal Drive®:** Acople directo metal-contra-metal entre el eje del motor y la base de las cuchillas. Evita el desgaste prematuro habitual en sistemas de plástico o engranajes blandos, garantizando una transferencia de torque óptima ($100\%$ eficiencia en torque mecánico).

```
   [ Motor Eléctrico ] ──( Eje Metálico )──► [ Acople All-Metal Drive ] ──► [ Cuchillas 4 Aspas ]
```

---

## 📂 Estructura del Repositorio

```bash
├── README.md                 # Documentación principal del sistema
├── docs/
│   ├── assets/               # Diagramas, láminas e imágenes vectoriales
│   │   └── lamina_interfaces_licuadora.jpg
│   └── especificacion_tecnica.pdf # Ficha técnica detallada
└── src/                      # Modelados 3D / Diagramas de bloques en código (si aplica)
```

---

## 📄 Licencia

Distribuido bajo la Licencia MIT. Consulta el archivo `LICENSE` para más información.
