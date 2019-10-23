# Estrutura de dados e Algoritmos

## 1. Arrays

### Data Structure vs API

<br>Data
<br>     > Usa em API
<br>     > Insere/deleta e procura
<br>     > Estruturas primitivas que construímos coisas com elas
<br>     > Array/Linked List/Binary Tree
     
 API 
 <br>   > Collections e algoritmos construídos em uma delas  - ArrayList
                                                         - Stacks + Queues
                                                         - Binary Heap
                                                       
### 3 coisas que precisa saber
- 1 Podem conter qualquer coisa
<br>Number, strings e até outros arrays. Quando você cria um array você tem que especificar o tamanho.
<br> ex: Object [ ] objects = new Object [10]; | Object[10] = fixed size

- 2 Tamanhos fixos 
<br>Arrays tem tamanhos fixos, ou seja, elas não podem crescerm pelo menos não por elas mesmas.

- 3 Acesso randominco/aleatório
<br>Usando um "array index" você pode acessa qualquer elemento

#### "A killer feature de um array é poder acessar qualquer elemento"

### Inserir, deletar e redimensionar

Inserindo - Criar espaço para o elemento "jogando" ele para o lado mas prestando atenção na capacidade total de dados ou no número de elementos.
<br>Deletando - Não precisa necessariamentte deletar/remover, apenas subescrever basta.
<br>Redimensionando - Array tem tamanhos fixos, mas podemos criar uma estrutura de dados - lembrar que ter espaços extras demais não é bom. Dynamic arrays é uma maneira de redimensionar o tamanhos de um array "copiando" a estrutura original e criando outra com mais espaços.
