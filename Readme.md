# Becoming Devops - Jornada rumo à "Cloud Native Applications and Infrastructure"

![Devops](https://dpsvdv74uwwos.cloudfront.net/statics/img/product-pages/devops.png)



Assim como a maioria das jornadas, a nossa se iniciou a partir de uma necessidade.
Mas no nosso caso, a necessidade em questão não era somente uma melhoria, reestruturação, nem um novo produto ou algo similar, mas sim de uma transformação desruptiva.

Estamos falando de uma transformação de negócio, que desencadeou, em diferentes ritmos, transformações de tecnologia, processos e principalmente de pessoas. Guarde com carinho este último item: PESSOAS, vamos falar também sobre isso mais adiante.

Neste artigo vamos focar na escolha das nossas novas ferramentas e o impacto das mesmas em nosso negócio, tecnologia e em nossos times.
Vamos falar muito de Cloud Native Computing Foundation (CNCF) e a importância dela em nossas escolhas.

## Tecnologia e processos
Brincando com um TL;DR, já vou direto pra conclusão em relação a tecnologia e processos: 
- **Tenha um forte direcionamento de onde o seu negócio e a sua TI querem chegar.
Mas caso não tenha, sem problemas, é uma excelente oportunidade de propor e ajudar a construir. O que não vale é ficar parado ou só cobrando de alguém.**

Uma vez com estes nortes estabelecidos ( v1 de um roadmap de evolução tecnológica), começa uma fase sensacional de construir o caminho para chegarmos nestes objetivos.
A notícia ruim é não existe um GPS para te guiar, e a boa, é que a construção e experimentação destes caminhos, é uma das experiências mais enriquecedoras que podemos ter profissionalmente. E aqui na **Localiza Labs** aconteceu exatamente isso.

Para fazer isso acontecer, foi formada uma força tarefa composta por vários setores da TI, e juntamente com parceiros altamente capacitados, iniciamos um processo de aprendizado sobre as novas tecnologias, arquiteturas de software e infraestrutura. 

Neste ponto da nossa jornada, tivemos a ajuda de quatro grandes "Guia 4 Rodas" (agora já sabem que vivi intensamente anos 80 e 90 :-) ) para nos apoiar nas tomadas de decisões: 
 - Os 12 Fatores (twelve factors) - [versão em inglês](https://12factor.net) e [versão em português](https://12factor.net/pt_br/)
 - [CNCF Cloud Native - Trail Map](https://github.com/cncf/landscape/blob/master/README.md#trail-map)
 - [CNCF Cloud Native - Landscape](https://landscape.cncf.io)
 - [SaFe - Devops Health Radar](https://www.scaledagile.com/devops/)
 
Se você é de TI, de qualquer área ou cargo e não conhece os 4 itens acima, vai por mim, invista e dedique uma horinha (60 minutos) do seu dia de HOJE para aprender sobre os mesmos.
Entenda principalmente o que são, qual o seu proposito e como você e seu time podem tirar proveito deles. #FicaADica.

Mas por que CNCF, e por que nos preocupamos tanto com isso?

O blog [veronez.dev](https://veronez.dev/2019/12/01/um-pouco-sobre-a-cloud-native-computing-foundation-cncf/) fez uma descrição muito legal sobre o tema:
*"A CNCF é uma fundação que faz parte da Linux Foundation e tem como objetivo promover o desenvolvimento de soluções de nuvem, sejam elas públicas, privadas ou híbridas. Dessa forma, a CNCF auxilia e sustenta um ecossistema de projetos de código aberto e sem vinculação a nenhum fornecedor, ou seja, soluções que podem ser implementadas em qualquer fornecedor de serviço de nuvem."*

Mais abaixo, vocês vão entender como estes pontos estão sendo muito importantes para a Localiza.

De todos os produtos que utilizamos em nossa nova stack tecnológica, 92% estão dentro do CNCF Landscape. Este é um percentual muito importante, que traz benefícios diretos e indiretos para todas as equipes de TI.

Visto aos desafios que superamos através destes beneficios, é muito gratificante poder destacar alguns deles:
 - Amplo acesso a informação: documentações, vídeos, podcast, fóruns, wikis, Repos Git, etc.;
 - Grande interoperabilidade e compatibilidade entre os componentes;
 - Maior facilidade no processo de recrutamento de novos colaboradores, visto à atratividade das ferramentas pelo publico de TI e disseminação das mesmas no mercado;
 - Grande liberdade de escolha de parceiros e ambientes de hospedagem;
 - Alto desacoplamento das aplicações com a infraestrutura que suporta as mesmas;
 - Maior facilidade em adoção de software livre por uma empresa tão grande como a nossa;
 - Muita autonomia para as tribos e squads;

E por fim, como consequência dos itens acima, dois ganhos indiretos super valiosos: 
 - Uma enorme proteção para o negócio da Localiza, que hoje é Tecnologia;
 - Grande diferencial competitivo, trazendo um TTM (time to market) muito expressivo para empresa assim como grande disponibilidade e performance de nossas aplicações;

Segue abaixo os itens da nossa stack que fazem parte do CNCF:

| Item                              | Categoria CNCF - Landscape           | Para que usamos                                                   |
| :-------------------------------- | :----------------------------------- | :---------------------------------------------------------------- |
| Docker                            | Container Runtime                    | Criação de uma unidade padronizada de software                    |
| Kubernetes                        | Scheduling & Orchestration           | Orquestração de containers                                        |
| Kubespray                         | Certified Kubernetes - Installer     | Instalação e parametrização inicial de um cluster                 |
| Helm 3                            | Application Definition & Image Build | Empacotamento e instalação de aplicações no cluster kubernetes    |
| Azure Devops - CI                 | Continuous Integration & Delivery    | Ferramenta de continuous integration                              |
| Azure Devops - CD                 | Continuous Integration & Delivery    | Ferramenta de continuous delivery                                 |
| Azure Container Registry          | Container Registry                   | Registry privado de imagens Docker                                |
| Prometheus                        | Monitoring                           | Monitoramento do cluster kubernetes e seus recursos               |
| Service Proxy NGINX (k8s Ingress) | Service Proxy                        | Ingress do cluster kubernetes                                     |
| Redis                             | Database                             | Cache Distribuído                                                 |
| Caligo                            | Cloud Native Network                 | CNI para cluster kubernetes                                       |
| Flanel                            | Cloud Native Network                 | CNI para cluster kubernetes - workers windows com .NET Framework  |
| Jaegger                           | Tracing                              | Ferramenta para Tracing de requisicoes                            |
| Rundeck                           | Automation                           | Automacao de scripts de Operations as a Service                   |
| RabbitMQ                          | Streaming & Messaging                | Desacoplamento de aplicações através do uso de filas de mensagens |
| Kafka                             | Streaming & Messaging                | Streaming e transporte de dados                                   |
| Terraform                         | Automation & Configuration           | IaC e automação                                                   |
| Ansible                           | Automation & Configuration           | IaC e gestão de configuração                                      |
| Kibana                            | Logging                              | Pesquisa de logs                                                  |
| Elasticsearch                     | Logging                              | indexação e logs distribuídos                                     |
| FluentD                           | Logging                              | Extração, enriquecimento ingestão de logs no Elasticsearch        |
| Grafana                           | Monitoring                           | Dashboards de Monitoramento para Prometheus                       |
| Zabbix                            | Monitoring                           | Monitoramento de servidores Linux                                 |
| Datadog                           | Monitoring                           | Monitoramento de Aplicações - APM                                 |
| Velero                            | Cloud Native Storage                 | Backup e restore cluster kubernetes                               |


Aos poucos, vamos fazer novos artigos contando no detalhe como foi construção de cada um deles, compartilhando experiência e principalmente, código.

## Pessoas
Umas das etapas mais cativantes desta jornada tem sido a transformação das pessoas.

Muito do que está relacionado à DevOps já virou clichê, como o próprio nome né? 
Algo que ouvimos com frequência, e as vezes ate com deboche, é que DevOps não é e não deve ser associado somente com ferramentas, com automação, com pipeline, e muito menos com cargo (que atire a primeira pedra quem nunca sofreu ou fez bulling com isso), e que na verdade trata-se de uma tal CULTURA.

Mas o que seria essa tal cultura DevOps ? Onde compra ? Tem DOC ? Fica em algum repo ?

Concordo um pouco com as pessoas que sempre nos lembram, e reforçam, os pontos que não são DevOps, como os citados acima, pois somente com tecnologia e automação, dificilmente iriámos conseguir romper o famoso ["Wall of Confusion"](https://sellegi.se/glossary/wall-of-confusion/) e nem fazer os sonhados ["10+ deploys Per Day](https://www.rundeck.com/blog/twl-10-deploys-per-day-hammond-allspaw). O fator humano neste processo é fundamental, e ter uma empresa que entenda, apoie e direcione neste ponto é mandatório.

![Wall of Conf - Muro da confusao](https://www.plutora.com/wp-content/uploads/2014/09/enterprise_devops_wall_of_confusion.jpg)

Estamos entendendo na prática, que ê muito difícil aprender através de cursos, meetup, youtube e podcast sobre o real papel e perfil das pessoas em um ambiente DevOps.
Ê quase impossível entender e aprender isso sem VIVER esta experiência, que inclusive vai ser diferente em todas as empresas.

Falo isso com confiança, pois trabalho a 10 anos na Localiza, e sempre respeitei e admirei muito o valor que a empresa dá para os clientes e colaboradores.
Passei por muitas mudanças e reestruturações, mas nada se compara com essa atual transformação, onde estou presenciando o quanto a empresa está investindo esforços e muito dinheiro no fator humano.

Criar uma cultura DevOps em uma startup com 50 funcionários e 5 produtos pode ser muiiiito diferente do que criar em uma TI com 700 colaboradores, 60 squads e aproximadamente mil aplicações.
Ê preciso muita vontade, patrocínio em todas as esferas e parceiros altamente capacitados.

É claro que nem tudo são flores.
Por mais que exista um grande plano por trás, a mudança, principalmente de mindset, tem que partir do próprio individuo. Não tem como forçar a barra.
Pessoas não possuem um arquivo .conf para alterarmos, reiniciar o serviço e uma nova forma de pensar e atuar entra em vigor. 
Também não possuem um arquivo YAML declarativo onde podemos mudar alguns parâmetros, "rodar a pipe" e pronto. Eita, ia ser bom né :-)
Nesta jornada estamos aprendendo que o tempo de cada pessoa e os estímulos necessários para cada uma delas são muito distintos.

E é aí que a coisa fica legal.
Poder observar e participar do amadurecimento dos colaboradores tem sido uma experiência que vou guardar pra sempre.
Analistas de todas as áreas e todas as senioridades trabalhando juntos  e com um único proposito, um grande compartilhamento de conhecimentos, senso de dono, forte trabalho em equipe, autonomia, lideres se reinventando a todo momento para melhor servir aos times e à empresa, o problema de um é o problema de todos, são alguns exemplos disso que estou falando. 


# Mensagem final
Fecho este artigo fazendo algumas provocações e convites para quem estiver lendo:
- Gostaria de trabalhar com DevOps raiz?
- Trabalha com TI e gostaria de ter apoio e exemplo para uma transformação na sua carreira atuando com as mais diversas tecnologias de ponta?
- Quer automatizar até a geladeira da sua casa (aqui tem um pouco de exagero)?
- Quer atuar e se especializar em todos os cloud providers do mercado?
- Já tem muita experiência com o mundo DevOps e gostaria de atuar em projetos de grande escala?
- Gostaria de nunca ficar entediado por falta de desafios?

Se alguma resposta foi sim, nos procure, se candidate e participe dos nossos processos de seleção.
Temos várias vagas em aberto e será um prazer tê-lo em nosso time Localiza Labs.