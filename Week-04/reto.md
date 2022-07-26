# Semana 3 [<img src="https://static.platzi.com/media/learningpath/badges/57d7a4b1-b706-454f-88a1-9fe36a1758f6.jpg" width="32">](https://platzi.com/clases/3235-ethereum-dev-program/52068-crea-tu-primer-smart-contract-actividades/)

**Reto #1**
Investigar que son los Events en Solidity. Luego, debes implementar un evento que se llame eventNewPokemon, el cual se disparará cada vez que un nuevo Pokemon es creado. Lo que emitirá el evento será el Pokemon que se creó.

**Reto #2**
Investigar sobre “”require” .
Entonces, antes de agregar un nuevo Pokemon, se debe validar que el id sea mayor a 0. De lo contrario, se debe desplegar un mensaje que corrija al usuario.
Entonces, antes de agregar un nuevo Pokemon, se debe validar que el name no sea vació y mayor a 2 caracteres. De lo contrario, se debe desplegar un mensaje que corrija al usuario.

**Reto #3**
Los Pokemons han evolucionado, ahora tienen una lista de habilidades (Habilities). Es decir, un Pokemon puede tener 1 ó muchas habilidades, cada habilidad tiene el siguiente formato: - Name - Description

**Reto #4** - Estudiante distinguido
Los Pokemons pueden pertenecer a más de un tipo (Type), por ejemplo: Bulbasaur es de tipo Grass y Poison. Proponga una solución e impleméntela.

Los Pokemons tienen debilidades (Weaknesses) las cuales pueden ser otros tipos de pokemones. Por ejemplo, Bulbasaur es débil contra pokemones de tipo Fire, Flying, Ice, Psychic. Proponga una solución e impleméntela.

- Resolucion 

1. **Reto : events** - me percate que uint gastaba menos gas que uint8, luego buscando encontre que era por la conversion que se hace de 256 a 8, por lo que ¿cuando usar uint menores a 256?, en bloques y cuando se guarda en storage, cada bloque usa 256 al guardar en storage por lo que debes hacer tetriz y completar bloques que sumados den 256.
2. **Reto : require** - use una conversion string a bytes para validiar la logitud de caracteres
3. **Reto : structure**: creé un estructura para la habilidades y la referencia por el index en la estructura de pokemon además de crear una función para crear nuevas habilidades que actualiza el indice máximo (para poder hace validaciones luego)
4. **Reto**: decidi crear un nuevo documento para manejar los tipo y debilidades ademas de exponer las respectivas debilidades medieante un par de funiones
- **Pruebas**
    - [PullRequest](https://github.com/gelopfalcon/solidity-eth-challenge/pull/15)
    - [GitHub](https://github.com/RavilcoDev/solidity-eth-challenge/tree/patch-1)
