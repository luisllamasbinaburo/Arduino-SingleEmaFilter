# Librería Arduino Single EMA
Librería para Arduino que implementa un filtro exponencial (EMA). La librería permite realizar filtros de paso bajo (low pass filter) y paso alto (high pass filter).

Más información https://www.luisllamas.es/libreria-arduino-single-ema/

## Instrucciones de uso

### Constructor

El filtro Single EMA se instancia a través de su constructor que recibe el parámetro Alpha del filtro como único valor.

```c++
SingleEMAFilter<int> singleEMAFilter(const size_t alpha);
```

### Filtrar señal
```c++
// Añadir un nuevo valor al filtro y devolver el valor filtrado Low Pass
singleEMAFilter.AddValue(value);
 
//Obtiene el ultimo valor filtrado Low Pass (el mismo que el devuelto al añadir el valor al filtro)
singleEMAFilter.GetLowPass();
 
//Obtiene el ultimo valor filtrado High Pass
singleEMAFilter.GetHighPass();
```

## Ejemplos
La librería Single EMA Filter incluye los siguientes ejemplos para ilustrar su uso.
* SingleEMAFilterInt: Ejemplo de filtrado para variables integer.
* SingleEMAFilterFloat: Ejemplo de filtrado para variables float.
