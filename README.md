# Estruturas de Dados: Filas e Pilhas em Java

## Descrição
Este projeto implementa diferentes estruturas de dados dinâmicas em Java, incluindo:
- Filas circulares com redimensionamento automático.
- Filas baseadas em arrays com estratégias de crescimento incremental e duplicativo.
- Filas encadeadas utilizando listas ligadas.
- Pilha encadeada para manipulação de dados em ordem LIFO.

## Estruturas Implementadas
### Filas
- **FilaCircular**: Implementação baseada em array circular, com redimensionamento dinâmico por duplicação.
- **FilaDuplicacao**: Fila com crescimento dinâmico utilizando estratégia de duplicação.
- **FilaIncremento**: Similar à anterior, mas expande o array com um incremento fixo.
- **FilaEncadeada**: Fila baseada em lista ligada.

### Pilhas
- **PilhaEncadeada**: Implementação de pilha com lista ligada.

### Exceção
- **FilaVaziaException**: Exceção personalizada para filas vazias.

### Interfaces e Classes Auxiliares
- **IFila**: Interface para padronizar a implementação das filas.
- **No**: Representa um nó para listas encadeadas.

## Como Executar
O projeto contém classes de teste para validação das estruturas implementadas. Para executar os testes:

1. Compile os arquivos Java:
   ```sh
   javac *.java
   ```
2. Execute a classe de teste:
   ```sh
   java TesteEstruturasEncadeadas
   ```

## Testes Incluídos
- **TesteEstruturasEncadeadas**: Testa filas e pilhas, incluindo um algoritmo para inverter a ordem dos elementos de uma fila utilizando uma pilha.
- **TesteFila (na FilaCircular)**: Testa a inserção, remoção e redimensionamento automático da fila circular.

## Exemplo de Uso
### Criando e manipulando uma fila encadeada:
```java
FilaEncadeada fila = new FilaEncadeada();
fila.enqueue("A");
fila.enqueue("B");
fila.enqueue("C");
System.out.println(fila.first()); // Saída: A
System.out.println(fila.dequeue()); // Remove A
```

### Criando e manipulando uma pilha encadeada:
```java
PilhaEncadeada pilha = new PilhaEncadeada();
pilha.push("1");
pilha.push("2");
pilha.push("3");
System.out.println(pilha.peek()); // Saída: 3
System.out.println(pilha.pop()); // Remove 3
```
