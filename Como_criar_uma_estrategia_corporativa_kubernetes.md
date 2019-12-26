# Como criar uma estratégia corporativa Kubernetes
## Nos ambientes emergentes nativos da nuvem de hoje, o Kubernetes está em toda parte.

 As organizações adoram o Kubernetes porque ajuda a aumentar significativamente a agilidade e a eficiência de suas equipes de desenvolvimento de software, permitindo reduzir o tempo e os perigos associados à colocação de novo software em produção. As equipes de operações de tecnologia da informação adoram o Kubernetes porque ajudam a aumentar a produtividade, reduzir custos e riscos e aproximam as organizações da consecução de seus objetivos de nuvem híbrida.

 Simplificando, o Kubernetes facilita o gerenciamento da complexidade do software. À medida que os aplicativos corporativos se tornam mais complexos, as equipes de desenvolvimento e operações (DevOps) precisam de uma ferramenta que possa orquestrar essa complexidade. Eles precisam de uma maneira de iniciar todos os serviços dependentes desses aplicativos, garantindo que os aplicativos e serviços estejam íntegros e possam se conectar um ao outro.

 Os contêineres aumentaram drasticamente em popularidade porque fornecem uma maneira consistente de empacotar componentes de aplicativos e suas dependências em um único objeto que pode ser executado em qualquer ambiente. Ao empacotar o código e suas dependências em contêineres, uma equipe de desenvolvimento pode usar unidades de código padronizadas como blocos de construção consistentes. O contêiner será executado da mesma maneira em qualquer ambiente e pode iniciar e terminar rapidamente, permitindo que os aplicativos sejam dimensionados para qualquer tamanho.

 De fato, as equipes de desenvolvimento estão usando contêineres para empacotar aplicativos inteiros e movê-los para a nuvem sem a necessidade de fazer alterações no código. Além disso, os contêineres podem facilitar a criação de fluxos de trabalho para aplicativos executados entre ambientes locais e na nuvem, permitindo a operação suave de praticamente qualquer ambiente híbrido.

## Os perigos de muitas coisas boas

 O problema é que, à medida que mais contêineres são implantados nas organizações e na nuvem, as equipes de operações precisam de uma maneira de acompanhá-los. Caso contrário, rapidamente uma coisa boa pode se tornar uma situação ruim ou, pelo menos, incontrolável. É aí que a orquestração entra em cena.
 
 O Kubernetes é uma plataforma de orquestração de contêineres de código aberto, permitindo que um grande número de contêineres trabalhe juntos em harmonia e reduzindo os encargos operacionais. De fato, o Kubernetes, originalmente desenvolvido pelo Google e agora gerenciado pela Cloud Native Computing Foundation (CNCF), tornou-se um padrão para orquestração de contêineres na nuvem, fornecendo uma plataforma para automatizar a implantação, o dimensionamento e as operações dos contêineres de aplicativos em vários clusters de hosts.

 Existe até um ecossistema emergente crescendo em torno de Kubernetes à medida que se expande nas empresas. As equipes de DevOps podem aproveitar as ferramentas incríveis que estão surgindo do movimento do software de código aberto, como novos bancos de dados, ferramentas de big data, inteligência artificial, análise de dados, pesquisa e muitos outros.

 Nos últimos dois anos, o Kubernetes mudou do ambiente de desenvolvimento e teste para o ambiente de produção em muitas empresas. De acordo com a pesquisa global do CNCF de 2018 no mercado de gerenciamento de contêineres, 40% dos entrevistados estão executando o Kubernetes em produção. O CNCF recebeu respostas de 2.400 desenvolvedores e gerentes de operações de TI, além de funcionários de empresas (com mais de 5.000 funcionários) em todo o mundo, principalmente da América do Norte e Europa.

 Quanto às ferramentas de gerenciamento de contêineres, o Kubernetes continua sendo o líder, com 83% dos entrevistados, um aumento de 77% em pesquisas anteriores do CNCF. O Elastic Container Service (ECS) da Amazon ficou um segundo distante, com apenas 24% dos entrevistados dizendo que estava em uso. E Docker e Shell Scripts subiram atrás, com 21% e 20% respectivamente, de acordo com o CNCF.

 **Kubernetes não é um piscar de olhos - está aqui para ficar - e sua prevalência provavelmente se expandirá drasticamente à medida que a complexidade do software se desloca para mais e mais partes da empresa.**

## Compreendendo a adoção atual do Kubernetes da sua organização

 A construção de uma estratégia corporativa do Kubernetes começa com a compreensão de onde o Kubernetes está sendo executado em sua organização e a imaginação de como isso vai mudar na próxima década. Nos últimos dois anos, o acesso ao Kubernetes ficou dramaticamente mais fácil. As ferramentas de código aberto tornam o provisionamento e a atualização de um cluster Kubernetes de forma rápida e fácil, e os provedores de nuvem agora estão oferecendo o Kubernetes como um serviço hospedado. Qualquer equipe que use o Amazon Web Services, o Google Cloud Platform ou o Microsoft Azure pode provisionar um cluster Kubernetes em minutos.

**K8s Autogerenciado**
 * KubeADM
 * Kops
 * Kubespray  
 * Rancher RKE
 * Hand-built

**K8s Hospedado**
 * Google GKE
 * Amazon EKS
 * Digital Ocean
 * Azure AKS

 Atualmente, não é incomum as organizações abordarem o Kubernetes da mesma maneira que criaram o OpenStack ou outros serviços compartilhados e centralizados. As equipes podem usar o Kubernetes para criar grandes agrupamentos de infraestrutura e, em seguida, oferecer às equipes de desenvolvimento acesso compartilhado a esses agrupamentos por meio dos namespaces do Kubernetes. O uso de namespaces torna possível para um administrador de cluster segmentar recursos de cluster e definir cotas de uso e limites de recursos para fornecer uma experiência razoavelmente bem isolada para cada equipe que precisa acessar o Kubernetes.

 Outras organizações deixaram para departamentos individuais ou equipes de DevOps decidirem por si mesmos como e onde usar o Kubernetes. Nessas organizações, não é incomum ter dezenas de clusters implantados nas nuvens públicas e nos datacenters da empresa.

 Com o tempo, é possível desenvolver tensões entre equipes individuais que desejam executar o Kubernetes exatamente da maneira que precisam, e uma organização de TI que deseja manter a segurança e o controle sobre como o Kubernetes é implementado.

 **O incentivo para as equipes de desenvolvimento é a flexibilidade**: ter controle administrativo no nível do cluster permite que eles configurem o cluster para executar exatamente como eles precisam em termos de armazenamento, política de segurança ou em qual infraestrutura ele é executado. As equipes de TI estão especialmente nervosas com os clusters implantados e deixados sem patch e sem gerenciamento. Eles gostariam de centralizar as operações e políticas em torno de clusters e fornecer acesso às equipes que precisam.

 Se o Kubernetes e os contêineres se tornarem a plataforma principal para a execução de aplicativos em qualquer infraestrutura, os gerentes de TI devem colaborar com o DevOps para desenvolver um plano e uma estratégia para o Kubernetes que satisfaça as necessidades da organização de desenvolvimento e atenda às necessidades da própria TI.

 Ao documentar e entender onde o Kubernetes está sendo executado em sua organização, procure pessoas que demonstrem conhecimentos existentes sobre contêiner. À medida que você progride na construção de sua estratégia, o desenvolvimento de uma equipe de especialistas que pode ajudar na administração dos clusters do Kubernetes e na implantação de aplicativos no Kubernetes será fundamental para impulsionar a adoção.

## Onde você estará executando o Kubernetes em cinco anos?

 Construir uma estratégia Kubernetes em toda a organização significa priorizar seus objetivos para esta nova tecnologia. Se sua equipe usar o Kubernetes e contêineres como uma maneira de reduzir os custos de infraestrutura, você provavelmente se concentrará em criar grandes grupos e tentar obter o máximo de densidade possível deles. Se, em vez disso, sua equipe se concentrar no uso do Kubernetes para acelerar o desenvolvimento e as equipes de suporte procurarem entrega contínua em diferentes plataformas de computação, você adotará uma abordagem diferente, enfatizando a flexibilidade e fornecendo mais ferramentas ao Kubernetes, como monitoramento e integração de CI / CD.

 Para priorizar seus objetivos, tente entender o potencial do Kubernetes e imagine como sua empresa pode usá-lo em cinco anos. O Kubernetes é uma ótima maneira de executar aplicativos modernos, centrados em microsserviços. Ele oferece um rico conjunto de funcionalidades que permitem que as equipes determinem como os diferentes serviços dos aplicativos modernos são executados, manipulam eventos inesperados, conectam-se uns aos outros e outros aplicativos e APIs.

 Hoje, todos os principais provedores de nuvem tornaram fácil a implantação de clusters Kubernetes em questão de minutos. As equipes estão continuamente criando novos aplicativos, implantando-os em diferentes nuvens e usando o Kubernetes para executá-los. Entre os clusters usados para desenvolvimento, preparo e produção, e a necessidade de implantar clusters Kubernetes em diferentes data centers e provedores de nuvem, não é difícil imaginar uma empresa bem organizada executando dezenas de clusters Kubernetes.

 O interessante é que as mesmas arquiteturas de aplicativos modernas que consideramos nativas da nuvem estão começando a sair do data center. As equipes que constroem software para fábricas, hospitais e lojas agora desejam executar aplicativos com análises de dados avançadas e arquiteturas complexas o mais próximo possível de seus clientes e instalações de produção. Hoje, pensamos no Kubernetes como uma ferramenta para executar cargas de trabalho de datacenter e nuvem, mas dentro de alguns anos, provavelmente o usaremos para executar aplicativos em qualquer infraestrutura. Mesmo dispositivos monomodo, como terminais de ponto de venda, dispositivos médicos, equipamentos de comunicação ou carros, se beneficiarão da capacidade de implantar e executar aplicativos facilmente usando microsserviços. Poderíamos estar olhando para milhares de implantações de borda, todas executadas como clusters Kubernetes individuais e apresentando uma API que precisa ser gerenciada.

 Entre clusters executados em diferentes nuvens, data centers e edge, é quase certo que sua organização estará executando mais de um cluster Kubernetes. A menos que você saiba que estará executando um único aplicativo em um único local, provavelmente faz sentido para a maioria das equipes criar sua estratégia de Kubernetes com a expectativa de que eles precisam poder provisionar e gerenciar facilmente muitos clusters de Kubernetes em diferentes locais.

 Novas tecnologias como o Kubernetes são empolgantes para trabalhar e não é incomum para muitas equipes tentarem se apropriar da construção de uma estratégia de conteinerização e Kubernetes para sua empresa. Não é incomum que as equipes individuais de DevOps, grupos de serviços compartilhados, TI central, plataforma em nuvem ou grupos de plataforma como serviço sintam que devem ser responsáveis pela construção de uma estratégia em torno do Kubernetes.

## Quem deve ser o dono da estratégia Kubernetes?

 Como sempre, não há uma resposta correta para determinar a equipe que deve possuir sua estratégia. As equipes de sucesso geralmente reúnem talentos de toda a organização e colaboram para determinar os requisitos. Ainda assim, investir em uma estratégia e construir uma plataforma significa encontrar orçamento, por isso é definitivamente mais comum que uma equipe assuma a liderança na entrega da estratégia. Duas equipes que vemos frequentemente liderando a estratégia de contêineres são a equipe de serviços compartilhados responsável pelo suporte aos desenvolvedores e DevOps e a função central de TI responsável pelas plataformas de computação

 A equipe de serviços compartilhados traz informações importantes sobre como uma organização está modernizando sua abordagem para o desenvolvimento de aplicativos, e as equipes de requisitos identificaram o que precisam em uma plataforma Kubernetes. Eles geralmente entendem outros sistemas principais que foram criados para o DevOps, como ferramentas de CI / CD, ambientes de desenvolvimento, serviços de dados e ferramentas de monitoramento de aplicativos. Se essas equipes possuem a estratégia ou simplesmente contribuem para ela, elas representam pelo menos um dos principais consumidores de contêineres da organização e devem ser uma parte crítica do desenvolvimento da estratégia da organização.

 A equipe central de TI focada em computação em nuvem e outras plataformas de computação também é uma equipe lógica para liderar uma estratégia Kubernetes. Essas equipes têm um forte entendimento das operações da plataforma, infraestrutura, segurança, multilocação e investimentos existentes em TI, e geralmente possuem uma experiência significativa na execução de projetos críticos. Um projeto liderado pela equipe de plataformas de TI se beneficiará definitivamente da compreensão dos amplos requisitos de muitas equipes diferentes em uma organização grande e complexa. Ainda assim, os projetos que saem da área central de TI geralmente sofrem com muito pouco envolvimento com os usuários finais e muita influência dos fornecedores de tecnologia existentes. Essas equipes geralmente têm muito pouca experiência com as arquiteturas de aplicativos mais recentes e se beneficiam enormemente ao trabalhar em estreita colaboração com as equipes que lideram a inovação no desenvolvimento de aplicativos.

## Gerenciamento centralizado versus descentralizado de Kubernetes 

 Independentemente de quem conduz a estratégia, uma das principais perguntas que surgirão é sobre o quanto a padronização é possível sem afetar o benefício da inovação, que é um objetivo central da plataforma de TI. Muitas equipes terão projetos experientes em torno do OpenStack e da plataforma como serviço que tiveram dificuldade em obter adoção porque os usuários não conseguiram flexibilidade suficiente para implantar os aplicativos da próxima geração que estavam construindo. Com o Kubernetes, há flexibilidade suficiente na plataforma e no ecossistema para satisfazer qualquer equipe. Expor essa flexibilidade é fundamental para a entrega de valor. Qualquer estratégia que abstraia o Kubernetes provavelmente enfrentará resistência de suas equipes mais inovadoras. Ao mesmo tempo, a flexibilidade do Kubernetes e seu ecossistema pode ser um obstáculo para algumas equipes que procuram uma plataforma para executar apenas aplicativos padrão.

 Um dos desenvolvimentos mais emocionantes no espaço Kubernetes em 2019 é o surgimento de abstrações leves ou software MicroPaaS. Esses são projetos executados no Kubernetes, mas fornecem estruturas que simplificam o gerenciamento de aplicativos. Na Rancher, desenvolvemos um MicroPaaS chamado [Rio](https://rio.io/), que incorpora Kubernetes, Prometheus, Knative e Istio para oferecer uma experiência simples e integrada que ajuda as equipes a entrar rapidamente no Kubernetes e obter uma tonelada de valor. O [Google Run](https://cloud.google.com/run/) é outro exemplo dessa abordagem para executar contêineres que abstrai uma parte da complexidade do Kubernetes. Essas abordagens tiram lições do espaço sem servidor, permitindo que os contêineres sejam reduzidos a zero, por exemplo, e fornecem linguagens declarativas simples para criar, conectar, dimensionar e monitorar serviços. Para equipes que usam CI / CD e aplicativos sem estado, elas podem oferecer uma experiência poderosa sem exigir que as equipes desenvolvam um entendimento profundo de toda a tecnologia subjacente.

 Ao criar sua estratégia do Kubernetes, considere combinar o melhor de uma abordagem descentralizada com controles e gerenciamento suficientes para garantir a conformidade e remover tarefas repetitivas. Tente centralizar e automatizar tarefas comuns, como gerenciamento do ciclo de vida do cluster Kubernetes, políticas RBAC, gerenciamento de infraestrutura e outras operações do segundo dia. Ao mesmo tempo, deixe as equipes com muitas opções para obter acesso aos clusters do Kubernetes e se podem usar um cluster compartilhado ou dedicado. Você deve se concentrar principalmente em manter a visibilidade de todos os clusters provisionados, não necessariamente forçando as equipes a utilizar um conjunto de clusters pré-aprovados de uma maneira especificada.

## A conteinerização e o Kubernetes interromperão alguns de seus outros planos

 Se sua organização decidiu que a adoção expandida de Kubernetes e contêineres acelerará a inovação e é fundamental para sua estratégia de TI, é importante considerar como isso afetará outros projetos que já estão acontecendo. Abaixo, veremos alguns projetos comuns que podem ser impactados pelo Kubernetes. Esta não é de maneira alguma uma lista exaustiva. Lembre-se de considerar os projetos existentes da sua organização e como sua estratégia de contêiner pode aumentá-los ou impactá-los.

### **Nossa organização investe fortemente em computação em nuvem**

 Para organizações que estão focando em uma estratégia de TI “primeiro na nuvem”, a adoção do Kubernetes quase certamente fará parte de uma estratégia maior na nuvem. Todo grande provedor de nuvem oferece clusters Kubernetes hospedados e, geralmente, outros tipos de serviços orientados a contêineres, como registros, monitoramento, CI / CD e serviços de plataforma. Uma questão fundamental para essas organizações é se elas devem criar uma estratégia para o Kubernetes independente da estratégia de computação em nuvem. Se uma organização optou por se comprometer com um provedor de nuvem, é provável que eles adiem a estratégia de seu provedor de nuvem para contêineres. Por exemplo, se uma organização executa ou planeja executar a maioria de seus aplicativos críticos no Azure, faria muito sentido que eles tivessem uma familiaridade profunda com os diferentes serviços de conteinerização no Azure. Obviamente, eles podem achar que esses serviços não atendem às suas necessidades por algum motivo, mas mesmo se implementarem seus próprios Kubernetes no Azure, eles desejarão implementá-lo de uma maneira que tire proveito de outros serviços do Azure.

 Por outro lado, se uma organização decidiu se concentrar na multi-nuvem como uma iniciativa estratégica, é provável que eles vejam o Kubernetes como uma oportunidade para unificar como eles interagem com todos os seus provedores de nuvem. Existem duas teorias concorrentes sobre a melhor maneira de criar uma estratégia multi-cloud no Kubernetes:
 * A primeira sugere que você use os provedores de nuvem apenas para o provisionamento da infraestrutura principal e crie uma plataforma consistente com base no Kubernetes sobre essa infraestrutura. Com essa abordagem, as equipes desenvolveriam uma implementação consistente do Kubernetes e de qualquer de seus serviços dependentes e, então, construiriam uma plataforma comum sobre a infraestrutura de nuvem. Essa abordagem visa minimizar o aprisionamento na nuvem e obter ampla portabilidade de aplicativos.
 Essas equipes tentarão não utilizar nenhum dos serviços proprietários oferecidos por diferentes provedores de nuvem, em vez de optar por soluções de código aberto ou de várias nuvens. As grandes empresas de software de plataforma recomendam frequentemente essa abordagem, sugerindo que o uso de suas plataformas PaaS em diferentes nuvens pode aliviar o aprisionamento na nuvem.
 * A segunda abordagem sugere que as equipes padronizem as políticas e o gerenciamento em torno do Kubernetes, mas assumem que onde quer que eles executem o Kubernetes, seus desenvolvedores provavelmente desejarão utilizar outros serviços que possam ser exclusivos para esse ambiente de computação. Essa abordagem sugere que, se você estiver executando o Kubernetes na AWS, não hesite em usar outros serviços que possam ser exclusivos da AWS. Essas equipes se preocupam menos com o bloqueio e mais com a flexibilidade das equipes de aplicativos para usar os recursos nativos de diferentes plataformas. Com essa abordagem, o foco precisa estar no fornecimento de gerenciamento e ferramentas comuns em torno de diferentes implementações do Kubernetes.

### **Estamos investindo em infraestrutura hiperconvergente como parte de uma atualização do data center**

 Para equipes que estão desenvolvendo nova capacidade de datacenter usando infraestrutura hiperconvergente, o Kubernetes certamente será uma carga de trabalho nessas plataformas. A implantação e operação do Kubernetes em infraestrutura hiperconvergente não é mais complicada do que executá-lo em qualquer outro lugar. No entanto, você pode achar que o provedor de infraestrutura hiperconvergente oferece uma implementação do Kubernetes como parte de sua plataforma. Com esses serviços, integrá-los a uma estratégia Kubernetes maior pode oferecer valor adicional. Como alternativa, como a maioria das plataformas de infraestrutura hiperconvergente oferece APIs para provisionamento de hosts ou VMs, pode fazer sentido incorporar o plano de controle na camada de gerenciamento do Kubernetes, para permitir o dimensionamento automático da infraestrutura à medida que os tamanhos de cluster aumentam e diminuem. O armazenamento é outra área em que a integração com infraestrutura hiperconvergente pode agregar muito valor. Muitas dessas plataformas possuem drivers Kubernetes que simplificam a criação de volumes e podem fornecer valor adicional ao backup e recuperação de cargas de trabalho com estado em execução na plataforma Kubernetes.

### **Estamos tentando modernizar nossos aplicativos existentes para melhorar a segurança e a estabilidade**

 Uma empresa compartilhou que tinha mais de 5.000 aplicativos existentes pelos quais era responsável pela entrega e achou que a conteinerização e o Kubernetes poderiam ser uma boa solução para melhorar a maneira como eles gerenciam esses aplicativos. Se você estiver criando uma estratégia do Kubernetes, em algum momento, precisará decidir como sua estratégia se aplica às cargas de trabalho herdadas existentes. A maioria desses aplicativos é estável, com muitas dependências complexas e conexões codificadas com outros serviços. Eles não se parecem com os aplicativos nativos da nuvem para os quais o Kubernetes foi criado, e ainda é possível contê-los e executá-los em um cluster do Kubernetes. Uma opção recomendada é que as equipes adiem o mergulho profundo em aplicativos herdados até que eles já estejam usando o Kubernetes para novas cargas de trabalho.

 Quando sua familiaridade com o Kubernetes se expande e sua equipe é capaz de gerenciar vários clusters de produção executando aplicativos nativos da nuvem e sem estado, esse é um bom momento para começar a analisar a execução de aplicativos herdados em contêineres. Um artigo inteiro pode ser escrito sobre as práticas recomendadas para a migração de aplicativos herdados para o Kubernetes, mas o ponto principal é que quase sempre faz sentido executá-los em clusters dedicados com diferentes abordagens ao gerenciamento de infraestrutura. Esses aplicativos são arquitetados com uma expectativa de estabilidade e cenários de falha infrequentes. Você pode imitar isso no Kubernetes e ainda obter muitos outros benefícios que o Kubernetes oferece, como segurança, suporte dos mais recentes sistemas operacionais, automação e excelente monitoramento e visibilidade.

### **Precisamos reduzir nossos gastos com infraestrutura / nuvem**

 Se sua organização está tentando reduzir custos, o potencial de usar o Kubernetes para melhorar a densidade pode ser bastante atraente. Os clusters Kubernetes oferecem multilocação e não é razoável esperar que você possa obter mais retorno sobre seus gastos em infraestrutura usando contêineres e melhor agendamento de recursos.

 No entanto, tente não orientar muito o seu caso de negócios para contêiner em direção à economia de custos. A maioria das organizações levará anos para migrar uma parte significativa da área de cobertura de aplicativos existente para contêineres e Kubernetes.

 A maior parte desse tempo será gasta para descobrir a estratégia correta para cada aplicativo, especificamente se é para substituir, re-projetar ou apenas migrá-lo. O Kubernetes certamente pode ajudá-lo a obter uma excelente utilização da infraestrutura, mas isso levará tempo, e a estratégia que você está desenvolvendo agora tem mais probabilidade de impactar sua organização, permitindo uma inovação rápida do que cortando os gastos com infraestrutura.

## Preparando suas equipes para a adoção mais ampla de Kubernetes

 Uma parte crítica de qualquer estratégia do Kubernetes é determinar como você treinará suas equipes para aproveitar o Kubernetes. Como dissemos anteriormente, se você achar que sua organização já possui alguns funcionários com experiência em contêineres ou Kubernetes, considere como incorporá-los à sua iniciativa. Isso não significa necessariamente retirá-los do trabalho existente, mas talvez eles possam trabalhar como parte da equipe, definindo requisitos, avaliando ferramentas ou desenvolvendo políticas.

 Independentemente do nível de habilidades da sua equipe, você certamente terá membros da equipe que precisam ser treinados para usar o Kubernetes ou administrá-lo. Felizmente, não faltam provedores de treinamento e cursos on-line da Kubernetes. Os melhores são orientados em torno de duas certificações principais disponíveis no CNCF para Kubernetes. O programa [Certified Kubernetes Administrator (CKA)](https://www.cncf.io/certification/cka/) é focado em indivíduos que gerenciarão os clusters Kubernetes, e o [Certified Kubernetes Application Developer](https://www.cncf.io/certification/ckad/) ajuda as equipes a entender como criar e executar aplicativos no Kubernetes.

 Ao criar sua equipe principal de administradores e usuários do Kubernetes, considere definir uma meta para treinar e certificar o maior número possível de membros da sua equipe. Os testes são bastante rigorosos e garantirão que você construa um forte conhecimento interno sobre o uso de contêineres e Kubernetes. Depois de ter algum conhecimento inicial, convém esperar para fazer mais treinamentos até sair da fase de design de sua estratégia e começar a integrar mais equipes nas implementações específicas do Kubernetes que sua organização está adotando.

## Avaliando plataformas de gerenciamento de contêineres e entregando o Kubernetes como serviço

 








