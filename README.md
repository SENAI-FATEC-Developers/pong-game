# Conhecimentos basicos de Javascript


## Tipos primitivos do JAVASCRIPT
-----------------

1- **Number**: é o número e podemos fazer operações sobre eles.      
    `12% 5`

    ```
        #- 12 % 5 : % é o módulo , então ele me dá o resto 12/5
       
    ```  

2- **String**: é a tipagem de texto , use "" ou ''' para informar que algo é string. 
Ex: `"Kayle" + "VII"`

#- Concatenação: number + string = string. `10 + ""20" = "1020"`

 #- NaN: Não é um numero

3. **Boolean**: Siginifica apenas True or False ,  pode ser usado também 0 ou 1 para representa-los no codigo. 
Ex:  `3 > 2 -> True`

#- Diferenças dos simbolos "=":

#- Para igualdade use: == . `3==3 -> true`

#-  Para igualdade de valor e tipo: === . `3===3 -> true`

#- Para negação da igualdade ( não é igual): !== . `3 !== 3 -> false`

#- Simbolos de comparação , maior , menor etc: >= , <= , < , > 


4. **Undefined**: Significa que a variável não foi atribuída ou que não retornamos algo em uma função.
5. **Null**: diz que um objeto é nulo, significa que isso não tem nada no objeto. 
6. **Symbol** : è um novo recurso não é muito usado mas depois pretendo coloca-lo. 

7. **Object** :  São coleção de propriedades , usando a logica "chave - valor" 
    `var user ={ name: "Peter", age:"24",} `

**Comparadores JAVASCRIPT**
    !== , === , >= ,<= ,> , <

## Variaveis JAVASCRIPT
-----------------
**Regras**: 
    1-  precisa começar com uma letra (pode terminar com um número). 

    2- Não pode começar com simbolo ou caractere special tipo @#$% . 
        Ex: `var ^a`

    3- Não pode começar com '$' or '_' (sublinhado)

    4- JS e  Casesensitive então há diferença entre digitar maiuscula e minuscula.  
        Ex: `var CASE` e diferente do que `var case`  então use `firsCase` para nomes grandes

**var**: Armazena valores em memória, também pode conter qualquer tipo do JS, você pode reatribuir um valor. 

**semicolon** ";" :  siginifica o fim de uma expressão.

#$- Expression:  è um fragmento de codigo que produz um valor.  

**=:** `var sa = 3` adiciona 3 ao sa,  não pode começãr com um numero. 

**prompt()**: È uma função que retorna o  o que você digita no alerta de entrada que aparece no navegador. (os valores mudam para strings). 

**number(variavel)**: È uma função que muda o valor da variavel para tipo numero, como a string "3" para 3 , so funciona com valores de numeros

    <!-- let (new in ECMAScript 6)-->  Abordarei ECMAScript mais tarde. 
    <!-- const (new in ECMAScript 6)-->


## Condicionais JAVASCRIPT 
-----------------
**if**:  Serve condições "if" ou "se" para fazer algo.
Ex: `if(conditions) {}`.

**else** :  Serve para uma condição oposta ao "se" ou "if" .  

Ex: `else{something occurs}` ou `if(conditions) {} else{something occurs}`.

**else if**: Serve para uma recomeçar a condição "if" apartir de uma contradição "else". 

Ex: `else if {something}` or `if(conditions) {} else if {something occurs}`.

    Abordarei mais tarde:
    <!-- ternary operator --> : 
    <!-- switch -->


## Operadores logicos do JAVASCRIPT 
-----------------

**&&:** Siginifica "and" no JS

**||:**  Siginifica "or" no JS

**ReferenceError**: E um erro do JS , e como se ele estivesse te falando : "Não sei qual é este valor, não está se referindo a nada"

**!:** Siginifica "not" no JS, 

 Ex: `if (!(name === "Null"))...`

# Funções do JAVASCRIPT  
-----------------

## O que são funções 

São peças de código, que executam ações, podemos utilizar as funções JS ou criar as nossas próprias (também podemos chamá-las a qualquer momento como quisermos). a () significa executar (chamar) a função `alert()`.

**argumentos**: são as coisas dentro de () quando uma função é chamada de `alert("Oi") `.

**console.log():** Serve para mostrar retornos de variaveis ou funções no console do navegador ou terminal.   

- Expressão de função:  
    Ex: `var a = function name() { return} `

- Função anonima: 
    Ex:`var name = function( ) {return)}:` 

- Declaração da função : 
    Ex: `function name() { return}  : `

return: Diz o que o resultado da função é , além disso nós permite usar o valor dessa função fora dela .
   
<!-- () => (new in ECMAScript 6) --> Abordarei Arrow function futuramente. 


**Parametros de uma função**: Adiciona parâmetros para você não se repetir, isto é "variáveis" que armazenam os valores submetidos quando você chama a função e passa o argumento.  

            ```
                function sing(song) { console.log(song)}
                sing("Legend's never die , they become...") 
            ```

## Estrutura de  dados do JAVASCRIPT 
-----------------
São formas de armazenamento de dados.

**Array** : representa por [] é uma lista de dados/elementos. Para acessar um valor, chame para o nome da lista e informe a posição dentro [] , dica: sempre faça arrays com apenas um tipo.

         Ex: like  `var list = ["tiger","car"..]; list[1]`

        index: são o número de comprimento/posição de uma matriz 

Obs1: arrays precisam estar em variáveis ou as mudanças neles não serão validas;  

Obs2: Há métodos/funções de array que criam uma nova lista como concat e outros que modificam a atual como pop ou shift.

Obs3: Para acessar um objeto dentro de um array use:
    `arrayName[position].objectPropertie` como em `database[0].username`

**Quais tipos de dados um Array pode armazenar ?**
string.booleans,numbers,functions , ou todos misturados (embora seja recomendado usar apenas um tipo) , ou podemos adicionar um array dentro de outro. 
        Ex: `list[0][2]`
         
**Object**: Podemos ter propriedades e valores, usamos para armazenar informações de um objeto (algo importante como usuários, compromissos, tipos de algo , etc.):  

 Ex: `objectName.propertieName` like `user.name`:  `var user = { properties:value,... } `

#- Para adicionar novas propriedades use: 

`objectName.newPropertieName = value` como em  `user.favouriteFood = "spinach`.

#- Para alterar valores use: 

`objectName.newPropertieName = value`

#-Podemos adicionar funções dentro de objetos , mas elas agora serão chamadas de metodos.      

`shout: function() { console.log("Welcome to League of Draven")} `

#- Podemos adicionar Arrays em Objetos e Objetos dentro de Arrays. 
                `var list = [ { username="kayle"}]`

Acessando dados de um array dentro do objeto : 
        object -> array: `user.spells[1]`

Acessando dados de um objeto dentro do array : 
        array -> object: `list[0].password`

#- Uma função dentro de um objeto é um "método", como `user.shout()`;

#- Podemos ter Arrays ou objetos vazios 
Ex: `var user = {}` ou `var user = []`

## JAVASCRIPT Loops
-----------------
**for**: executar um loop, dependendo de uma condição. 

Ex: `for (var i=0; i < todos.length; i++){}`

    ++ :  use para incrementar um valor em  +1 

**while**: é o mesmo de "for" mas o contador está fora da função e verifica a condição primeiro  do que  o "do while".  

    ```
        var counterOne = 0;
        while(conuterOne < 10) { 
            console.log(counterOne);
            counterOne++
        }
    ```
**do while**: "do while" é um pouco diferente do que "while", pois isso Faz algo primeiro e depois verifica a condição:  
   
        ```
            var count = 10
            do { 
                console.log(count);
                count--
            } while (count > 0)
        ```
**forEach**: 
    Isto executa algo para cada item de um Array, portanto devemos coloar as ações que podemos fazer na função. 

    1- argumento : È cada item desse Array.

    2- argumento : È o índice desse item. 

    Obs:  Podemos fazer uma função fora de um forEach e colocá-lo dentro dele para manipular mais facilmente as informações. 

     ```
  
        function logTodos(todo,i){
            console.log(todo,i);
        }

        todos.forEach(logTodos)
        todosImportant.forEach(logTodos);
    ```

