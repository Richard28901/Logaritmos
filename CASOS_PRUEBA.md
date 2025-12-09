# 🧪 Casos de Prueba - Calculadora de Logaritmos

Use estos casos para probar la calculadora y verificar que funciona correctamente.

## Prueba 1: Número Decimal Pequeño

**Input**: `0.001349`

**Salida Esperada**:
```
Paso 1: El número es menor que 1
        Después del punto hay 2 cero(s) antes de la primera cifra significativa
        Fórmula: -(Ceros + 1) = -(2 + 1) = -3
        Notación de tabla: Se escribe como ⁻3

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 1349
        La mantisa (siempre positiva) es: .1300
        Matemáticamente: log(0.001349) - (-3) = -2.870054 - (-3) = 0.129946

Resultado Final:
Notación Académica: ⁻3.1300
Equivalente decimal: -2.8700
```

---

## Prueba 2: Número Mayor que 100

**Input**: `134.9`

**Salida Esperada**:
```
Paso 1: El número es mayor o igual a 1
        La parte entera tiene 3 dígito(s): 134
        Fórmula: Dígitos - 1 = 3 - 1 = 2

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 1349
        La mantisa (siempre positiva) es: .1301
        Matemáticamente: log(134.9) - 2 = 2.130254 - 2 = 0.130254

Resultado Final:
Notación Académica: 2.1301
Equivalente decimal: 2.1301
```

---

## Prueba 3: Número Exacto (Potencia de 10)

**Input**: `1000`

**Salida Esperada**:
```
Paso 1: El número es mayor o igual a 1
        La parte entera tiene 4 dígito(s): 1000
        Fórmula: Dígitos - 1 = 4 - 1 = 3

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 1000
        La mantisa (siempre positiva) es: .0000
        Matemáticamente: log(1000) - 3 = 3.000000 - 3 = 0.000000

Resultado Final:
Notación Académica: 3.0000
Equivalente decimal: 3.0000
```

---

## Prueba 4: Número Entre 0 y 1

**Input**: `0.5`

**Salida Esperada**:
```
Paso 1: El número es menor que 1
        Después del punto hay 0 cero(s) antes de la primera cifra significativa
        Fórmula: -(Ceros + 1) = -(0 + 1) = -1
        Notación de tabla: Se escribe como ⁻1

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 5000
        La mantisa (siempre positiva) es: .6990
        Matemáticamente: log(0.5) - (-1) = -0.301030 - (-1) = 0.698970

Resultado Final:
Notación Académica: ⁻1.6990
Equivalente decimal: -0.3010
```

---

## Prueba 5: Número Muy Pequeño

**Input**: `0.000001`

**Salida Esperada**:
```
Paso 1: El número es menor que 1
        Después del punto hay 5 cero(s) antes de la primera cifra significativa
        Fórmula: -(Ceros + 1) = -(5 + 1) = -6
        Notación de tabla: Se escribe como ⁻6

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 1000
        La mantisa (siempre positiva) es: .0000
        Matemáticamente: log(0.000001) - (-6) = -6.000000 - (-6) = 0.000000

Resultado Final:
Notación Académica: ⁻6.0000
Equivalente decimal: -6.0000
```

---

## Prueba 6: Número Simple (Un Dígito)

**Input**: `5`

**Salida Esperada**:
```
Paso 1: El número es mayor o igual a 1
        La parte entera tiene 1 dígito(s): 5
        Fórmula: Dígitos - 1 = 1 - 1 = 0

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 5000
        La mantisa (siempre positiva) es: .6990
        Matemáticamente: log(5) - 0 = 0.698970 - 0 = 0.698970

Resultado Final:
Notación Académica: 0.6990
Equivalente decimal: 0.6990
```

---

## Prueba 7: Número Grande

**Input**: `123456`

**Salida Esperada**:
```
Paso 1: El número es mayor o igual a 1
        La parte entera tiene 6 dígito(s): 123456
        Fórmula: Dígitos - 1 = 6 - 1 = 5

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 1235
        La mantisa (siempre positiva) es: .0915
        Matemáticamente: log(123456) - 5 = 5.091515 - 5 = 0.091515

Resultado Final:
Notación Académica: 5.0915
Equivalente decimal: 5.0915
```

---

## Prueba 8: Número Decimal (Entre 1 y 10)

**Input**: `2.5`

**Salida Esperada**:
```
Paso 1: El número es mayor o igual a 1
        La parte entera tiene 1 dígito(s): 2
        Fórmula: Dígitos - 1 = 1 - 1 = 0

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 2500
        La mantisa (siempre positiva) es: .3979
        Matemáticamente: log(2.5) - 0 = 0.397940 - 0 = 0.397940

Resultado Final:
Notación Académica: 0.3979
Equivalente decimal: 0.3979
```

---

## Prueba 9: Número Muy Cercano a Cero

**Input**: `0.00001`

**Salida Esperada**:
```
Paso 1: El número es menor que 1
        Después del punto hay 4 cero(s) antes de la primera cifra significativa
        Fórmula: -(Ceros + 1) = -(4 + 1) = -5
        Notación de tabla: Se escribe como ⁻5

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 1000
        La mantisa (siempre positiva) es: .0000
        Matemáticamente: log(0.00001) - (-5) = -5.000000 - (-5) = 0.000000

Resultado Final:
Notación Académica: ⁻5.0000
Equivalente decimal: -5.0000
```

---

## Prueba 10: Número Decimal Aleatorio

**Input**: `0.00789`

**Salida Esperada**:
```
Paso 1: El número es menor que 1
        Después del punto hay 2 cero(s) antes de la primera cifra significativa
        Fórmula: -(Ceros + 1) = -(2 + 1) = -3
        Notación de tabla: Se escribe como ⁻3

Paso 2: Para encontrar la mantisa, buscamos los dígitos significativos: 7890
        La mantisa (siempre positiva) es: .8969
        Matemáticamente: log(0.00789) - (-3) = -2.103119 - (-3) = 0.896881

Resultado Final:
Notación Académica: ⁻3.8969
Equivalente decimal: -2.1031
```

---

## Casos de Error (Deben mostrar alerta)

Estos casos DEBEN rechazarse con un mensaje de alerta:

| Input | Razón | Mensaje |
|-------|-------|---------|
| `-5` | Número negativo | "Por favor ingresa un número positivo mayor que 0" |
| `0` | Cero (logaritmo indefinido) | "Por favor ingresa un número positivo mayor que 0" |
| `` (vacío) | Sin entrada | "Por favor ingresa un número positivo mayor que 0" |
| `abc` | No es un número | "Por favor ingresa un número positivo mayor que 0" |

---

## Checklist de Validación

Después de hacer cada prueba, verifica:

- [ ] La **característica** es correcta (revisa la fórmula explicada)
- [ ] La **mantisa** está entre 0 y 1
- [ ] La **notación de tabla** tiene barra (⁻) solo si característica < 0
- [ ] La **notación decimal** es negativa si característica < 0
- [ ] `característica + mantisa ≈ valor decimal` (con pequeño margen de redondeo)
- [ ] El proceso paso a paso está clara explicado
- [ ] No hay errores en la consola del navegador (F12 → Console)

---

## Ejemplos de Números para Practicar

Estos son números que puedes probar para familiarizarte:

```
Muy pequeños: 0.000001, 0.00001, 0.0001, 0.001
Pequeños: 0.01, 0.1, 0.5, 0.9
Alrededor de 1: 1, 2, 5, 9.9, 10
Medianos: 50, 99, 100, 500, 999
Grandes: 1000, 5000, 10000, 100000, 1000000
Exactos: 10, 100, 1000, 0.1, 0.01, 0.001
```

---

## Notas Importantes

1. **Los decimales pueden variar ligeramente** por redondeo
   - Esperamos 4 decimales de precisión
   - Pequeñas diferencias en el 4to decimal son normales

2. **La explicación es lo más importante**
   - Verifica que entiendes POR QUÉ cada característica es ese número
   - No solo si el número es correcto

3. **Prueba en tu navegador favorito**
   - La calculadora debe funcionar en Chrome, Firefox, Safari, Edge
   - Funciona offline (no necesita internet)

4. **Documenta cualquier problema**
   - Si encuentras un error, nota el input exacto y el comportamiento

---

**Estado**: ✅ Todos los casos de prueba están listos
**Última actualización**: Diciembre 2024
