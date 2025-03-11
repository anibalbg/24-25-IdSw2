## Archivos
1. **[NumAlea.java](./src/NumAlea.java)**
2. **[Retocaracol.java](./Retocaracol.java)**
3. **[RetoDevolverCambio.java](./RetoDevolverCambio.java)**
## Errores  
### 1. Elige nombres descriptivos
 Fallo: En el archivo Retocaracol.java, el nombre coche no es descriptivo. No queda claro qué representa exactamente.

 Ejemplo: int coche = (int) (Math.random() * 10) + 1;

Sugerencia: Un nombre más descriptivo sería probabilidadDeCoche o eventoCoche.

### 2. Elige nombres al nivel de abstracción apropiado
Fallo: En el archivo NumAlea.java, el nombre WhacAMole no es apropiado para el nivel de abstracción del problema. El código no tiene relación con el juego "Whac-a-Mole".

Ejemplo: public class WhacAMole { ... }

Sugerencia: Un nombre más apropiado sería JuegoAdivinanza o AdivinaElNumero.

### 3. Usa nomenclatura estándar donde sea posible
Fallo: En el archivo RetoDevolverCambio.java, la variable CantidadDeBilletes no sigue la convención de nomenclatura estándar de Java (camelCase).

Ejemplo: double CantidadDeBilletes;

Sugerencia: El nombre debería ser cantidadDeBilletes.

### 4. Nombres no ambiguos
Fallo: En el archivo Retocaracol.java, el nombre sube y baja son ambiguos. No queda claro si se refieren a la acción del caracol o a otra cosa.

Ejemplo: int sube = (int) (Math.random() * 4) + 1;

Sugerencia: Nombres más claros serían metrosSubidos y metrosBajados.

### 5. Usa nombres largos para ámbitos largos
Fallo: En el archivo RetoDevolverCambio.java, la variable resto es demasiado corta para un ámbito largo donde se usa repetidamente.

Ejemplo: double resto;

Sugerencia: Un nombre más descriptivo sería restoDevolucion.

### 6. Evita codificaciones
Fallo: En el archivo Retocaracol.java, el número 3.5 está codificado directamente en el código, lo que dificulta su comprensión.

Ejemplo: if(coche <= 3.5) { ... }

Sugerencia: Debería ser una constante con un nombre descriptivo, como PROBABILIDAD_COCHE.

### 7. Los nombres deberían describir los efectos laterales
Fallo: En el archivo NumAlea.java, el método daleUnaPista no describe claramente que también imprime un mensaje en la consola.

Ejemplo: static void daleUnaPista(int numeroDelUsuario, int numeroDeLaMaquina) { ... }

Sugerencia: Un nombre más descriptivo sería imprimirPistaSegunDistancia.

### 8. Los nombres deben revelar su intención
Fallo: En el archivo RetoDevolverCambio.java, el nombre preguntaEntero no revela claramente que se trata de una función que obtiene un número del usuario.

Ejemplo: static int preguntaEntero(String pregunta) { ... }

Sugerencia: Un nombre más claro sería obtenerNumeroDelUsuario.

### 9. La elección de buenos nombres lleva tiempo, pero ahorra más de lo que toma
Fallo: En el archivo Retocaracol.java, el nombre profundidadCaracol es descriptivo, pero podría ser más claro si se refina.

Ejemplo: int profundidadCaracol = (int) (Math.random() * 10) + 10;

Sugerencia: Un nombre más preciso sería profundidadActualCaracol.

### 10. Nombres pronunciables que permitan mantener una conversación
Fallo: En el archivo RetoDevolverCambio.java, el nombre moneda005 no es fácil de pronunciar.

Ejemplo: double moneda005 = 0.05;

Sugerencia: Un nombre más pronunciable sería monedaCincoCentimos.

### 11. Mayúsculas en los caracteres inicio de palabra (CamelCase)
Fallo: En el archivo RetoDevolverCambio.java, la variable CantidadDeBilletes no sigue la convención CamelCase.

Ejemplo: double CantidadDeBilletes;

Sugerencia: Debería ser cantidadDeBilletes.

### 12. Nombres del dominio del problema y de la solución
Fallo: En el archivo Retocaracol.java, el nombre BORDE_SUPERIOR_COCHE no está relacionado con el dominio del problema (un caracol en un pozo).

Ejemplo: final String BORDE_SUPERIOR_COCHE = "[][] O-=-O [][]";

Sugerencia: Un nombre más relacionado con el dominio sería BORDE_SUPERIOR_EVENTO.

### 13. Elige una palabra para un concepto abstracto y aferrarte a él
Fallo: En el archivo RetoDevolverCambio.java, se usan tanto billete como moneda para referirse a conceptos similares (dinero).

Ejemplo: int billete500 = 500; y double moneda005 = 0.05;

Sugerencia: Se podría usar denominacion para ambos casos.

### 14. Nombres de paquetes deben ser sustantivos y comenzar en minúsculas
Fallo: No hay paquetes definidos en los archivos, pero si los hubiera, deberían seguir esta convención.

Ejemplo: (No aplicable en este caso).

Sugerencia: Si se creara un paquete, debería ser algo como juego o utilidades.

### 15. Nombres de clases deben ser sustantivos y comenzar en mayúsculas
Fallo: En el archivo Retocaracol.java, el nombre de la clase Retocaracol no es un sustantivo claro.

Ejemplo: public class Retocaracol { ... }

Sugerencia: Un nombre más apropiado sería SimulacionCaracol.

### 16. Nombres de métodos deben ser verbos o una frase con verbo y comenzar en minúsculas
Fallo: En el archivo NumAlea.java, el método imprimeTablero no sigue la convención de comenzar con minúscula.

Ejemplo: static void imprimeTablero(int golpe) { ... }

Sugerencia: Debería ser imprimirTablero.

### 17. Nombres de métodos de acceso deben anteponer get(is para lógicos) y /set o put
Fallo: En el archivo NumAlea.java, el método preguntaEntero no sigue la convención de métodos de acceso.

Ejemplo: static int preguntaEntero(String pregunta) { ... }

Sugerencia: Debería ser getEnteroDelUsuario.

### 18. Si un nombre requiere un comentario, el nombre no revela su intención
Fallo: En el archivo NumAlea.java, el comentario // esto es para hacer un numero aleatorio y decir si esta cerca o lejos y el tablero sugiere que el nombre de la clase no es descriptivo.

Ejemplo: public class NumAlea { ... }

Sugerencia: Un nombre más descriptivo sería JuegoAdivinanzaNumeros.

### 19. Nombres de una letra y muy en particular, 'O' y 'l' que se confunden con 0 y 1
Fallo: En el archivo Retocaracol.java, el nombre i en el bucle for es aceptable, pero podría ser más descriptivo.

Ejemplo: for (int i = 1; i <= profundidadTotal; i = i + 1) { ... }

Sugerencia: Un nombre más descriptivo sería profundidadActual.
