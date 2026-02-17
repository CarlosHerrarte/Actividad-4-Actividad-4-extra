1. Funcionamiento del programa

El programa es un simulador de cotizaciones de seguros que realiza los siguientes pasos:

Inicio y ciclo principal:

Pregunta al usuario si desea “Cotizar” o “Salir”.

Si elige “Salir”, el programa termina.

Si elige “Cotizar”, comienza una nueva cotización.

Ingreso de datos del asegurado:

Nombre (solo texto)

Edad (solo números)

Estado civil (solo “SI” o “NO”)

Edad del cónyuge si está casado (solo números)

Hijos (solo “SI” o “NO”)

Cantidad de hijos (solo números)

Ingreso de datos financieros y patrimoniales:

Cantidad de propiedades (solo números)

Salario mensual (solo números)

Cálculo de recargos:

Según la edad del asegurado

Según la edad del cónyuge

Según la cantidad de hijos

Según la cantidad de propiedades (35% por propiedad)

Según los ingresos del asegurado (5% del salario)

Cálculo del precio final:

Precio final = Precio base + recargo total

Resultado:

Se muestran al usuario:

Nombre del asegurado

Recargo total

Precio final de la cotización

Repetición:

El programa vuelve a la pregunta inicial para permitir nuevas cotizaciones hasta que el usuario escriba “Salir”.

2. Partes del problema que se deben considerar

Validaciones de datos:

Evitar que se ingresen textos donde deberían ir números (edad, hijos, propiedades, salario).

Evitar respuestas distintas a “SI” o “NO” para preguntas binarias.

Cálculo de recargos:

Edad del asegurado

Edad del cónyuge

Cantidad de hijos

Cantidad de propiedades

Salario del asegurado

Control del flujo:

Permitir que el usuario haga múltiples cotizaciones.

Terminar el programa de manera segura con “Salir”.

3. Posibles mejoras

Refactorización con funciones:

Crear funciones para:

Validar texto y números

Calcular recargos

Mostrar resultados

Esto haría el código más limpio y fácil de mantener.

Uso de objetos:

Representar al asegurado como un objeto con propiedades: nombre, edad, casado, hijos, propiedades, salario.

Permitir calcular cotizaciones de manera más estructurada.

Interfaz más amigable:

Usar formularios HTML en lugar de prompt y alert, para una mejor experiencia de usuario.

Manejo de errores:

Actualmente se repite el prompt en bucles infinitos; se podría agregar un límite de intentos.

Flexibilidad en recargos:

Guardar los porcentajes de recargos en una estructura de datos, lo que facilitaría cambios futuros sin modificar todo el código.
