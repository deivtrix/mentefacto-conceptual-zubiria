# Especificación Gráfica del SVG Canónico para Mentefactos

Este documento define la geometría vectorial, coordenadas, paleta de colores y reglas de renderizado XML para la generación del ideograma SVG canónico.

---

## 1. Geometría General y Proporciones

* **Lienzo**: `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 850 560" width="100%" height="auto">`
* **Tipografía**: `font-family="system-ui, -apple-system, sans-serif"`

```
                      ┌──────────────────────┐
                      │  P1. SUPRAORDINADA   │ (Arriba: Y=40, W=200, H=50)
                      └──────────▲───────────┘
                                 │ Conector con flecha (#0284c7)
                      ╔══════════╧═══════════╗      ≠      ┌──────────────────────┐
┌──────────────────┐  ║                      ║────────────►│  P3.1 EXCLUSIÓN 1    │ (Derecha: X=600, W=210)
│ P2.1 ISOORDINADA │◄─╢   CONCEPTO CENTRAL   ║             ├──────────────────────┤
├──────────────────┤  ║    (DOBLE RECT)      ║────────────►│  P3.2 EXCLUSIÓN 2    │
│ P2.2 ISOORDINADA │◄─╢                      ║      ≠      └──────────────────────┘
└──────────────────┘  ╚══════════╤═══════════╝             (Con glifo '≠' en #dc2626)
(Izquierda: X=40, W=210)         │
                     ( [Criterio de Clasificación] )       (Cápsula ovalada: Y=310, H=36, rx=18)
                                 │
             ┌───────────────────┴───────────────────┐
             ▼                                       ▼
  ┌──────────────────────┐               ┌──────────────────────┐
  │  P4.1 INFRAORDINADA  │               │  P4.2 INFRAORDINADA  │ (Abajo: Y=410, W=210, H=50)
  └──────────────────────┘               └──────────────────────┘
```

---

## 2. Coordenadas y Estilos por Componente

### 1. Concepto Central (Doble Rectángulo Canónico)
* **Posición**: $X=325, Y=190, W=200, H=60, rx=8$.
* **Doble contorno concéntrico**:
  * Rectángulo exterior: `width="200" height="60" rx="8" fill="#f8fafc" stroke="#0f172a" stroke-width="2"`
  * Rectángulo interior: `x="329" y="194" width="192" height="52" rx="6" fill="#f8fafc" stroke="#0f172a" stroke-width="1.5"`
* **Texto**: `x="425" y="226" font-size="16" font-weight="900" fill="#0f172a" text-anchor="middle" letter-spacing="1"`

### 2. Supraordinada (P1 - Arriba)
* **Posición**: $X=325, Y=40, W=200, H=50, rx=8$.
* **Estilo**: `fill="#e0f2fe" stroke="#0284c7" stroke-width="2"`.
* **Conector**: Línea vertical ascendente de $(425, 190)$ a $(425, 95)$ con `marker-end="url(#arrow-up)" stroke="#0284c7" stroke-width="2"`.

### 3. Isoordinadas (P2 - Izquierda)
* **Posición**: $X=40, W=210, H=50, rx=8$.
  * **Si es 1 isoordinada**: $Y=195$ (centrada frente al concepto).
  * **Si son 2 isoordinadas**: Caja 1 en $Y=160$, Caja 2 en $Y=230$.
  * **Si son 3 isoordinadas**: Caja 1 en $Y=130$, Caja 2 en $Y=195$, Caja 3 en $Y=260$.
* **Estilo**: `fill="#dcfce7" stroke="#16a34a" stroke-width="2"`.
* **Conectores**: Líneas ortogonales que nacen en $X=325, Y=220$ y se dirigen hacia el borde derecho de cada caja ($X=250$) con trazo verde `#16a34a`.

### 4. Exclusiones (P3 - Derecha)
* **Posición**: $X=600, W=210, H=50, rx=8$.
  * **Si son 2 exclusiones**: Caja 1 en $Y=160$, Caja 2 en $Y=230$.
  * **Si son 3 exclusiones**: Caja 1 en $Y=130$, Caja 2 en $Y=195$, Caja 3 en $Y=260$.
* **Estilo**: `fill="#fee2e2" stroke="#dc2626" stroke-width="2"`.
* **Conectores y Glifo**: Líneas ortogonales rojas `#dc2626` con el símbolo **`≠`** destacado sobre cada línea:
  * Para 2 exclusiones: `<text x="575" y="180" font-size="20" font-weight="bold" fill="#dc2626">≠</text>` y en `y="250"`.
  * Para 3 exclusiones: glifos centrados frente a cada una de las 3 alturas.

### 5. Criterio Clasificador (Cápsula Ovalada Intermedia)
* **Posición**: $X=310, Y=310, W=230, H=36, rx=18$.
* **Estilo**: `fill="#f3e8ff" stroke="#9333ea" stroke-width="2"`.
* **Texto**: `x="425" y="333" font-size="12" font-weight="bold" fill="#7e22ce" text-anchor="middle"`.

### 6. Infraordinadas (P4 - Abajo)
* **Posición**: $Y=410, W=210, H=50, rx=8$.
  * Si son 2: $X=180$ y $X=460$.
  * Si son 3: $X=60$, $X=320$ y $X=580$.
* **Estilo**: `fill="#fef3c7" stroke="#d97706" stroke-width="2"`.
* **Conectores**: Líneas descendentes ramificadas con `marker-end="url(#arrow-down)" stroke="#d97706" stroke-width="2"`.

---

## 3. Reglas de Texto y Escape XML

1. **Principio de Integridad Taxonómica**: Jamás mutilar un adjetivo diferenciador esencial para ahorrar espacio.
2. **Límite de 28 Caracteres por Línea**:
   * Si la frase cabe en 28 caracteres: va centrada con `<text x="..." y="...">Frase</text>`.
   * Si la frase supera los 28 caracteres: es **obligatorio usar `<tspan>` multilínea**:
     ```xml
     <text x="145" y="185" font-size="12" fill="#0f172a" text-anchor="middle">
       <tspan x="145" dy="-6">Línea 1 del texto largo</tspan>
       <tspan x="145" dy="14">Línea 2 complementaria</tspan>
     </text>
     ```
3. **Escape XML Estricto**:
   * Reemplazar `&` por `&amp;`
   * Reemplazar `<` por `&lt;`
   * Reemplazar `>` por `&gt;`

---

## 4. Plantilla de Marcadores SVG (`<defs>`)

```xml
<defs>
  <marker id="arrow-up" viewBox="0 0 10 10" refX="5" refY="5" markerWidth="6" markerHeight="6" orient="auto">
    <path d="M 0 10 L 5 0 L 10 10 z" fill="#0284c7"/>
  </marker>
  <marker id="arrow-down" viewBox="0 0 10 10" refX="5" refY="5" markerWidth="6" markerHeight="6" orient="auto">
    <path d="M 0 0 L 10 0 L 5 10 z" fill="#d97706"/>
  </marker>
</defs>
```
