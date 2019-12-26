# Um guia para Kubernetes com Rancher
-------------------------------------

# Discutindo Kubernetes com Rancher

## Introdução
 Parabéns por iniciar sua jornada com contêineres Linux! Sua equipe escolheu astutamente o desenvolvimento e implantação da estrutura que fornece portabilidade, agilidade e escalabilidade de aplicações. A instalação do Docker foi o início da sua jornada com contêiners. Agora, você está pronto para implantar sua aplicação baseada em contêiner em escala com o Kubernetes. Nesse ponto, você se depara com uma variedade desconcertante de fornecedores de software, cloud providers e projetos open source que prometem implantações Kubernetes bem-sucedidas e sem problemas. Como você decide para onde ir a partir daqui?
	
 Rancher irá ajudá-lo a percorrer esta confusão.

 Assim como o Docker é o melhor primeiro passo para desenvolver aplicações baseadas em contêiners, o Rancher Labs é seu parceiro lógico na implantação em escala.Embora você não precise da implantação em escala planetária hoje, você e sua equipe de DevOps podem ter certeza de que, quando vocês atingirem esse marco o Rancher tem a capacidade de lidar com os maiores clusters de todos os tipos de Kubernetes: do local ao híbrido e de uma única nuvem pública a implantações de diversas nuvens em provedores independentes.

 Mais importante, como seu parceiro nessa jornada, o Rancher Labs mantém-se fiel às raízes de código aberto dos contêineres. Nós não assinamos o modelo freemium de dual-class. O Rancher é verdadeiramente open source, com todos os recursos disponíveis para todos. Somente o Rancher fornece uma desistalação livre de resíduos, deixando sua infraestrutura Kubernetes existente em funcionamento sem fantasmas nas máquinas. Estaremos lá se você precisar, mas poderá desaparecer se você decidir que não. Se você mudar de idéia, um simples reinstalar nos leva de volta, apoiando-o perfeitamente como se nunca tivéssemos saído.

 Este artigo apresenta a filosofia e os recursos do Rancher e explica como ele faz parceria com milhares de usuários para fornecer a melhor experiência de gerenciamento de contêineres. Nele compartilhamos mais sobre a jornada sobre a implantação em larga escala de contêiners e os principais requisitos para o gerenciamento de vários clusters. No final, concluímos com etapas concretas sobre como começar a usar Kubernetes com Rancher.


## Quem é Rancher Labs
 A Rancher Labs foi fundada em 2014 para fornecer as ferramentas necessárias para tirar o máximo proveito e vantagem da tecnologia de contêineres. Nós acreditamos que o Kubernetes permitirá uma nova era da portabilidade de aplicações. Nosso principal produto, Rancher, é uma plataforma completa de gerenciamento de contêineres que fornece um fácil acesso para trabalhar com todos os tipos de instalações Kubernetes.

 Para garantir o sucesso do Kubernetes, o Rancher inclui um rico conjunto de recursos. Sabendo que você precisará deles mais cedo ou mais tarde, incorporamos em nossa plataforma os recursos mais solicitados por milhares de clientes. A incorporação desses recursos economiza tempo e dinheiro, evitando as centenas de horas necessárias para configurar, integrar, solucionar problemas e manter a multiplicidade de projetos open source necessários para fornecer funcionalidade comparável.

 Os recursos amigáveis da empresa do Rancher incluem um catálogo de aplicativos embutido, monitoramento e registro integrados e RBAC superior. A disponibilização desde o início permite um ótimo começo à medida que você dimensiona sua implantação.
 
 ![alt text](C:\Users\ferna\Desktop\Imagens_Traduções\image2.png)


## Parceria com Rancher na sua jornada Kubernetes
 Quando você e sua equipe negociam a rotação de seus primeiros contêineres do Docker, você percebe que a execução de cargas de trabalho em vários servidores não é a força do Docker. Em vez disso, o Kubernetes é a melhor ferramenta no gerenciamento de cluster de contêineres: executa os contêineres certos no momento certo, dimensiona-os para cima e para baixo de acordo com a carga, lida com falhas de hardware ou contêiner e gerencia a rede e o armazenamento.

 Escolher o Kubernetes para dimensionar seu aplicativo em contêiner é a decisão certa, mas a última coisa que você quer é que sua equipe perca tempo dissecando os ziguezagues das diferentes opções de hospedagem do Kubernetes.  Idealmente, você deseja encontrar um parceiro com experiência em todos os tipos de plataforma que possa orientá-lo. Isso permite que suas equipes de desenvolvimento e DevOps se concentrem em perguntas e tarefas mais pertinentes que criam valor.  Por exemplo, quais recursos devem estar neste sprint? Como eles devem arquitetar o software para agregar valor único? Qual tecnologia de banco de dados eles devem escolher para diferentes componentes de aplicativos?

 No que diz respeito aos tipos de plataforma, se você ainda não tomou uma decisão sobre onde executar o Kubernetes, há três opções iniciais com base nos requisitos de negócios:
	 A. Implante em um provedor Kubernetes hospedado, como Google Kubernetes Engine (GKE), Amazon Elastic Container Service para Kubernetes (EKS) ou Azure 		Kubernetes Service (AKS).
	 B. Instale, execute e gerencie o Kubernetes em uma plataforma IaaS, como Amazon EC2, Azure, Google Cloud ou DigitalOcean.
	 C. Instale, execute e gerencie o Kubernetes na infraestrutura que você possui, no bare metal ou em uma solução de nuvem privada como o VMware.

 As duas últimas opções requerem instalação e configuração do Kubernetes. Você pode ter visto Kelsey Hightower do Google explicar as etapas envolvidas em seu conhecido tutorial - __Kubernetes, the Hard Way__ . Nesse caso, você aprecia as dificuldades envolvidas. Embora existam scripts e ferramentas de automação como kops, kubo e kubespray, alguns são limitados no suporte a diferentes plataformas e nenhum fornece gerenciamento de cluster pós-instalação. O Rancher fornece uma instalação simplificada que minimiza a complexidade, fornecendo uma maneira consistente de instalar o Kubernetes em qualquer plataforma. Além disso, fornece gerenciamento de cluster em escala.

 Mesmo se você estiver usando uma solução que fornece um cluster Kubernetes pré-criado, há benefícios significativos no uso do Rancher. Ele se integra perfeitamente à infraestrutura de gerenciamento do GKE, EKS e AKS e oferece controle total dos recursos da nuvem. Em vez de ter que aprender três interfaces diferentes, o Rancher fornece uma visão comum e consistente de cada um desses serviços hospedados com um único painel de vidro para acessar e interagir com eles.


### Amplitude de suporte da plataforma Rancher
 Como seu parceiro candidato na implantação do Kubernetes, vamos analisar os recursos do Rancher em todos os principais tipos de hosts de contêineres.

**Servidores Bare Metal** :  O Rancher provisiona e instala o Kubernetes em racks de servidores bare metal e fornece uma infraestrutura de contêiner escalável sem a sobrecarga da virtualização.
			    
**vSphere/ESXi** :  O Rancher se integra perfeitamente à sua infraestrutura de VM, executando contêineres em cima de VMs, permitindo que você se beneficie de snapshots, DR e outros benefícios que você espera da sua infraestrutura de VM. Nesse ambiente, você pode executar cargas de trabalho de contêiner e não contêineres lado a lado.

**EC2, Azure, GCE, Digital Ocean** :  O Rancher fornece instâncias de computação, instala o Kubernetes nelas e gerencia o ciclo de vida completo de todos os recursos. Isso permite que você se beneficie de uma plataforma IaaS enquanto executa um cluster de contêiner gerenciado pelo Kubernetes.
		
**GKE, EKS, AKS** :  O Rancher fornece gerenciamento completo dos recursos da nuvem, incluindo a capacidade de aumentar e diminuir os recursos. No entanto, em vez de aprender interfaces diferentes cada vez que você alterna nuvens ou gerencia contas e acessa entre elas, o Rancher fornece uma visão comum e consistente de cada um desses hosts.Serviços. Centraliza o RBAC e mantém seus clusters seguros.

 Para aqueles que já implantaram o Kubernetes, os clusters existentes podem ser dobrados na estrutura de gerenciamento do Rancher. Por exemplo, se sua equipe de desenvolvimento possui um cluster em execução no GKE, você pode instalar o Rancher e importar o cluster GKE existente. Da mesma forma, mudar de um provedor para outro é tão fácil quanto criar um novo cluster no novo provedor com o Rancher e migrar cargas de trabalho do cluster existente. Como toda a configuração de recursos, como segurança, políticas etc., que existem no Rancher, esses recursos podem ser facilmente gerados em outro local e uma simples atualização de DNS conclui a migração do aplicativo.

 O Rancher também fornece o conjunto completo de ferramentas necessárias para gerenciar todos os aspectos do ciclo de vida do aplicativo na plataforma.
 Independentemente de qual tipo de cluster Kubernetes o Rancher gerencia, ele pode se vincular a componentes internos como o Microsofts Active Directory, fornecer monitoramento, visibilidade e solução de problemas em nível corporativo e integrar-se perfeitamente aos pipelines de CI / CD.

## Um futuro multi-cluster para aplicações em nuvem
 Até agora, nós apenas discutimos kubernetes clusters únicos. As empresas que adotaram o Kubernetes no início provavelmente ficarão presas ao gerenciamento de vários clusters, com um silo de cada vez. Essas empresas sem sorte descobrem que não podem migrar aplicativos facilmente em diferentes nuvens para aproveitar os custos mais baixos ou novos recursos. Além disso, se um de seus provedores de nuvem pública falhar ou uma zona de disponibilidade fica prejudicada, eles não podem instanciar facilmente seu aplicativo em contêiner na nuvem de outro provedor sem pular através de muitos aros.

 A maioria das equipes de DevOps concorda que os benefícios de uma verdadeira plataforma multi-nuvem e multi-cluster são bastante atraentes. Felizmente, o Rancher fornece gerenciamento Kubernetes de várias nuvens e vários clusters a partir de um único console, mantendo o mesmo ambiente de desenvolvimento e fluxo de trabalho para a equipe de desenvolvimento de aplicativos.  Além disso, como uma solução de nível empresarial, o Rancher fornece outros recursos: 
 * Agnosticismo: um verdadeiro sistema multi-cluster deve ser capaz de gerenciar qualquer plataforma baseada no Kubernetes nas nuvens privadas e públicas. O Rancher se integra a uma ampla variedade de plataformas e faz isso ao fornecer consistência de uma única interface front-end.
 * Suporte contínuo à nuvem híbrida: enquanto muitas equipes de desenvolvimento favorecem o uso da infraestrutura de nuvem pública para executar seus contêineres, empresas em setores regulamentados ou aqueles que enfrentam problemas de jurisdição de dados podem precisar depender de nuvens privadas. O Rancher suporta nuvens públicas, mas também se destaca na implantação nativa em um ambiente de nuvem privada, no bare metal ou em uma base de VM corporativa como o vSphere da VMware. Ele também suporta airgap, instalações e implantações de borda.
 * Políticas centralizadas: uma solução multi-cluster precisa permitir a configuração centralizada de políticas que podem ser empurradas e aplicadas em cada cluster do Kubernetes.  Por exemplo, uma política de rede específica que governa a conectividade entre serviços individuais em um aplicativo da web de três camadas, pode ser criada uma vez no Rancher e empurrada através do AKS, EKS e GKE sem precisar ser reconfigurada em cada silo do Kubernetes.
 *  RBAC centralizado e gerenciamento de identidade: a maioria das empresas possui identidade e funções armazenadas no Microsoft Active Directory (AD) e LDAP. Os kubernetes nativos não são particularmente fortes em seu apoio de identidade e papéis. No entanto, o Rancher pode integrar com anúncio, LDAP, SAML, OpenID e outros serviços e alavancar as mesmas identidades e papéis de empresas para permissão e controle de acesso em todos os clusters.
 * Visibilidade e solução de problemas centralizados: efetuando login em cada cluster Kubernetes para aprender o status dos pods e trabalhar com alertas silo por silo é ineficiente e provavelmente resultará em negligência da infraestrutura e problemas potenciais. Uma solução compatível com vários clusters como o Rancher pode unificar a visibilidade em todos os clusters e apresentá-los através de uma interface unificada.
 Esses recursos são fundamentais para o valor da Rancher para a empresa, mas os recursos do Rancher se estendem muito além disso.  Rancher também inclui catálogos de aplicativos públicos e privados com suporte ao Helm, bem como monitoramento integrado do Prometheus com alertas,  log de auditoria completo e envio de log para vários pontos de extremidade.


## Cenários onde o Rancher pode ajudar
 Para ajudar você a entender melhor o valor do Rancher, examinaremos alguns cenários que podem estar relacionados aos desafios existentes que você e sua equipe estão enfrentando:

### Cenário 1: Implantando o mesmo aplicativo em diferentes nuvens públicas:
 O Rancher pode ser usado para criar clusters Kubernetes em diferentes zonas de disponibilidade em um único provedor, por exemplo, AWS ou em diferentes nuvens, por exemplo, AWS e Azure. Por exemplo, EU General Data Protection Regulation (GDPR) os dados de clientes europeus podem precisar residir na EU, enquanto os dados do resto do mundo podem residir nos centros de dados dos EUA. Usando o Rancher, o mesmo aplicativo pode ser implantado em diferentes regiões como a EU e os EUA, usando as mesmas políticas  identidade e funções de acesso, garantindo consistência em todas instanciações. E quando o aplicativo é atualizado, o Rancher pode apenas fornecer com facilidade a nova versão em todas as regiões. Esse mesmo recurso também pode ser útil para recuperação de desastres, exibindo aplicativos em diferentes zonas de disponibilidade, se um desastre natural ou falha técnica derrubar o aplicativo nos locais originais.

### Cenário 2: Implantando partes diferentes de aplicativos em nuvens diferentes:
 Os desenvolvedores de aplicativos podem se encontrar dependentes de certos serviços que uma nuvem pública fornece, como o Serviço de Banco de Dados Relacional da AWS ou o Azure Cognitive Services for AI. Nessa situação, o Rancher pode executar facilmente uma parte de um aplicativo no AWS EC2 ou EKS, enquanto executa a outra parte, interagindo com a AI, no AKS do Azure. O Rancher pode conseguir isso mantendo os mesmos controles de diretiva e gerenciamento de acesso usando o Active Directory corporativo para bloquear o acesso. Da mesma forma, o Rancher pode monitorar a integridade do aplicativo nos dois clusters, fornecendo um único ponto de administração e manutenção nas duas nuvens públicas.

### Cenário 3: Implantando em uma nuvem privada:
 Se os dados corporativos precisarem residir em uma nuvem privada para conformidade, o Rancher poderá ser facilmente usado para implantar uma instância local do aplicativo. Para nuvens privadas, o Rancher pode implantar em um rack bare metal ou em um cluster vSphere. Assim como nos outros cenários, o Rancher pode fazer isso enquanto integra as informações de função e identidade presentes no Active Directory e fornece registro e monitoramento unificados. Se as regras de conformidade mudarem, e a empresa quiser migrar o aplicativo para uma nuvem pública para reduzir custos, o Rancher estará pronto para fazer isso com apenas alguns cliques do mouse.


## Començando sua jornada Kubernetes
 Para iniciar sua jornada para o sucesso, basta dar o primeiro passo correto. Esse primeiro passo é fácil: instale o Rancher no seu sistema. Depois de fazer isso, você achará o Rancher um ótimo parceiro. Independentemente de você seguir as implantações EKS, AKS ou GKE, montar novos clusters internamente em bare metal ou executar o Kubernetes em nós de computação em nuvem, o Rancher estará lá para apoiá-lo.

### Rancher: Solução de alcance livre sem bloqueio
 Diferente de outras soluções de gerenciamento de contêineres corporativos, o Rancher é puro código-fonte aberto e, o mais importante, não o prende à plataforma. O Rancher fornece um modelo de implantação de baixo custo, usando agentes para comunicação com clusters gerenciados e garantindo uma desinstalação sem resíduos. Se você decidir que o Rancher não é o melhor para você, desinstale-o e seu cluster Kubernetes existente continuará funcionando. Você poderá usar o painel do provedor ou emitir comandos diretos do kubectl sem nenhum rastro do Rancher. Quando você mudar de idéia e nos convidar para voltar, estaremos ao seu lado, trabalhando lado a lado com você para ajudar a gerenciar todos os seus clusters.

### Rancher: Código aberto sem compromisso
 O Rancher não se inscreve em um modelo freemium. Não enviamos uma versão básica para uso da comunidade e retemos uma versão corporativa para aqueles que pagam. É a mesma versão do Rancher, se você é um cliente pagante ou não. Estamos confiantes de que nosso produto fala por si e provará seu valor para você.
 Se você gostaria de apoio, fale conosco. Sustentamos nosso desenvolvimento por meio de contratos de suporte de nossos clientes. Envolva-nos para facilitar sua vida e apoiar o desenvolvimento contínuo da melhor solução para gerenciamento de contêineres.
 Para começar, concluiremos com sugestões para os recursos do Rancher, que podem fornecer respostas para as perguntas restantes e uma página de início rápido para começar. Realmente, não há restrições quanto à escolha de Rancher como seu companheiro nesta jornada; sem compromisso a longo prazo e custo zero. Então vamos começar!

# Recursos do Rancher para introdução:
 Começando: <https://rancher.com/quick-start/>
 
 Benefícios únicos do Rancher: <https://rancher.com/what-is-rancher/what-rancher-adds-to-kubernetes/

