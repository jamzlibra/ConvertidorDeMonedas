# Currency Converter

Este proyecto es un conversor de moneda desarrollado en Java, que permite a los usuarios convertir monedas entre diferentes países utilizando la API de ExchangeRate-API y la API de RestCountries.

## Descripción del Proyecto

El conversor de moneda es una herramienta que facilita la conversión de montos entre diversas monedas. Proporciona una interfaz interactiva para seleccionar pares de monedas y realizar conversiones, con soporte adicional para obtener monedas de países especificados por el usuario.

### Características principales

- **Conversión de monedas comunes**: Opciones predefinidas para convertir entre EUR, USD y MXN.
- **Conversión de otras monedas**: Permite la entrada de cualquier par de países para obtener sus monedas y realizar la conversión.
- **Interfaz interactiva**: Solicita entradas del usuario y proporciona resultados en tiempo real.
- **Manejo de errores**: Muestra mensajes de error claros cuando no se puede realizar la conversión.

### APIs utilizadas

- **ExchangeRate-API**: Para obtener las tasas de conversión entre diferentes monedas.
- **RestCountries API**: Para obtener el código de moneda correspondiente a un país.

### Métodos de Conversión

El proyecto utiliza la API de ExchangeRate-API para obtener las tasas de conversión y la API de RestCountries para obtener el código de moneda correspondiente a un país.

### Cómo funciona

1. El usuario selecciona una opción de conversión predefinida o elige "Otros países" para especificar países personalizados.
2. Si se selecciona "Otros países", el usuario ingresa los nombres de los países de origen y destino.
3. El sistema obtiene el código de moneda correspondiente a los países ingresados.
4. El usuario ingresa la cantidad a convertir.
5. El sistema realiza la conversión y muestra el resultado.

## Uso

### Ejecución del programa

Para ejecutar el programa, necesitas tener configurado el entorno de Java. El programa se ejecuta desde la línea de comandos:

```sh
java -cp .;gson-2.10.1.jar com.conversor.CurrencyConverter
```

### Ejemplo de uso

1. Seleccionar una opción de conversión:
    ```
    Seleccione una opción:
    1. EUR a USD
    2. EUR a MXN
    3. USD a EUR
    4. USD a MXN
    5. MXN a EUR
    6. MXN a USD
    7. Otros países
    Opción: 7
    ```

2. Ingresar los nombres de los países:
    ```
    Ingrese el nombre del primer país:
    Canada
    Ingrese el nombre del segundo país:
    Japon
    ```

3. Ingresar la cantidad a convertir:
    ```
    Ingrese la cantidad a convertir:
    500
    ```

4. Resultado:
    ```
    500 CAD = XXX JPY
    ```

## Registro de versiones

### Versión 1.0.0
- **Versión 1.0.0** (05/05/2024): Implementación inicial de la funcionalidad básica de conversión de monedas.

## Autor
- [Julio Macias](https://github.com/jamzlibra)
