## 1. Fundamentos e Teoria (2-4 semanas)

Antes de colocar a mão na massa, é crucial entender a teoria por trás de um compilador.

### Tópicos para Estudo

* **Linguagens Formais e Autômatos:** Compreenda as bases teóricas.
    * **Gramáticas:** Regular, Livre de Contexto e Sensível ao Contexto. A maioria das linguagens de programação usa gramáticas Livres de Contexto.
    * **Autômatos Finitos:** Determinísticos (DFA) e Não Determinísticos (NFA). Essenciais para a análise léxica.
    * **Máquinas de Turing:** Entenda o que é uma computação e os limites de um autômato.
* **Estrutura de um Compilador:** Conheça as fases principais de um compilador.
    * **Análise Léxica:** Transforma o código-fonte em *tokens*.
    * **Análise Sintática:** Organiza os *tokens* em uma estrutura hierárquica (árvore sintática).
    * **Análise Semântica:** Verifica a correção lógica e de tipos do código.
    * **Geração de Código Intermediário:** Cria uma representação mais abstrata do código.
    * **Otimização de Código:** Melhora o código intermediário.
    * **Geração de Código de Destino:** Produz o código final (Assembly, bytecode, etc.).

### Recursos Recomendados

* **Livros:**
    * *Compiladores: Princípios, Técnicas e Ferramentas* (também conhecido como "Livro do Dragão") de Aho, Lam, Sethi e Ullman. É a bíblia da área. Pode ser denso, mas é essencial.
    * *Engineering a Compiler* de Keith D. Cooper e Linda Torczon. Uma abordagem mais prática e moderna.
* **Cursos Online:**
    * Cursos de teoria da computação em plataformas como Coursera ou edX.
* **Ferramentas:**
    * `flex` (ou `lex`) e `bison` (ou `yacc`) para ter uma ideia de como funcionam os geradores de analisadores léxicos e sintáticos.

---

## 2. Implementação das Fases do Compilador (8-12 semanas)

Nesta etapa, você começará a construir seu próprio compilador, passo a passo, em C. O ideal é começar com uma linguagem de brinquedo, com poucas funcionalidades. Por exemplo, uma linguagem que suporte apenas atribuições, operações aritméticas e impressão.

### 2.1. Análise Léxica (2 semanas)

* **Objetivo:** Ler o código-fonte e converter os caracteres em uma sequência de *tokens*.
* **Tarefa:** Implemente uma função que, a cada chamada, retorne o próximo *token* do código. Você precisará de uma estrutura para representar o *token* (tipo, valor, linha, coluna). Use uma máquina de estados finitos simples para identificar *tokens* como números, identificadores, operadores e palavras-chave.

### 2.2. Análise Sintática (4 semanas)

* **Objetivo:** Organizar os *tokens* em uma Árvore de Sintaxe Abstrata (AST - Abstract Syntax Tree).
* **Tarefa:** Implemente um *parser*. O método mais comum para iniciantes é o *Recursive Descent Parsing*. Crie uma função para cada regra da sua gramática. O resultado será a AST, que é uma representação hierárquica do programa.

### 2.3. Análise Semântica (2 semanas)

* **Objetivo:** Verificar se o programa faz sentido.
* **Tarefa:** Percorra a AST e realize verificações, como:
    * Declarar e usar variáveis (tabela de símbolos).
    * Verificar a compatibilidade de tipos.

### 2.4. Geração de Código (2-4 semanas)

* **Objetivo:** Traduzir a AST para uma linguagem de destino.
* **Tarefa:** Percorra a AST e gere código. Para simplificar, comece gerando código em uma linguagem intermediária como o bytecode da JVM ou LLVM IR. Uma alternativa ainda mais simples é gerar código em C e usar o compilador C para gerar o executável final.

---

## 3. Otimização e Melhorias (Tempo contínuo)

Com um compilador funcional, você pode começar a adicionar recursos e otimizações.

### Tópicos Avançados

* **Geração de Código de Máquina:** Em vez de gerar C, produza código Assembly para uma arquitetura específica (ex: x86-64 ou ARM).
* **Otimizações:** Implemente otimizações de baixo nível e alto nível (ex: *dead code elimination*, *constant folding*, *loop unrolling*).
* **Tratamento de Erros:** Melhore a maneira como o compilador lida com erros, fornecendo mensagens de erro mais claras.
* **Gerenciamento de Memória:** Implemente um coletor de lixo (*garbage collector*) para a sua linguagem, se for o caso.