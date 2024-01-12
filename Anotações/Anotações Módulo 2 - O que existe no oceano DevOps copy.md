# Tópicos sobre Começando em DevOps

## Conteúdo de artigos e Alura+

### Shift Left

- Shift Left é uma prática que consiste em deslocar para a esquerda as atividades testes, segurança e deploy, que normalmente estão mais à direita no processo, para que assim desde o ínicio de cada ciclo elas possam ser discutidas e planejadas, evitando problemas e acelerando a entrega de software.

### Cloud: o que é, História e Guia da computação em nuvem
[Artigo](https://encurtador.com.br/awPX6)

### Git Flow versus Trunk-based development

- Git Flow: É um modelo alternativo de ramificação do Git que consiste no uso de ramificações de recursos e várias ramificações primárias.

    - Com o Git Flow, é fácil para os desenvolvedores trabalharem em suas próprias funcionalidades em seu próprio ritmo, pois cada funcionalidade tem sua própria branch.

- Trunk-based: É uma estratégia que tenta minimizar a complexidade de lidar com múltiplos branches. Nesta abordagem, todos os desenvolvedores trabalham em uma única branch – o tronco (trunk/master/main).

    - Trunk Based Development incentiva uma cultura de entrega contínua, onde o código é integrado e testado frequentemente. Isso pode resultar em um ritmo de desenvolvimento mais rápido, mas também requer uma disciplina rigorosa de testes e integração.

### O que é Infraestrutura como Código(IaC)?

- Infraestrutura como Código(IaC): é um processo de gerenciamento de infraestrutura de TI que aplica as práticas recomendadas do desenvolvimento de software DevOps ao gerenciamento de recursos de infraestrutura de nuvem.


### DevSecOps

- DevSecOps é a camada de segurança do DevOps.

    ![DevSecOps](/Anexos/img/devSecOps.png)

- Segurança a qualquer custo, mesmo que diminua a velocidade. Abaixo os pilares do DevSecOps:

    - Segurança em primeiro lugar
    - Automação é fundamental
    - Velocidade
    - Entrega rápida e contínua (CI/CD)
    - Confiabilidade

- Em resumo, a camada de segurança, na prática entra diretamente na pipeline, com checks (auditorias e scanners de vírus) de arquivos maliciosos antes de subir a aplicação, por exemplo.

### Observabilidade

- Monitoramento de sistemas distribuídos (problema).

- Desafio: Agir proativamente ou reativamente em métricas e logs distribuídos.

- Pilares da Observabilidade:

    - Métricas
    - Traços Distribuídos
    - Logs

- Uma ferramenta para exportar algumas métricas é o **Prometheus** (base de dados para métricas).

- A ferramenta para visualizar essas métricas é o **Grafana** (importa a base de dados do Prometheus).

- Uma ferramenta para trabalhar com Instrumentação Manual é a Jaeger. Podem ser plugadas na ferramenta:

    - Service Mesh (Istio)
    - Proxy (Envoy, Traefik, Kong)

- Para trabalhar com logs pode-se usar: Sidecar, Logging agent instalado no host, Shell script. Uma ferramenta para ser utilizada é o Graylog.

### O que são Feature Flags ou Feature Toggles?
[Artigo](https://encurtador.com.br/BNS37)

### O que são Containers?

    - Antes do container se utilizava a infraestrutura On-premise. [Link](https://en.wikipedia.org/wiki/On-premises_software)

    - Em uma linha do tempo, a evolução dessa infraestrutura é a criação da Máquina Virtual (Servidor com N Sistemas Operacionais).

    - Após a criação das Máquinas Virtuais foram criadas os Containers.

    Diferença entre Container e Máquina Virtual

    ![Imagem](/Anexos/img/ContainerxVM.png)

### O que é Seerverless?

    - Serverless é um modelo de desenvolvimento nativo em nuvem para criação e execução de aplicações sem o gerenciamento de servidores.

    - É um paradigma de execução de código focado na não preocupação com servidores.
    
    - Alguns provedores desse serviço são: Amazon webserver, Microsoft Azure, Google Cloud.

    - Componentes Serverless: Lambda, API Gateway, SQS, DynamoDB, SNS, S3.


### SRE (Site Reliability Engineering) - Engenharia de Confiabilidade de Sites

- O embate entre Desenvolvedores e Infra acontecem no ponto de **"Confiabilidade"**. (Como você pode assegurar que seu software é confiável?)

- Nesse cenário nasce o SRE, pra que se consiga deixar esse deploy mais confiável e seguro. (Foi desenvolvida essa disciplina pelo Google)

- Ajuda a obter métricas para trazer informações de confiabilidade. Seu ponto forte é a **Observabilidade**.

- Quatro sinais de ouro do SRE: Latência, Tráfego, Erros e Saturação.