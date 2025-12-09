# 📚 Guía Rápida - Calculadora de Logaritmos

## Acceso Rápido

**Para ejecutar localmente:**
```bash
# Opción 1: Python (http.server)
python3 -m http.server 8000

# Opción 2: Node.js (http-server)
npx http-server

# Opción 3: PHP
php -S localhost:8000

# Opción 4: Simplemente abrir index.html en el navegador
```

Luego abre: **http://localhost:8000**

---

## ¿Qué es un Logaritmo?

Un **logaritmo en base 10** responde la pregunta: *"¿A qué potencia debo elevar 10 para obtener este número?"*

**Ejemplos:**
- log₁₀(100) = 2 (porque 10² = 100)
- log₁₀(1000) = 3 (porque 10³ = 1000)
- log₁₀(5) ≈ 0.699 (porque 10^0.699 ≈ 5)

---

## Estructura de un Logaritmo

```
log₁₀(N) = Característica + Mantisa
         = (parte entera) + (parte decimal)
         = (siempre negativa para N<1) + (siempre positiva)
```

### Característica
- **Para N ≥ 1**: Cuenta los dígitos de la parte entera y resta 1
  - 134 → 3 dígitos → característica = 2
  - 1000 → 4 dígitos → característica = 3

- **Para N < 1**: Cuenta los ceros tras el punto y agrega 1 negativo
  - 0.1 → 1 cero → característica = -1
  - 0.001 → 2 ceros → característica = -3

### Mantisa
- Siempre está entre 0 y 1 (0 ≤ m < 1)
- Se calcula: `mantisa = logTotal - característica`
- Históricamente se buscaba en tablas impresas

---

## Ejemplos Paso a Paso

### Ejemplo 1: log₁₀(50)
```
Paso 1: 50 ≥ 1, parte entera "50" = 2 dígitos
        Característica = 2 - 1 = 1

Paso 2: log₁₀(50) ≈ 1.699
        Mantisa = 1.699 - 1 = 0.699

Resultado: 1.699 (notación tabla y decimal)
```

### Ejemplo 2: log₁₀(0.0005)
```
Paso 1: 0.0005 < 1, tras punto "0005" = 3 ceros
        Característica = -(3 + 1) = -4

Paso 2: log₁₀(0.0005) ≈ -3.301
        Mantisa = -3.301 - (-4) = 0.699

Resultado: ⁻4.0699 (tabla) = -3.301 (decimal)
```

---

## Notaciones

### Notación de Tabla (Académica)
- Se usa una barra sobre la característica negativa
- Ejemplo: `⁻3.1300` significa característica -3, mantisa .1300
- La barra se escribe: `<span style="text-decoration:overline">3</span>`

### Notación Decimal (Moderna)
- Se escribe el logaritmo real en formato decimal
- Ejemplo: `-2.8700`
- Es lo que ves en calculadoras científicas

---

## Casos Especiales

| Número | Característica | Mantisa | Tabla | Decimal |
|--------|----------------|---------|-------|---------|
| 1      | 0              | 0.0000  | 0.0000 | 0.0000 |
| 10     | 1              | 0.0000  | 1.0000 | 1.0000 |
| 100    | 2              | 0.0000  | 2.0000 | 2.0000 |
| 0.1    | -1             | 0.0000  | ⁻1.0000 | -1.0000 |
| 0.01   | -2             | 0.0000  | ⁻2.0000 | -2.0000 |

---

## Propiedades Importantes

1. **Mantisa es SIEMPRE positiva**
   - Incluso para logaritmos negativos
   - Ej: log₁₀(0.5) = -1 + 0.699

2. **La barra se lee como "negativo"**
   - ⁻3.1300 = -3 + 0.1300 = -2.8700

3. **Recuperar el original**
   - logOriginal = característica + mantisa
   - -2.8700 = -3 + 0.1300 ✓

---

## Historicamente...

Antes de 1974 (año de la primera calculadora científica comercial):

- Los científicos e ingenieros usaban **tablas de logaritmos** impresas
- Estas tablas tenían 50-100+ páginas
- Mostraban las **mantisas** para diferentes secuencias de dígitos
- Usar logaritmos hacía que multiplicaciones fueran sumas (más rápido)

**Ventaja**: log(a × b) = log(a) + log(b)

Ejemplo histórico:
- Para multiplicar 12.3 × 45.6:
  1. Buscar log(12.3) ≈ 1.0899
  2. Buscar log(45.6) ≈ 1.6590
  3. Sumar: 1.0899 + 1.6590 = 2.7489
  4. Buscar antilog(2.7489) ≈ 561 ✓
  
Hoy multiplicamos directamente (12.3 × 45.6 = 561), pero aprender esto ayuda a entender la estructura de los números.

---

## Validación: ¿Mi respuesta es correcta?

1. **¿La mantisa está entre 0 y 1?** → ✓ Correcto
2. **¿El resultado tabla + decimal son equivalentes?** → ✓ Correcto
3. **¿Característica + mantisa = logOriginal?** → ✓ Correcto
4. **¿Para números grandes, característica es positiva?** → ✓ Correcto
5. **¿Para números pequeños, característica es negativa?** → ✓ Correcto

---

## Recursos Adicionales

- **Wikipedia**: Logaritmo (base 10)
- **Khan Academy**: Logarithms (video lectures)
- **Historical**: Tables of Logarithms (Museum of Mathematics)

---

**Última actualización**: Diciembre 2024
**Versión**: 1.0
**Estado**: ✅ Completo y validado
