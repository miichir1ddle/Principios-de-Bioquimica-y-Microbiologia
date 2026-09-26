# Seminario 4: Factores que afectan la velocidad de las reacciones enzimáticas

*Principios de Bioquímica y Microbiología, Ingeniería Química, 2do año. Base: Conferencia 2 (Enzimas) y el material "Factores que influyen sobre la actividad enzimática". Bibliografía: Lehninger cap. 8, Voet y Voet caps. 12 y 13, Cardellá Tomo I caps. 15 y 16.*

> Nota: los gráficos están hechos en ASCII. Para entregar quizás prefieras redibujarlos a mano o en Excel.

---

## 1. Influencia de la concentración de sustrato [S]

Con la concentración de enzima, el pH y la temperatura **constantes**, al variar [S] la velocidad inicial (V₀) describe una **curva hiperbólica** (saturación):

```
 V0
 Vmax ┤ - - - - - - - - - - - - ______________
      │                     ___---
      │                 _--
 Vmax/2 ┤ - - - - - -_-  
      │           _/ ¦
      │         _/   ¦
      │       _/     ¦
      │     _/       ¦
      │   _/         ¦
      └──/───────────¦──────────────────── [S]
                    Km
```

Se distinguen tres zonas:

1. **[S] baja:** V₀ es **proporcional a [S]**. Reacción de **primer orden** respecto al sustrato (n = 1). Hay muchos centros activos libres y cada molécula de sustrato adicional encuentra una enzima.
2. **[S] intermedia:** V₀ crece cada vez menos y deja de ser proporcional. Es un **orden mixto**.
3. **[S] alta (saturante):** V₀ **se hace independiente de [S]** y tiende asintóticamente a **Vmáx**. Reacción de **orden cero** (n = 0). Todos los centros activos están ocupados y la enzima está **saturada** por el sustrato. Aumentar [S] ya no acelera la reacción.

El fenómeno de saturación es una característica de las reacciones enzimáticas. Todas las enzimas lo muestran, pero varían en la [S] necesaria para alcanzarlo.

**Ecuación de Michaelis-Menten** (mecanismo E + S ⇄ ES → E + P, un solo sustrato):

```
          Vmáx · [S]
V₀ = ─────────────────
         Km + [S]
```

**Nota sobre la conferencia:** el texto dice que a altas [S] "la velocidad comienza a disminuir". Eso solo ocurre con inhibición por exceso de sustrato. En una cinética de Michaelis-Menten ideal, la curva se aproxima a Vmáx y se mantiene.

---

## 2. Significado de Km y Vmáx

### Vmáx (velocidad máxima)

- Es la velocidad que se alcanza a **concentración saturante de sustrato**, cuando **toda la enzima está en forma de complejo ES**.
- Vmáx = k₃ · [E]t, donde k₃ es la constante catalítica (número de recambio) y [E]t la concentración total de enzima. **Depende de la cantidad de enzima**.
- Varía de una enzima a otra y se ve afectada por la **estructura del sustrato, el pH y la temperatura**.

### Km (constante de Michaelis)

- Es la **concentración de sustrato a la cual la velocidad es la mitad de Vmáx** (V₀ = Vmáx/2). Se demuestra con la ecuación: si V₀ = Vmáx/2, entonces Km + [S] = 2[S], y por tanto **Km = [S]**.
- Se expresa en **mol/L**. Es una **constante característica de cada enzima para cada sustrato**.
- **Mide la afinidad de la enzima por el sustrato** (de forma aproximada, 1/Km). Un **Km bajo** indica **alta afinidad**, porque con poco sustrato se alcanza la mitad de Vmáx. Un **Km alto** indica **baja afinidad**.
- Si varias enzimas compiten por el mismo sustrato, este será transformado preferentemente por la de **menor Km**.
- No es un valor fijo. Puede variar con **temperatura, pH y estructura del sustrato**. Si la enzima tiene varios sustratos, cada uno tiene su Km.
- **Km es independiente de la concentración de enzima.**

**Representación de Lineweaver-Burk** (dobles inversos):

```
 1     Km   1      1
──── = ──── · ─── + ────
 V₀   Vmáx  [S]   Vmáx
```

```
  1/V0 │            /
       │          /      pendiente = Km/Vmáx
       │        /
 1/Vmáx┤-----/
       │   /
 ──────┼──/──────────────── 1/[S]
 -1/Km │/
```

Es una recta que corta el eje **Y en 1/Vmáx**, el eje **X en –1/Km**, y tiene **pendiente Km/Vmáx**.

---

## 3. Influencia de la concentración de enzima [E]

Con [S] **saturante** (en exceso), y con pH y temperatura constantes, la velocidad es **directamente proporcional a la concentración de enzima**: V = k₃ · [E]t.

```
 V0
   │                          /
   │                        /
   │                      /
   │                    /
   │                  /
   │                /
   │              /
   │            /
   │          /
   │        /
   └───/───────────────────────────── [E]
```

- Al duplicar [E], se **duplica la velocidad**, y la **pendiente** de la recta equivale a k₃ (número de recambio).
- Solo se cumple si [S] es **suficientemente elevada** para saturar toda la enzima presente. Si [S] fuera limitante, la respuesta sería menos que proporcional.
- **Aplicación práctica:** la proporcionalidad permite **cuantificar la actividad enzimática** en tejidos y muestras clínicas.
- Con [S] fija, aumentar [E] hace subir **Vmáx**, pero **Km no cambia**.

---

## 4. Influencia de la temperatura y del pH

### Temperatura

```
 Actividad
 (V0)
   │                   ***
   │                *       *
   │              *           *
   │            *               *
   │          *                    *
   │        *                         *
   │      *                              *
   │    *                                   *
   └────────────────────┬──────────────────────── T (°C)
                   T óptima (~37 °C)
```

- **Al subir la temperatura**, aumenta la energía cinética de las moléculas y las colisiones, por lo que la velocidad **crece** (en general se duplica cada 10 °C, dentro del intervalo en que la enzima es estable).
- Se alcanza una **temperatura óptima**. En muchas enzimas de mamíferos es de ~**37 °C**.
- Por encima de ~**45 °C** comienza la **desnaturalización térmica**. Como las enzimas son proteínas, pierden su conformación nativa y **se inactivan**. La mayoría se inactivan entre **55 y 60 °C**.
- Resultado: una **curva acampanada asimétrica**, con ascenso gradual y caída brusca.
- **Excepciones:** bacterias y algas de aguas termales tienen óptimos altos, y ciertas bacterias árticas, cercanos a 0 °C.

### pH

```
 Actividad
 (V0)
   │                 ***
   │              *       *
   │            *           *
   │          *               *
   │        *                   *
   │      *                       *
   │    *                            *
   └───────────────┬──────────────────────── pH
              pH óptimo
```

- Cada enzima tiene un **pH óptimo** donde su actividad es máxima. Por encima o por debajo la actividad **disminuye**, con una **curva acampanada**.
- **Causa:** el pH modifica el estado de ionización de los **grupos ácido-base de la enzima** (los del centro activo, catalíticos o de unión al sustrato) y del **sustrato**. También altera las interacciones que mantienen la estructura terciaria. Un pH muy alto o muy bajo produce **desnaturalización** e inactivación.
- Ejemplos de pH óptimo: **pepsina 1,5**, fosfatasa ácida 5,0, catalasa 7,6, tripsina 7,7, fumarasa y ribonucleasa 7,8, **fosfatasa alcalina 9,0**, arginasa 9,7. Muchas enzimas tienen su máximo cerca de la neutralidad (6 a 8).
- El pH óptimo **no siempre coincide** con el pH intracelular normal.

---

## 5. Inhibición reversible frente a irreversible

| Característica | **Reversible** | **Irreversible** |
|---|---|---|
| **Unión inhibidor-enzima** | **No covalente** (puentes de hidrógeno, iónicas, hidrofóbicas), débil | **Covalente**, o muy estable |
| **Efecto en la enzima** | No la modifica de forma permanente | **Modifica de modo permanente** un grupo funcional necesario para la catálisis |
| **Recuperación de la actividad** | **Sí**, al eliminar el inhibidor (diálisis, dilución) o aumentar [S] en la competitiva | **No**, la enzima queda inactiva. Se recupera solo con síntesis de enzima nueva |
| **Velocidad de acción** | **Rápida**, alcanza el equilibrio E + I ⇄ EI | **Lenta**, la inhibición aumenta gradualmente con el tiempo |
| **Aplicación de Michaelis-Menten** | **Se aplica** (equilibrio rápido y reversible). Tiene una **Kᵢ** | **No se aplica**, porque no supone complejos reversibles |
| **Tipos** | Competitiva, no competitiva, acompetitiva | No se clasifica así |
| **Ejemplos** | Malonato sobre succinato deshidrogenasa; sulfanilamida | **DFP** (gas nervioso, acetilcolinesterasa), metales pesados, iodoacetato, penicilina |

---

## 6. Inhibición competitiva frente a no competitiva

| Aspecto | **Competitiva** | **No competitiva** |
|---|---|---|
| **Sitio de unión del inhibidor** | Al **centro activo** de la enzima **libre** (E). Compite con el sustrato. Suele ser **análogo estructural del sustrato**. Forma E–I | A un **sitio distinto del centro activo**. Se une a la **enzima libre (E) o al complejo ES**, formando EI y ESI (inactivos). **Deforma** la enzima y cambia la conformación del centro activo |
| **Efecto sobre Km** | **Aumenta** el Km aparente (se necesita más sustrato para llegar a Vmáx/2). Disminuye la afinidad aparente | **No cambia** (en la no competitiva pura), porque no altera la unión del sustrato |
| **Efecto sobre Vmáx** | **No cambia**. Con [S] muy alta se **desplaza al inhibidor** y se alcanza la misma Vmáx | **Disminuye**. No se recupera aunque se aumente [S] |
| **Efecto de aumentar [S]** | **Revierte** la inhibición | **No revierte** la inhibición |
| **Gráfica de Lineweaver-Burk** | Rectas con **igual ordenada en el origen (1/Vmáx)**, es decir, **se cruzan en el eje Y**. **Distinta pendiente** (mayor con inhibidor) y **distinto corte en X** (–1/Km más cercano a cero) | Rectas con **igual corte en el eje X (–1/Km)**. **Distinta ordenada en el origen** (1/Vmáx mayor con inhibidor) y **distinta pendiente**. Se cruzan en el eje X |
| **Ejemplo** | **Malonato** sobre succinato deshidrogenasa; **sulfanilamida** (compite con el ácido p-aminobenzoico) | Metales pesados que se unen a grupos –SH fuera del centro activo, ciertos inhibidores alostéricos |

**Gráficas de Lineweaver-Burk**

```
COMPETITIVA (se cruzan en el eje Y)          NO COMPETITIVA (se cruzan en el eje X)

 1/V0 │       /  con I                         1/V0 │          /  con I
      │     /  /                                    │        /
      │   /  /   sin I                              │      /  /
      │ /  /  /                                     │    /  /   sin I
1/Vmax┤/ /  /                                       │  /  /  /
      │ /  /                                        │/  /  /
      │/ /                                    1/Vmax'┤ /  /  (con I, sube)
 ─────┼/──────────── 1/[S]                    1/Vmax ┤/ /
  -1/Km'  -1/Km                                      │/
  (con I) (sin I)                              ──────┼──────────── 1/[S]
                                                   -1/Km (igual)
```

**Resumen:**

| | Km | Vmáx | Corte en Y | Corte en X |
|---|---|---|---|---|
| **Sin inhibidor** | Km | Vmáx | 1/Vmáx | –1/Km |
| **Competitiva** | ↑ | = | **igual** | se acerca a 0 |
| **No competitiva** | = | ↓ | **sube** | **igual** |

Un tercer tipo, la **acompetitiva**, se une solo al complejo ES. Disminuyen **Km y Vmáx** y se obtienen **rectas paralelas** (pendiente constante). Es poco frecuente en reacciones de un solo sustrato.
