## Funcionalidades

### Funcionando correctamente:

- Registrar pacientes con sus datos básicos y una prioridad inicial.
- Asignar o modificar la prioridad de los pacientes.
- Ver la lista de espera de pacientes, ordenada por prioridad y hora de registro.
- Atender al siguiente paciente, respetando el orden de prioridad.

### Problemas conocidos:

- La funcionalidad al asignar una prioridad a un nombre que no hay, se repite el texto anterior, por lo tanto no es tan amigable al saber cuando se equivoca.

### A mejorar:

- Implementar una interfaz de usuario más amigable.
- Implementar una función que detecte el sintoma automaticamente y le asigne prioridad.
- Implementar una función que detecte segun la edad y el sintoma, la prioridad. (Ej: Niño de 8 años con hipotermia y un hombre de 25 años con hipotermia)

## Ejemplo de uso

**Paso 1: Registrar un Nuevo Paciente**

Se comienza registrando un nuevo paciente que acaba de llegar al hospital.

```
Opción seleccionada: 1) Registrar paciente
Ingrese el nombre del paciente: Joaquín Cornejo
Ingrese la edad del paciente: 25
Ingrese el síntoma del paciente: Dolor de cabeza
```

El sistema registra a Joaquín Cornejo con una prioridad inicial "Bajo" y guarda la hora actual de registro. La prioridad inicial puede ser ajustada más tarde basada en una evaluación médica más detallada.

**Paso 2: Asignar Prioridad a un Paciente**

Tras una evaluación inicial, el médico determina que el estado de Ana requiere atención prioritaria.

```
Opción seleccionada: 2) Asignar prioridad a paciente
Ingrese el nombre del paciente: Joaquín Cornejo
Seleccione el nuevo nivel de prioridad (Alto, Medio, Bajo): Alto
```

El sistema actualiza la prioridad de Joaquín Cornejo a "Alto", asegurando que será una de las próximas pacientes en ser atendida.

**Paso 3: Ver la Lista de Espera**

El usuario revisa la lista de espera para ver todos los pacientes y sus prioridades.

```
Opción seleccionada: 3) Mostrar lista de espera
```

La lista muestra a Joaquín Cornejo en la parte superior, indicando su prioridad alta y que es la siguiente en línea para recibir atención.

**Paso 4: Atender al Siguiente Paciente**

Joaquin Cornejo es llamada para ser atendida basándose en su prioridad.

```
Opción seleccionada: 4) Atender al siguiente paciente
```

El sistema muestra que Joaquín Cornejo está siendo atendida y la elimina de la lista de espera.
