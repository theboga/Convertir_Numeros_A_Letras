# Convertir números a Letras en JavaScript
Función que convierte un número o cantidad a letras en JavaScript ideal para una factura cheques o sistemas que necesiten mostrar en letra una cantidad  Es personalizable y configurarse para cualquier moneda USD PesosMX etc.

Puedes probar el código Aquí: https://jsfiddle.net/the_boga/k9ms7pxd/4/

``` javascript
numeroALetras(1120) // Devuelve - Mil ciento veinte Pesos
numeroALetras(3850512.12) // Devuelve - Tres millones ochocientos cincuenta mil quinientos doce Pesos y doce centavos

```
### Configuración

``` javascript
  //***** CONFIGURACIÓN ****
  // UDS - Pesos MX - Pesos colombianos etc. determina la etiqueta de la moneda
  const moneda = "USD"; 
  // puedes usar "con" o "y" Chiquipesos - centavos etc.
  const cents  = ["y", "Centavos"]; 
  // 1 = Todo minúsculas, 2 = Todo Mayúsculas, 3 = Title case moneda Mayúscula, 
  // 4 = Todo minúculas y moneda Mayúscula, 0 = Camel Case 
  const format = 3
```
---
#### Configurando la Moneda
***moneda*** Puedes cambiar el tipo de moneda ejemplo:

``` javascript
const moneda = "USD"; 

```
``` javascript
console.log( numeroALetras(1120) ) // Devuelve - Mil ciento veinte USD

```
---
#### Configurando los centavos
***cents*** Puedes cambiar la terminación de los centavos ejemplo

``` javascript
const cents  = ["con", "Centavos"]; 

```
``` javascript
console.log( numeroALetras(1120.50) ) // Devuelve - Mil ciento veinte USD con cincuenta Centavos

```
---
#### Configurando el formato
***moneda*** Puedes cambiar el formato de Salida ejemplo:

``` javascript
// 1 = Todo minúsculas, 2 = Todo Mayúsculas, 3 = Title case moneda Mayúscula, 
// 4 = Todo minúculas y moneda Mayúscula, 0 = Camel Case 
  const format = 2

```
``` javascript
console.log( numeroALetras(1120.50) ) // Devuelve - MIL CIENTO VEINTE USD CON CINCUENTA CENTAVOS

```
---
