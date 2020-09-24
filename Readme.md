# Becoming Devops - Jornada rumo à "Cloud Native Applications and Infrastructure"

![Devops](https://dpsvdv74uwwos.cloudfront.net/statics/img/product-pages/devops.png)




Assim como a maioria das jornadas, a nossa se iniciou a partir de uma necessidade.
Mas no nosso caso, a necessidade em questao nao era somente uma melhoria, reestruturacao, nem um novo produto ou algo similar, mas sim de uma transformaçao desruptiva.

Estamos falando de uma transformacao de negocio, que desencadeou, em diferentes ritimos, transformaçoes de tecnologia, processos e principalmente de pessoas. Guarde com carinho este ultimo item: PESSOAS, vamos falar também sobre isso mais adiante.

Neste artigo vamos focar na escolha das nossas novas ferramentas e o impacto das mesmas em nosso negocio, tecnologia e em nossos times.
Vamos falar muito de Cloud Native Computing Foundation (CNCF) e a importancia dela em nossas escolhas.

## Tecnologia e processos
Brincando com um TL;DR, ja vou direto pra conclusao em relacao a tecnologia e processos: 
- **Tenha um forte direcionamento de onde o seu negocio e a sua TI querem chegar.
Mas caso nao tenha, sem problemas, é uma excelente oportunidade de propor e ajudar a construir. O que nao vale é ficar parado ou só cobrando de alguem.**

Uma vez com estes nortes estabelecidos ( v1 de um roadmap de evolucao tecnologica), começa uma fase sensacional de construir o caminho para chegarmos nestes obtivos.
A noticia ruim é nao existe um GPS para te guiar em caminho certeiro, e a boa, é que a contrucao e experimentacao destes caminhos, é uma das experiencias mais enriquecedoras que podemos ter profissionalmente. E aqui na **Localiza Labs** aconteceu exatamente isso.

Para fazer isso acontecer, foi formada uma força tarefa composta por varios setores da TI, e juntamente com parceiros altamente capacitados, inicamos um processo de estudo e capacitacao sobre as novas tecnologias e arquiteturas de software e infraestrutura. 

Neste ponto da nossa jornada, tivemos a ajuda de quatro grandes "Guia 4 Rodas" (agora ja sabem que vivi intensamente anos 80 e 90 :-) ) para nos apoiar nas tomadas de decisoes: 
 - Os 12 Fatores (twelve factors) - [versao em ingles](https://12factor.net) e [versao em portugues](https://12factor.net/pt_br/)
 - [CNCF Cloud Native - Trail Map](https://github.com/cncf/landscape/blob/master/README.md#trail-map)
 - [CNCF Cloud Native - Landscape](https://landscape.cncf.io)
 - [SaFe - Devops Health Radar](https://www.scaledagile.com/devops/)
 
Se voce é de TI, de qualquer area ou cargo e nao conhece os 4 itens acima, vai por mim, investa e dedique uma horinha (60 minutos) do seu dia de HOJE para aprender sobre os mesmos.
Entenda principalmente o que sao, qual o seu proposito e como voce e seu time podem tirar proveito deles. #FicaADica.

Mas por que CNCF, e por que nos preocupamos tanto com isso?

Conforme muito bem descrito pelo blog [veronez.dev:](https://veronez.dev/2019/12/01/um-pouco-sobre-a-cloud-native-computing-foundation-cncf/)
*"A CNCF é uma fundação que faz parte da Linux Foundation e tem como objetivo promover o desenvolvimento de soluções de nuvem, sejam elas públicas, privadas ou híbridas. Dessa forma, a CNCF auxilia e sustenta um ecossistema de projetos de código aberto e sem vinculação a nenhum fornecedor, ou seja, soluções que podem ser implementadas em qualquer fornecedor de serviço de nuvem."*

Mais abaixo, voces vao entender como estes pontos estao sendo muito importantes para a Localiza.

De todos os produtos que utilizamos em nossa nova stack tecnologica, 92% estao dentro do CNCF Landscape. Este é um percentual muito importante, que traz beneficios diretos e indiretos para todas as equipes de TI.

Destes beneficios, é muito gratificante poder destacar alguns deles, visto aos desafios que superamos atraves dos mesmos:
 - Amplo acesso a informacao: documentacoes, videos, podcast, foruns, wikis, Repos Git, etc;
 - Grande interoperabilidade e compatbilidade entre os componentes;
 - Maior facilidade no processo de recrutamento de novos colaboradores, visto à atratividade das ferramentas pelo publico de TI e dissiminaçao das mesmas no mercado;
 - Grande liberdade de escolha de parceiros e ambientes de hospedagem;
 - Alto desacomplamento das aplicacao com a infraestrutura que suporta as mesmas;
 - Maior facilidade em adocao de software livre por uma empresa tao grande como a nossa;
 - Muita autonomia para as tribos e squads;

E por fim, como consequencia dos itens acima, dois ganho indiretos super valiosos: 
 - Uma enorme proteção para o negocio da Localiza, que hoje é Tecnologia;
 - Grande diferencial competitivo, trazendo um TTM (time to market) muito expressivo para empresa assim como grande disponibilidade e performance de nossas aplicacoes;

Segue abaixo os itens da nossa stack que fazem parte do CNCF:

| Item                              | Categoria CNCF - Landscape           | Para que usamos                                                   |
| :-------------------------------- | :----------------------------------- | :---------------------------------------------------------------- |
| Docker                            | Container Runtime                    | Criacao de uma unidade padronizada de software                    |
| Kubernetes                        | Scheduling & Orchestration           | Orquestracao de containers                                        |
| Kubespray                         | Certified Kubernetes - Installer     | Instalacao e parametrizacao inicial de um cluster                 |
| Helm 3                            | Application Definition & Image Build | Empacotamento e instalacao de aplicacoes no cluster kubernetes    |
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
| RabbitMQ                          | Streaming & Messaging                | Desacoplamento de aplicacoes atraves do uso de filas de mensagens |
| Kafka                             | Streaming & Messaging                | Streamming e transporte de dados                                  |
| Terraform                         | Automation & Configuration           | IaC e automaçao                                                   |
| Ansible                           | Automation & Configuration           | IaC e gestao de configuracao                                      |
| Kibana                            | Logging                              | Pesquisa de logs                                                  |
| Elasticsearch                     | Logging                              | Indexao e logs distribuidos                                       |
| FluentD                           | Logging                              | Extracao, enriquecimento ingestao de logs no Elasticsearch        |
| Grafana                           | Monitoring                           | Dashboards de Monitoramento para Prometheus                       |
| Zabbix                            | Monitoring                           | Monitoramento de servidres Linux                                  |
| Datadog                           | Monitoring                           | Monitoramento de Aplicacoes - APM                                 |


Aos poucos, vamos fazer novos artigos contando no detalhe como foi construcao de cada um deles, compartilhando experiencia e principalmente, código.

## Pessoas
Umas das etapas mais cativantes desta jornada tem sido a tranformacao das pessoas.

Muito do que está relacionado à DevOps ja virou cliche, como o proprio nome né? 
Algo que ouvimos que frequencia, e as vezes ate com deboche, é que DevOps nao é e nao deve ser associado somente com ferramentas, com automacao, com pipeline, e muito menos com cargo (que atire a primeira pedra quem nunca sofreu ou fez bulling com isso), e que na verdade trata-se de uma tal CULTURA.

E que p**** é essa de cultura magica que é entao a essencia do DevOps? 

Concordo um pouco com as pessoas que criticam e reforcam os pontos que nao sao DevOps, como os citados acima, pois somente com tecnologia e automacao, dificilmente iriámos conseguir romper o famoso ["Wall of Confusion"](https://sellegi.se/glossary/wall-of-confusion/) e nem fazer os sonhados ["10+ deploys Per Day](https://www.rundeck.com/blog/twl-10-deploys-per-day-hammond-allspaw). O fator humano neste processo é fundamental, e ter uma empresa que entenda, apoie e direcione neste ponto é mandatório.

![Wall of Conf - Muro da confusao](https://www.plutora.com/wp-content/uploads/2014/09/enterprise_devops_wall_of_confusion.jpg)

Estamos entendendo na prática, que ê muito dificil aprender através de cursos, meetup, youtube e podcast sobre o real papel e perfil das pessoas em um ambiente DevOps.
Ê quase impossivel entender e aprender isso sem VIVER esta experiencia, que inclusive vai ser diferente em todas as empresas.

Falo isso com confiança, pois trabalho a 10 anos na Localiza, e sempre respeitei e admirei muito o valor que a empresa dá para os clientes e colaboradores.
Passei por muitas mudancas e reestruturaçoes, mas nada se compara com essa atual transformacao, onde estou presenciando o quanto a empresa está invetindo esforcos e muito dinheiro no fator humano.

Criar uma cultura DevOps em uma startup com 50 funcionarios e 5 produtos pode ser muiiiito diferente do que criar em uma TI com 700 colaboradores, 60 squads e aproximadamente mil aplicacoes.
Ê preciso muita vontade, patrocinio em todas as esferas e parceiros altamente capacitados.

É claro que nem tudo sao flores.
Por mais exista um grande plano por tras, a mudanca, principalmente de mindset, tem que partir do proprio individuo. Nao tem como forçar a barra.
Pessoas nao possuem um arquivo .conf para alterarmos, reiniciar o serviço e uma nova forma de pensar e atuar entra em vigor. 
Também nao possuem um arquivo YAML declarativo onde podemos mudar alguns parametros, "rodar a pipe" e pronto. Eita, ia ser bom né :-)
Nesta jornada estamos aprendendo que o tempo de cada pessoa e os estimulos necessarios para cada uma delas sao muito distintos.

E é ai que a coisa fica legal.
Poder observar e participar do amadurecimento dos colaboradores tem sido uma experiencia que vou guardar pra sempre.
Analistas de todas as senioridades trabalhando de um forma muito similar, um grande compartilhamento de conhecimentos, senso de dono, forte trabalho em equipe, autonomia, lideres se reinventando a todo momento para melhor servir aos times e à empresa, o problema de um é o problema de todos, sao alguns exemplos disso que estou falando. 


# Conclusao e mensagem final
Fecho este artigo fazendo algumas provocacoes e convites para quem estiver lendo:
- Gostaria de trabalhar com DevOps raiz?
- Trabalha com TI e gostaria de ter apoio e exemplo para uma transformacao na sua carreira atuando com as mais diversas tecnologias de ponta?
- Quer automatizar até a geladeira da sua casa (aqui tem um pouco de exajeiro)?
- Quer atuar e se especializar em todos os cloud providers do mercado?
- Ja tem muita experiencia com o mundo DevOps e gostaria de atuar em projetos de grande escala?
- Gostaria de nunca ficar entediado por falta de desafios?

Se alguma resposta foi sim, nos procure, se canditade e participe dos nossos processos de seleçao.
Temos varias vagas em aberto e sera um prazer te-lo em nosso time Localiza Labs.












