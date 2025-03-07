# Análisis de Errores en Código

## Descripción
A continuación, detallo los errores encontrados en mis códigos según la teoría de IDSW2.

| Asignatura       | Enlace |
|------------------|--------|
| **Programación 1** | [Reto Caracol](https://github.com/aadrigaar/prg1-22-23/blob/main/retos/entregas/adrianGarcia/Reto%20Caracol/Reto%20Caracol%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java) |
| **Programación 1** | [Whac-A-Mole](https://github.com/aadrigaar/prg1-22-23/blob/main/retos/entregas/adrianGarcia/Reto%20WhacAMole/Reto%20WhacAMole%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java) |
| **Programación 1** | [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/main/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java) |

---
## Legibilidad

### Nombrado

**Nombres desinformativos** (Uso de variables con nombres poco descriptivos)
- `profundidadCaracolm` y `profundidadCaracoln` podrían llamarse `profundidadCaracolSube` y `profundidadCaracolBaja` para mayor claridad. [Reto Caracol](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20Caracol/Reto%20Caracol%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L37)
- `monigote` y `monigote1` podrían tener nombres más descriptivos como `posicionMole1` y `posicionMole2`. [Whac-A-Mole](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20WhacAMole/Reto%20WhacAMole%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L9)
- `Atendidas` debería llamarse `clientesAtendidos` para mejorar la comprensión. [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L15)

**Evitar nombres en serie**
- Uso de variables como `caja1`, `caja2`, `caja3`, `caja4`. En su lugar, se podría utilizar un array `cajas[i]`. [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L6)

---
## Comentarios

**Ausencia de comentarios explicativos**
- No hay comentarios que expliquen la lógica del caracol subiendo y bajando. [Reto Caracol](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20Caracol/Reto%20Caracol%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L34)
- La generación de números aleatorios para la posición del objetivo en Whac-A-Mole no está documentada. [Whac-A-Mole](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20WhacAMole/Reto%20WhacAMole%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L16)
- No se explica cómo funciona la simulación de la fila en el supermercado. [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L30)

---
## Formato y Consistencia

**Uso de valores mágicos**
- `profundidadTotal = 20`, `profundidadDelAgua = 7`. Se recomienda definir constantes con nombres más representativos. [Reto Caracol](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20Caracol/Reto%20Caracol%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L6)
- `dimension = 4` en Whac-A-Mole debería estar definido como una constante. [Whac-A-Mole](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20WhacAMole/Reto%20WhacAMole%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L5)
- `horarioTrabajo = 12 * 60` podría reemplazarse por `MINUTOS_POR_DIA = 720`. [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L10)

**Mensajes de salida confusos**
- `System.out.println("Por la mañana el caracol " + profundidadCaracolm + " metros y por la noche bajo " + profundidadCaracoln + " metros");`
  - Falta claridad en la estructura del mensaje. [Reto Caracol](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20Caracol/Reto%20Caracol%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L40)

---
## Código Muerto

**Variables sin utilidad**
- `profundidadFinal` no es realmente necesaria, ya que `profundidadCaracol` puede actualizarse directamente. [Reto Caracol](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20Caracol/Reto%20Caracol%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L39)
- `casilla` se define fuera del bucle, pero se usa dentro solo una vez. [Whac-A-Mole](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20WhacAMole/Reto%20WhacAMole%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L8)

**Eliminar línea innecesaria**
- `System.out.println("")` dentro de un `if` vacío. [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L28)

---
## Principios DRY y YAGNI

**Código repetitivo**
- Se repite la impresión de la estructura del pozo en cada iteración del bucle. Se recomienda encapsular en una función. [Reto Caracol](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20Caracol/Reto%20Caracol%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L47)
- Se repite la lógica para generar posiciones aleatorias del objetivo. [Whac-A-Mole](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/Reto%20WhacAMole/Reto%20WhacAMole%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L16)
- Se repiten estructuras `if` para cada caja en lugar de usar un bucle. [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L32)
 
**Variables innecesarias (YAGNI)**
- `itemEnCaja2`, `itemCaja3`, `itemsCaja4` se pueden reemplazar por un array `itemsPorCaja[i]`. [Reto CCCF](https://github.com/aadrigaar/prg1-22-23/blob/c3471e21734d91e9ad15c876dde8bee8a0891220/retos/entregas/adrianGarcia/RetoCCCF/RetoCCCF%20-%20Adri%C3%A1n%20Garc%C3%ADa%20Arranz.java#L11)
