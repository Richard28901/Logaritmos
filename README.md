# 🧮 Calculadora Educativa de Logaritmos (Base 10)

Una herramienta interactiva que enseña a los estudiantes cómo se estructura un logaritmo usando el **método manual de tablas de logaritmos**, separando el resultado en dos partes: **Característica** y **Mantisa**.

## 🎯 Objetivo Educativo

Este proyecto simula cómo los matemáticos y científicos calculaban logaritmos antes de las calculadoras modernas, utilizando tablas impresas. El logaritmo se descompone en:

- **Característica (Parte Entera)**: Indica el orden de magnitud del número
- **Mantisa (Parte Decimal)**: Se consulta en tablas estándar de logaritmos

## 📋 Reglas Matemáticas Implementadas

### 1. Cálculo de la Característica

#### Para números ≥ 1:
```
Característica = (Número de dígitos de la parte entera) - 1
Ejemplo: 134.9 → 3 dígitos → Característica = 2
```

#### Para números < 1:
```
Característica = -(Ceros después del punto + 1)
Ejemplo: 0.001349 → 2 ceros tras el punto → Característica = -3
Notación de tabla: Se escribe con barra: ⁻3 (sobrerrayado)
```

### 2. Cálculo de la Mantisa

```
Mantisa = log₁₀(N) - Característica
```

- **Siempre es positiva** (0 ≤ mantisa < 1)
- Se muestra con **4 decimales** (simulando tablas estándar)
- Se calcula matemáticamente para precisión perfecta

### 3. Formatos de Visualización

**Notación Académica/Tablas** (cuando característica es negativa):
```
⁻3.1300  →  Característica -3, Mantisa .1300
```

**Notación Decimal Estándar**:
```
-2.8700  →  Valor real del logaritmo
```

## 🚀 Características

✅ **Interfaz educativa y moderna**: Diseño limpio con gradientes y animaciones
✅ **Explicación paso a paso**: Muestra todo el proceso de cálculo
✅ **Validación de entrada**: Rechaza números negativos o cero
✅ **Dos formatos de salida**: Notación de tabla + notación decimal
✅ **Responsive**: Funciona en computadoras, tablets y móviles
✅ **Sin dependencias externas**: HTML, CSS y JavaScript vanilla
✅ **Accesible**: Soporta entrada por teclado (Enter para calcular)

## 💡 Ejemplos de Uso

### Ejemplo 1: Número Mayor que 1
**Entrada**: 134.9
- Parte entera: 134 (3 dígitos)
- Característica: 3 - 1 = **2**
- Mantisa calculada: **0.1301**
- **Resultado**: 2.1301 = -2.1301 (decimal)

### Ejemplo 2: Número Menor que 1
**Entrada**: 0.001349
- Ceros después del punto: 2 (0.00...)
- Característica: -(2 + 1) = **-3**
- Mantisa calculada: **0.1300**
- **Resultado**: ⁻3.1300 = -2.8700 (decimal)

### Ejemplo 3: Un Dígito
**Entrada**: 5
- Parte entera: 5 (1 dígito)
- Característica: 1 - 1 = **0**
- Mantisa calculada: **0.6990**
- **Resultado**: 0.6990 = 0.6990 (decimal)

## 🛠️ Estructura del Código

```
index.html
├── HEAD
│   ├── Meta información
│   ├── Título
│   └── Estilos CSS
│       ├── Diseño responsivo
│       ├── Animaciones
│       ├── Gradientes
│       └── Componentes interactivos
├── BODY
│   ├── Contenedor principal
│   │   ├── Título y subtítulo
│   │   ├── Grupo de entrada
│   │   ├── Botón de cálculo
│   │   └── Área de resultados
│   │       ├── Paso 1: Característica
│   │       ├── Paso 2: Mantisa
│   │       └── Resultado final
│   └── Script JavaScript
│       ├── Validación
│       ├── Cálculos matemáticos
│       ├── Extracción de información
│       └── Generación de HTML dinámico
```

## 📱 Compatibilidad

- ✅ Chrome/Edge (versión 90+)
- ✅ Firefox (versión 88+)
- ✅ Safari (versión 14+)
- ✅ Navegadores modernos en Android/iOS

## 🎓 Cómo Usar

1. **Abre el archivo** `index.html` en tu navegador
2. **Ingresa un número** en el campo de entrada (ej: 0.001349 o 134.9)
3. **Haz clic en "Calcular y Explicar"** o presiona Enter
4. **Lee el proceso paso a paso** para entender cómo se calcula
5. **Compara los dos formatos** de resultado (tabla vs decimal)

## 🧠 Conceptos Matemáticos

El logaritmo en base 10 se define como:
$$\log_{10}(N) = \text{Característica} + \text{Mantisa}$$

Donde:
- **Característica**: Un número entero (positivo, negativo o cero)
- **Mantisa**: Un número decimal entre 0 y 1 (siempre positivo)

Esta descomposición fue fundamental antes de las calculadoras:
- La **característica** se calculaba mentalmente
- La **mantisa** se buscaba en tablas impresas de 5+ páginas

Hoy en día, es una herramienta educativa valiosa para entender:
- La estructura de los logaritmos
- La notación científica
- Los órdenes de magnitud
- La historia de las matemáticas

## 📝 Licencia

Proyecto de código abierto para fines educativos.

## 👨‍💻 Autor

Desarrollado como una herramienta educativa para enseñar logaritmos usando métodos históricos.