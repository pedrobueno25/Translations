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


 












