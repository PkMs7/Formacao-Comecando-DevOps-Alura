# Tópicos sobre Começando em DevOps

## Conteúdo de artigos e Alura+

### O que é DevOps?

- DevOps: Desenvolvimento(Desenvolvimento de código, novas funcionalidades) / Operações(Monitoramento, infraestrutura, saúde do sistema que está em disponibilizaçõa, garantia de estabilidade).

- Desenvolvedores são mais maleáveis, aceitam melhor a mudança. Operações são menos flexíveis, geralmente partindo da premissa "Não toque num sistema que está funcionando". O movimento DevOps quer derrubar essa barreira, num cenário de implementação de novas funcionalidades (desenvolvimento), sem que isso derrube o que já está funcionando (operações).

- Importância da visibilidade dos scripts de ambientes e configurações, para que todos entendam onde e o que está acontecendo.

- ![Algumas ferramentas de DevOps](/Anexos/img/ferramentasDevOps.png)

### O que você precisa saber para começar em DevOps?

- DevOps: É uma cultura na engenharia de software que aproxima os desenvolvedores de software (Dev) e os operadores do software / administradores do sistema (Ops).

- DevOps precisa conhecer um pouco do lado do dev pois facilita a configuração de ambiente e prepara o local para integrar com as variáveis de ambiente e dependências por exemplo.

- Ifraestrutura como Código (IaC): é um processo de gerenciamento de infraestrutura de TI que aplica as práticas recomendadas do desenvolvimento de software DevOps ao gerenciamento de recursos de infraestrutura de nuvem.

- Terraform: é uma ferramenta de software de infraestrutura como código criada pela HashiCorp. Os usuários definem e fornecem infraestrutura de data center usando uma linguagem de configuração declarativa conhecida como HashiCorp Configuration Language ou, opcionalmente, JSON.

- Idempotência: é a propriedade que algumas operações têm de poderem ser aplicadas várias vezes sem que o valor do resultado se altere após a aplicação inicial.

### Guia de Carreira: DevOps - Youtube

- DevOps vem pra resolver os problemas de demora de entrega de um software e problemas de deploy do software em produção.

- Guia da conversa: https://techguide.sh/




## Conteúdo dos módulos de treinamento

### Arquitetura de computadores: por trás de como seu programa funciona

#### 1.0 Como o computador lê o seu código

- Bit: Binary Digit ou dígito binário. Essa é a menor unidade possível para o armazenamento de informação.

- Byte: Costuma-se trabalhar com grupos de 8 bits, essa quantidade agrupada de bits é chamada de byte.

- Liguagens Compiladas (Compiladores): Traduzem em um arquivo o código de alto nível em código de máquina.

- Liguagens Interpretadas (Tradutores): Traduzem linha a linha e executam no mesmo momento o código de alto nível em código de máquina.

- JIT (Just In Time) Compilation: Também conhecida como tradução dinâmica, é a compilação de um programa em tempo de execução , usando uma abordagem diferente da compilação anterior à execução. Geralmente, consiste em transformar o código em código de máquina, que é então executado diretamente, mas também pode se referir a tradução para outros formatos.


#### 2.0 Como o computador executa um programa?

- Memória não volátil: Consiste no tipo de armazenamento de memória do computador em que se pode persistir dados; isto é: uma vez gravados, os dados são conservados e portanto não há perda ao se retirar a fonte de energia. (HD ou SSD)

    - HD (Hard Drive): Um dispositivo de armazenamento de dados eletromecânico que armazena e recupera dados digitais usando armazenamento magnético e um ou mais pratos rígidos de rotação rápida revestidos com material magnético.

    - SSD (Solid State Drive): Um dispositivo de armazenamento de estado sólido que usa conjuntos de circuitos integrados para armazenar dados de forma persistente, normalmente usando memória flash e funcionando como armazenamento secundário na hierarquia de armazenamento do computador.

- Memória volátil: É a memória do computador que requer energia para manter as informações armazenadas; ele retém seu conteúdo enquanto está ligado, mas quando a energia é interrompida, os dados armazenados são rapidamente perdidos. (RAM)

    - RAM (Random Access Memory): é uma memória temporária computacional de acesso rápido; ou seja, é um local de armazenamento temporário de informações digitais usada pelo processador para armazenar informações temporariamente e que possui um acesso feito de forma aleatória mais rápido que ao HD, DVD, pendrive (permite a rápida leitura e escrita de informações), utilizada como memória primária em sistemas eletrônicos digitais.

- Processador: É a parte de um sistema computacional, que realiza as instruções de um programa de computador, que executar a aritmética básica, orientado por um padrão binário 0 e 1 que possibilita a entrada, o processamento e saída de dados.

    - CPU (Central Processing Unit): O papel da CPU pode ser comparado ao papel de um cérebro no funcionamento de um computador. Isto é, realiza operações lógicas, cálculos e processamento de dados.

    - Clock: Um sinal de clock ou sinal de relógio é um sinal lógico eletrônico que oscila entre um estado alto e baixo em uma frequência constante e é usado como um metrônomo para sincronizar ações de circuitos digitais.

#### 3.0 Como o computador executa vários programas?

- Lei de Moore: Em 1965, Gordon Moore previu que o número de componentes de um circuito integrado (transistores) dobraria a cada período de 18 meses, resultando num processador duas vezes mais rápido. Isso originou a chamada Lei de Moore. Essa lei virou uma medida econômica das empresas e é responsável pelo crescimento exponencial de performance da tecnologia que vemos nas últimas décadas.

- I/O (Input/Output): É um termo utilizado quase que exclusivamente no ramo da computação (ou informática), indicando entrada (inserção) de dados por meio de algum código ou programa, para algum outro programa ou hardware, bem como a sua saída (obtenção de dados) ou retorno de dados, como resultado de alguma operação de algum programa, consequentemente resultado de alguma entrada.

- Drivers de Dispositivo: A função de um driver de dispositivo ou controlador de dispositivo é aceitar requerimentos abstratos do software independente do dispositivo acima dele e cuidar para que a solicitação seja executada, permitindo que o software interaja com o dispositivo.

- GPU (Graphics Processing Unit): A placa de vídeo é a unidade responsável pela renderização dos pixels na tela do computador e está em todos os computadores pessoais.

#### 4.0 Como a memória funciona?

- Cache: É um dispositivo de acesso rápido, interno a um sistema, que serve de intermediário entre um operador de um processo e o dispositivo de armazenamento ao qual esse operador acede.

- Cache-Friendly: Algumas linguagens que oferecem um controle maior na alocação de memória, como C e C++, podem ter o tempo de execução de seus programas influenciados pela memória cache. Ou seja, só mudando a ordem de execução de alguns trechos de código, ele pode ficar bem rápido ou lento. Programas que conseguem otimizar ao máximo isso são chamados de cache-friendly ou bons para o cache.

- Hierarquia de memória: 

    Da mais rápida para a mais lenta (quanto mais lenta maior a capacidade de armazenamento):

    1ª - Registradores
    2ª - Cache L1
    3ª - Cache L2
    4ª - Cache L3
    5ª - RAM
    6ª - SSD
    7ª - HD
    8ª - Cloud

- Princípio da Localidade: 

    - Localidade temporal: Se um item é referenciado, ele tenderá a ser referenciado novamente.
    - Localidade espacial: Se um item é referenciado, itens cujos endereços são próximos a este, tenderão a ser referenciados também.


#### 5.0 Como os dados são armazenados?

- UTF-8: Essa codificação representa os caracteres em pedaços de 8 bits e sua grande vantagem é manter os textos codificados apenas em ASCII (a grande maioria da Web no passado) intactos. Ele tem um tamanho variável e cada caractere pode ocupar 8, 16, 24 ou 32 bits.

- UTF-16: Essa codificação representa os caracteres em pedaços de 16 bits. Isso significa que a codificação não é mais compatível com ASCII e ocupa o dobro de memória em textos que possuem apenas caracteres da língua inglesa. Ele tem um tamanho variável e cada caractere pode ocupar 16 ou 32 bits.

- UTF-32: Essa codificação representa os caracteres em pedaços de 32 bits. Ela não é compatível com ASCII e ocupa 4 vezes mais espaço em textos que só utilizavam ASCII. Mesmo assim, diferentemente do UTF-8 e UTF-16, essa codificação tem um tamanho fixo e essa é sua grande vantagem. Como cada caractere ocupa a mesma quantidade de bits, é fácil saber em qual posição cada caractere está em um texto (é só pegar o índice do caractere e multiplicar por 32).