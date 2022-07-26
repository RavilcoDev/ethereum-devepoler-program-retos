# Semana 3 [<img src="https://static.platzi.com/media/learningpath/badges/57d7a4b1-b706-454f-88a1-9fe36a1758f6.jpg" width="32">](https://platzi.com/clases/3235-ethereum-dev-program/52067-infraestructura-y-funcionamiento-de-la-ethereum-vi/)

## Tarea 1 - Ernesto García Ethereum Developer de Open Zeppelin nos invita a aprender y poner en práctica nuestro conocimientos a través de un repositorio y playground de opcodes EVM.

**Introduccion - Almacenamiento de datos**
![process-intro](./assets/process-intro.png
)
En este caso usaremos el siguente input ```0x363d3d37363df3```, este ingresa por calldata y se ejecutara el Opcode **36**
![process-1](./assets/process-1.png)
El siguiente es el **3D**( 2 veces)
![process-2](./assets/process-2.png)
Ahora **37** usara las entradas en el stack(pila), siendo primero el ultimo que ingresamos.
![process-3](./assets/process-3.png)
Volvemos a usar **36** y **3D** llenando nuevamente el stack.
![process-4](./assets/process-4.png)
Por último **F3** nos retornara por la pantalla el resultado
![process-5](./assets/process-5.png)

**Pueba del resultado**
[![result-in-evm](./assets/result-in-evm.png)](https://www.evm.codes/playground)



- **RECURSOS UTILIZADOS**
    - [Opcodes](https://www.evm.codes)
    - [EMV Playground](https://www.evm.codes/playground)
    - [Documentacion](https://www.evm.codes/about)
