# Preguntas y respuestas del tutorial:
### 	¿Puedes entender las diferencias entre las dos propuestas?
### Sí, en la versión con DI la vista recibe el almacenamiento desde afuera a través del factory, sin saber qué implementación es. En la versión sin DI la vista crea directamente ImageLocalStorage() adentro, acoplándose a esa clase específica.

### ¿Ventajas/desventajas de cada una?
### Con DI es más flexible y testeable pero más complejo de entender. Sin DI es más simple y directo pero si mañana quiero cambiar el almacenamiento a S3 por ejemplo, toca modificar la vista directamente, lo cual no es ideal.

### 