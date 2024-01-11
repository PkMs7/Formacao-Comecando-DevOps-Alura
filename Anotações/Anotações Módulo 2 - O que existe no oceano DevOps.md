# Tópicos sobre Começando em DevOps

## Conteúdo de artigos e Alura+

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

### SRE (Site Reliability Engineering) - Engenharia de Confiabilidade de Sites

- O embate entre Desenvolvedores e Infra acontecem no ponto de **"Confiabilidade"**. (Como você pode assegurar que seu software é confiável?)

- Nesse cenário nasce o SRE, pra que se consiga deixar esse deploy mais confiável e seguro. (Foi desenvolvida essa disciplina pelo Google)

- Ajuda a obter métricas para trazer informações de confiabilidade. Seu ponto forte é a **Observabilidade**.

- Quatro sinais de ouro do SRE: Latência, Tráfego, Erros e Saturação.

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

### 4 Golden Signals

- Latência, Tráfego, Erros e Saturação. Esses sinais podem ser observados através do Grafana.

### Monitoramento com Netdata

    - Netdata é uma ferramenta de monitoramento (entendimento de como nossa aplicação e ambiente estão se comportando). É uma ferramenta open source.

    - Requisitos (Máquina Linux)

    - Comandos de instalação na documentação do site Netdata. [Clique Aqui](https://www.netdata.cloud)

    - SLA: Métricas de contrato

    - O Netdata já possui nativamente sistemas de alarmes em situações configuradas.

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
