# Metodología de Pseudomentefactos para Objetos y Artefactos Técnicos

Este documento formaliza la metodología para construir **Pseudomentefactos** aplicados a dispositivos de hardware, software, instrumentos de medición y artefactos tecnológicos físicos.

---

## 1. Naturaleza Ontológica del Pseudomentefacto

En la Pedagogía Conceptual clásica, los mentefactos se concibieron para abstracciones científicas, matemáticas y nocionales (*Gravedad, Triángulo, Célula, Democracia*).

Sin embargo, en el ámbito contemporáneo de la ciencia y la ingeniería, se interactúa a diario con **objetos físicos manufacturados, instrumentos de medición y dispositivos tecnológicos** (*Microscopio, Termómetro, Brújula, Microcontrolador, Motor, Computadora*).

Forzar un artefacto manufacturado dentro de las categorías de un mentefacto puramente platónico genera inconsistencias lógicas (como atribuirles "esencia inmutable" o "subclases metafísicas"). Esto se resuelve mediante la **Mutación Estructural a Lógica Técnica y Funcional**.

---

## 2. Tabla de Mutación Estructural Obligatoria

Cuando el semáforo ontológico marca **🟡 Luz Ámbar**, la estructura de las 4 operaciones mentefactuales muta de inmediato:

| Operación | En Mentefacto Conceptual (🟢 Luz Verde) | En Pseudomentefacto Técnico (🟡 Luz Ámbar) |
| :--- | :--- | :--- |
| **P1. Supraordinada** | Género próximo taxonómico (*¿Qué es?*). | **Función técnica u objeto técnico general** (*¿Para qué sirve?*). |
| **P2.x Isoordinadas** | Notas esenciales ontológicas (ADN del concepto). | **Principios de funcionamiento y arquitectura de interfaz privativa** (superando la prueba de sustracción). |
| **P3.x Exclusiones** | Conceptos hermanos abstractos directos. | **Artefactos alternativos que cumplen la MISMA función técnica** bajo otra arquitectura interna. |
| **P4. Infraordinadas** | Subclases o divisiones conceptuales lógicas. | **Variantes técnicas de fabricación, diseño constructivo o factor de forma**. |

---

## 3. Las Reglas de Validación en Pseudomentefactos

### 1. Supraordinada Funcional
La supraordinada de un artefacto es su **función técnica u objeto técnico superior** (ej. para *Microscopio*: *Instrumento de magnificación óptica*; para *Arduino*: *Plataforma de prototipado con microcontrolador*). Prohibido asignarle géneros abstractos vacíos.

### 2. Isoordinadas: Principios Operativos vs. Accesorios
* **Principio**: Las isoordinadas describen la arquitectura de interfaz y la dinámica funcional que hacen al artefacto operar.
* **Prueba de Sustracción de Accesorios**:  
  *Pregunta*: *«Si al artefacto le retiro este componente, ¿sigue siendo la misma plataforma/artefacto?»*  
  Si le quito el cable USB, el chip serial o la pantalla y sigue cumpliendo su propósito con sus interfaces nativas, ese componente es un **accesorio contingente** y queda vetado de las isoordinadas. Solo permanecen los principios operativos inalienables (ej. la capa de abstracción de hardware y el pinout estandarizado).

### 3. Exclusiones: Mismo Nivel Funcional (Anti-Rival Didáctico)
* **Regla estricta**: Las exclusiones deben ser artefactos que compitan directamente bajo la **misma función técnica**.
* **Prohibición de mezcla jerárquica**:  
  * *Error común*: Comparar una placa de microcontrolador (*Arduino*) con una computadora monoplaca con sistema operativo (*Raspberry Pi*) o con un controlador lógico industrial de riel DIN (*PLC*). Son rivales didácticos de divulgación informal, no hermanos del mismo nivel técnico.
  * *Corrección*: Se debe contrastar con otras plataformas de prototipado con microcontrolador (ej. *ESP32 / NodeMCU*, *STM32 Nucleo*, *Raspberry Pi Pico*).

### 4. Infraordinadas: Variantes Constructivas y Factor de Forma
Las infraordinadas de un artefacto no son subclases platónicas; son sus **variantes de manufactura, factores de forma o métodos de integración física** (ej. placas estándar para shields apilables, placas compactas para protoboard/PCB, placas modulares para IoT y batería).

---

## 4. Estructura Abstracta del Pseudomentefacto

```text
               [ FUNCIÓN TÉCNICA U OBJETO SUPERIOR: F ] (P1)
                                       │
               ┌───────────────────────┴───────────────────────┐
               │                                               │
 [ P2: PRINCIPIOS Y ARQUITECTURA ]                    [ P3: ARTEFACTOS HERMANOS ]
 • Principio operativo inalienable                    ≠ E_1 (Misma función técnica
 • Arquitectura de interfaz privativa                   con arquitectura interna distinta)
               │                                      ≠ E_2 (Misma función técnica
               │                                        con método operativo alterno)
               │                                               │
               └───────────────────────┬───────────────────────┘
                                       ▼
                             [ ARTEFACTO CENTRAL: A ]
                                       │
                 [ CRITERIO: Variable de diseño o integración ]
                                       │
         ┌─────────────────────────────┼─────────────────────────────┐
         ▼                             ▼                             ▼
[ VARIANTE CONSTRUCTIVA 1 ]   [ VARIANTE CONSTRUCTIVA 2 ]   [ VARIANTE CONSTRUCTIVA 3 ]
(Formato técnico v_1)         (Formato técnico v_2)         (Formato técnico v_3)
```
