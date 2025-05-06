# Proyecto de Investigación AG: *Fractales*

Este proyecto forma parte de una investigación académica orientada al estudio, análisis y generación de **fractales**, con énfasis en su aplicación matemática, visual y computacional. Fue desarrollado en el marco de la carrera de Ingeniería en Sistemas de Información.

## 🧠 Objetivos

- Comprender los fundamentos matemáticos de los fractales.
- Explorar su presencia en la naturaleza y en fenómenos computacionales.
- Implementar algoritmos que generen fractales conocidos (por ejemplo: Conjunto de Mandelbrot, Conjunto de Julia, Árboles recursivos).
- Evaluar la complejidad computacional y los patrones emergentes.

## 📁 Contenidos del repositorio

## 🛠️ Tecnologías y herramientas utilizadas

- Lenguaje de programación: Python / C / [tu lenguaje aquí]
- Librerías: matplotlib, numpy, PIL (según el caso)
- Herramientas de documentación: LaTeX, Markdown
- Visualización: scripts interactivos o renderizado en 2D/3D

## 📈 Metodología

1. **Investigación teórica** sobre la historia y fundamentos de los fractales.
2. **Diseño e implementación** de generadores recursivos e iterativos.
3. **Experimentación** con distintos parámetros para observar comportamientos emergentes.
4. **Análisis de resultados** tanto visual como numéricamente.
5. **Redacción de conclusiones** y discusión de aplicaciones reales.

## 📷 Ejemplos visuales

<p align="center">
  <img src="images/mandelbrot.png" width="300" alt="Mandelbrot">
  <img src="images/julia.png" width="300" alt="Julia">
</p>

## 👥 Autores

- [Nombre y Apellido 1] - UTN - Ingeniería en Sistemas  
- [Nombre y Apellido 2] - UTN - Ingeniería en Sistemas  
- [Tu nombre] *(coordinador / desarrollador principal / etc.)*

## 📄 Licencia

Este proyecto se publica bajo la Licencia MIT (u otra si aplica). Podés usar, modificar y distribuir el contenido citando la fuente original.

---

> “Los fractales no son solo figuras bonitas, son una ventana a la complejidad del universo.”  
> — *Benoît B. Mandelbrot*


## Investigacion Teorica
1. Fractales y Terrenos:
Los fractales, como el algoritmo de Perlin Noise o Diamante-Cuadrado, se utilizan comúnmente para generar terrenos naturales. Estos algoritmos crean patrones de ruido que simulan variaciones realistas en el terreno, como montañas, valles y llanuras. Estos terrenos tienen una apariencia auto-similar a diferentes escalas, lo cual es característico de los fractales.

2. Algoritmos Genéticos:
Los algoritmos genéticos (AG) son técnicas de optimización que se inspiran en la evolución natural. Funcionan con una población de soluciones (en este caso, parámetros para el terreno fractal) que evolucionan a lo largo de varias generaciones, buscando mejorar alguna medida de "aptitud" (fitness), que en este contexto podría ser qué tan realista o deseable es el terreno generado.

3. Proceso de Generación de Terreno con AG y Fractales:
a) Codificación de los Terrenos:
Individuos en la población genética: Cada individuo puede representar un conjunto de parámetros de un algoritmo fractal. Estos parámetros podrían incluir:

Escala y frecuencia del ruido (en el caso de Perlin Noise).

Factores de rugosidad o variabilidad en el terreno.

Otros parámetros como la altura máxima, la distribución de las colinas, la pendiente, etc.

Genes: Cada parámetro es un "gen" en el cromosoma del individuo.

b) Función de Aptitud:
La función de aptitud debe evaluar qué tan bueno es el terreno generado por un conjunto de parámetros. Algunos enfoques para definir la aptitud pueden ser:

Realismo visual: Comparando el terreno generado con imágenes de terrenos reales.

Diversidad de terreno: Un terreno que tenga una variedad adecuada de formas (montañas, llanuras, ríos) puede ser considerado más apto.

Jugabilidad o accesibilidad: Si el terreno se utiliza en un videojuego, la función de aptitud puede considerar si es jugable o interesante para los usuarios.

c) Operadores Genéticos:
Selección: Seleccionar los mejores individuos basados en la función de aptitud (terrenos más realistas o interesantes).

Cruzamiento (Crossover): Combinar los parámetros de dos individuos para crear nuevos individuos, por ejemplo, cruzando las escalas de dos terrenos.

Mutación: Cambiar aleatoriamente uno o varios parámetros en un individuo, permitiendo explorar nuevas configuraciones de terreno.

d) Evolución:
Este proceso se repite por varias generaciones, y con cada ciclo, los terrenos generados tienden a mejorar en base a la función de aptitud.

Con cada nueva generación, los parámetros del terreno se van ajustando, mejorando gradualmente el realismo y las características del paisaje.

4. Implementación Básica:
Para implementar un sistema de generación de terreno con fractales y algoritmos genéticos, podrías seguir estos pasos:

Paso 1: Define los parámetros de entrada del algoritmo fractal (como la frecuencia del ruido, amplitud, etc.).

Paso 2: Codifica estos parámetros en una representación genética (un vector de valores).

Paso 3: Define una función de aptitud que evalúe qué tan bien el terreno generado se ajusta a tus expectativas.

Paso 4: Aplica los operadores genéticos (selección, cruzamiento, mutación) a la población.

Paso 5: Repite el proceso hasta que obtengas un terreno satisfactorio.

5. Ventajas de Este Enfoque:
Permite explorar una amplia gama de configuraciones posibles para el terreno de forma eficiente.

Se pueden generar terrenos altamente adaptados a un criterio específico (realismo, jugabilidad, etc.).

La naturaleza evolutiva del proceso permite adaptarse y refinar gradualmente las características del terreno.

6. Desventajas:
Requiere de una definición clara de la función de aptitud, que podría ser compleja de evaluar, especialmente si se busca realismo visual.

El proceso evolutivo puede ser costoso en términos de tiempo de cómputo, especialmente para grandes poblaciones o terrenos muy complejos.

Este enfoque, si bien es más lento que un algoritmo de generación fractal tradicional, tiene el potencial de generar terrenos mucho más adaptativos y específicos según el criterio de optimización que utilices.
