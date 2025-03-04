READ ME - TABELA HASH EM JAVA

1. DESCRIÇÃO

  Este projeto consiste na implementação de uma Tabela Hash em Java, que segue as especificações fornecidas. 
  A Tabela Hash é uma estrutura de dados fundamental em ciência da computação, usada para armazenar e recuperar informações de maneira eficiente.
  Este é um programa Java que demonstra a implementação de uma tabela hash para armazenar alunos usando o conceito de sondagem linear. 
  A função de hash utilizada neste programa é simples e pode ser personalizada para atender às necessidades do seu projeto. Ela usa o cálculo do módulo para determinar a posição de armazenamento de um aluno na tabela hash.

2. FUNCIONALIDADE

  O programa permite realizar as seguintes operações em uma tabela hash de alunos:
  
  - Inserir um aluno na tabela hash.
    
  - Remover um aluno da tabela hash.
    
  - Buscar um aluno na tabela hash.
    
  - Imprimir o conteúdo da tabela hash.
  
  O fator de carga da tabela hash (número de elementos / tamanho da tabela) é calculado e exibido.

3. REQUISITOS FUNCIONAIS

  Requisitos Mínimos
    
    1. O código está limpo e organizado. Os nomes de atributos e métodos são claros. Os métodos
    são definidos de forma correta para melhor organização de código e reutilização de
    funcionalidades. (1,0)
    
    2. A função hash evita ao máximo colisões, possui baixa complexidade matemática e funciona
    corretamente para os dois tipos de chaves: int e String. (1,0)
    
    3. A inserção é feita de forma correta, utilizando a função hash, e implementada de acordo
    com as especificações definidas no item 1 deste documento. (1,0)
    
    4. A busca é feita de forma correta, utilizando a função hash, e implementada de acordo com
    as especificações definidas no item 1 deste documento. (2,0)
    
    5. A remoção é feita de forma correta, utilizando a função hash, e implementada de acordo
    com as especificações definidas no item 1 deste documento. (2,0)
    
    6. Ao menos dois tipos de tratamento de colisão foram implementados. (1,0)
    
    7. O código possui teste de eficiência na busca. (1,0)
    
    8. O código possui feedback de funcionamento com impressão de valores obtidos a partir de
    uma chave. (1,0)
    
  Requisitos Extras
    
    1. O código está armazenado em um repositório Github com descrição explicativa sobre a
    funcionalidade do programa. (TDE - 1,0)

4. USABILIDADE
  
  Java Development Kit (JDK) instalado.
  
  a. Clone o repositório ou faça o download do código-fonte.
  
  b. Compile o código Java (Main.java).
  
  c. Execute o programa.
  
  d. Siga as instruções do programa para realizar as operações na tabela hash.

5. ESTRUTURA
  
   - Aluno.java: Definição da classe Aluno.

  - Hash.java: Definição da classe Hash e implementação da tabela hash.
 
  - Main.java: Programa principal para interação com o usuário.

6. SINTAXE

  Classe Aluno
  
    - Aluno(): Este é o construtor padrão da classe Aluno. Ele é usado para criar uma instância de aluno com valores padrão. O número de registro (RA) é definido como -1, e o nome é definido como uma string vazia.
 
    - Aluno(int ra, String nome): Este é um construtor personalizado da classe Aluno. Ele permite criar uma instância de aluno com um RA e um nome específico.
  
    - obteRa(): Este método retorna o número de registro (RA) do aluno.
 
    - obterNome(): Este método retorna o nome do aluno.

  Classe Hash
   
    - Hash(int tam_vetor, int max): Este é o construtor da classe Hash. Ele é usado para criar uma tabela hash com um tamanho especificado (tam_vetor) e um número máximo de elementos (max). Ele inicializa a tabela hash e outros atributos.
   
    - estaCheio(): Este método verifica se a tabela hash está cheia, ou seja, se o número de elementos nela é igual ao número máximo de elementos especificado.
   
    - obterTamanhoAtual(): Retorna o número atual de elementos na tabela hash.
   
    - inserir(Aluno aluno): Este método insere um aluno na tabela hash. Ele usa uma função de hash para calcular a posição de inserção do aluno. Se a posição estiver ocupada, ele faz sondagem linear para encontrar a próxima posição vazia.
   
    - deletar(Aluno aluno): Remove um aluno da tabela hash com base no seu número de registro (RA). Ele encontra a posição do aluno usando a função de hash e, em seguida, verifica se o aluno existe naquela posição antes de removê-lo.
  
    - buscar(int ra): Este método busca um aluno na tabela hash com base no seu RA. Ele usa a função de hash para encontrar a posição inicial e verifica se o aluno está naquela posição ou faz sondagem linear para encontrar o aluno desejado.
  
    - imprimir(): Imprime o conteúdo da tabela hash, exibindo as informações dos alunos armazenados.
   
    - FuncaoHash(Aluno aluno): Esta é uma função de hash simples que recebe um objeto Aluno e retorna uma posição na tabela hash com base no RA do aluno. Você pode personalizar essa função de hash de acordo com as necessidades do seu projeto.

Classe Main
    - main(String[] args): Este é o ponto de entrada do programa. Ele lida com a interação do usuário, permite que o usuário escolha ações como inserir, remover, buscar e imprimir alunos na tabela hash, e interage com as classes Aluno e Hash.

7. EXEMPLO DE IMPRESSÃO

 
  Programa gerador de Hash!
 
  Digite o tamanho da Hash!
 
  10
  
  Digite o numero maximo de elementos!

  10
 
  O fator de carga e: 1.0
 
  Digite 0 para parar o algoritmo!
 
  Digite 1 para inserir um elemento!

  Digite 2 para remover um elemento!
 
  Digite 3 para busca um elemento!
 
  Digite 4 para imprimir a Hash!
  
  1

  Qual e a matricula do aluno?
 
  5
 
  Qual e o nome do aluno?
 
  pEDRO
 
  Digite 0 para parar o algoritmo!
 
  Digite 1 para inserir um elemento!
 
  Digite 2 para remover um elemento!
 
  Digite 3 para busca um elemento!
 
  Digite 4 para imprimir a Hash!
 
  4
 
  Tabela Hash:
 
  5:5 pEDRO
 
  Digite 0 para parar o algoritmo!

  Digite 1 para inserir um elemento!
 
  Digite 2 para remover um elemento!

  Digite 3 para busca um elemento!
 
  Digite 4 para imprimir a Hash!
 
  0
  
  Process finished with exit code 0

8. AUTORES
 
  Código elaborado por Pedro Noah Milarski e Vitor Bertoldi
