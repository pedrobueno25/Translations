# Rancher 2.3: Arquitetura Técnica
# Background
> De acordo com a 451 Research, 76% das empresas padronizarão o Kubernetes nos próximos 3 anos, pois promete um conjunto consistente de recursos em qualquer infraestrutura - do datacenter à nuvem e até edge - “Kubernetes and Beyond – Effective Implementation of Cloud Native Software in the Enterprise” por Jay Lyman, Analista Principa 451 Research.

 Ao unificar suas operações de TI com o Kubernetes, as empresas obtêm benefícios importantes, como maior confiabilidade, segurança aprimorada e maior eficiência com automação padronizada. No entanto, depender apenas do Kubernetes upstream geralmente não é suficiente para as equipes implantarem na produção. Falta visibilidade central, aplicação consistente de políticas e sistemas complexos de gerenciamento. Esses recursos são possíveis apenas em uma plataforma de gerenciamento Kubernetes como o Rancher. O Rancher foi construído desde o início para oferecer:

 * **Operações consistentes de cluster**: Atualizações, backups e implantações simplificados do Kubernetes.
 * **Política de segurança e gerenciamento de usuários**: Gerenciamento consistente de RBAC, PSP e usuário.
 * **Ferramentas e serviços compartilhados**: Acesso imediato a ferramentas e serviços.

# Rancher 2.3: Construído em Kubernetes
 * O Rancher 2.3 é uma plataforma completa de gerenciamento de contêineres construída no Kubernetes.
 * O Rancher 2.3 contém três componentes principais - uma **distribuição Kubernetes certificada**, uma **plataforma de gerenciamento Kubernetes** e **gerenciamento de aplicativos**
 
 ![Image 1](/images/image6.png)

## Certificados Kubernetes com Rancher Kubernetes Engine (RKE)
 O RKE é um instalador Kubernetes extremamente simples e extremamente rápido que funciona em qualquer lugar. O RKE é particularmente útil para levantar clusters Kubernetes em clusters VMware, servidores bare metal e instâncias de VM em nuvens que ainda não oferecem suporte ao serviço Kubernetes. Além disso, muitas pessoas usam o RKE em provedores de nuvem que já oferecem suporte aos serviços Kubernetes, para que tenham uma implementação consistente do Kubernetes em todos os lugares. No Rancher 2.3, os clusters podem ser provisionados nas arquiteturas Linux x86_64 e Arm64, bem como nos sistemas Windows 19.03.

 O RKE no Rancher gerencia o ciclo de vida completo dos clusters Kubernetes desde a instalação inicial até a manutenção contínua. Os usuários do Rancher podem:
 * Automatize o provisionamento de instância de VM em muitas nuvens usando drivers de máquina.
 * Instale o control plane do Kubernetes e os nós do banco de dados etcd.
 * Nós worker provisionados nos nós Windows e Linux Arm64 e x86_64.
 * Adicionar ou remover nós nos clusters Kubernetes existentes.
 * Atualize os clusters do Kubernetes para novas versões.
 * Monitore a integridade dos clusters Kubernetes.

## Operações consistentes de cluster
 Com o Rancher 2.3, você pode optar por gerenciar seus próprios clusters Kubernetes existentes provisionados por ferramentas existentes ou usar clusters Kubernetes gerenciados por uma nuvem. Os serviços Kubernetes, como EKS, GKE e AKS, podem ser facilmente provisionados ou importados para a provisão de instalação do Rancher e operar clusters RKE Kubernetes em qualquer infraestrutura de nuvem, virtualizada ou bare metal.

 O Rancher pode ser facilmente gerenciado com Infraestrutura como código com o provedor Terraform 2.0 do Rancher. Com isso, você pode armazenar facilmente suas configurações para clusters, namespaces, segredos e aplicativos de catálogo no Git. O Rancher possui uma API poderosa com a qual você pode fazer scripts para executar tarefas de rotina.

## Política de segurança e gerenciamento de usuários
 O gerenciamento unificado de cluster começa com autenticação centralizada. O Rancher 2.3 fornece um proxy de autenticação para todos os clusters do Kubernetes sob gerenciamento. Esse é um recurso crucial para a TI corporativa adotar serviços Kubernetes na nuvem, como o GKE.
 
 O GKE normalmente exige que seus usuários se autentiquem usando suas credenciais do Google. Com o Rancher 2.3, um desenvolvedor corporativo pode entrar em um cluster GKE usando as credenciais do Active Directory gerenciadas pela TI corporativa.
 
  ![Image 2](/images/image7.png)
 
 O Rancher 2.3 se baseia na autenticação centralizada com políticas de controle de acesso centralizadas definidas em nível global e aplicadas aos clusters sob gerenciamento. Aproveitando os recursos nativos de RBAC do Kubernetes, o Rancher 2.3 permite que os administradores de TI configurem e apliquem políticas de controle de acesso e segurança em vários clusters do Kubernetes.

 O Rancher 2.3 apresenta um novo conceito chamado Projetos. Um projeto é um ou mais namespaces do Kubernetes e suas políticas associadas, como regras RBAC, cota de recursos etc. Os usuários podem criar projetos e atribuir outros usuários ou grupos aos projetos que ele possui. Os usuários podem receber diferentes funções em vários projetos. Por exemplo, um desenvolvedor pode receber privilégios completos de criação / leitura / atualização / exclusão em um projeto dev, mas apenas acesso somente leitura nos projetos de preparação e produção. Os usuários podem apenas criar, modificar ou excluir espaços para nome nos projetos dos quais são membros. Isso aprimora muito a funcionalidade de autoatendimento multitenant do Kubernetes.

 Em uma versão futura, o Rancher fornecerá visibilidade da capacidade e do custo dos recursos subjacentes consumidos pelos clusters do Kubernetes.

## Gerenciamento de carga de trabalho de aplicativo

 A interface do usuário do Rancher 2.3 não tenta ocultar os conceitos subjacentes do Kubernetes e apresenta uma estrutura de implantação de aplicativos diferente do Kubernetes. O Rancher fornece uma interface de usuário fácil de usar para recursos nativos do Kubernetes, como pods e implantações.

 A experiência do catálogo de aplicativos no Rancher 1.0 foi adaptada para suportar gráficos Helm. Helm é um poderoso mecanismo de modelagem para implantar aplicativos no Kubernetes. Mas os usuários ainda precisam ler a documentação extensa para entender exatamente quais variáveis definir e os valores certos para essas variáveis. Este é um processo propenso a erros. O Rancher simplifica a implantação do gráfico Helm, expondo apenas o conjunto certo de variáveis e orientando o usuário ao longo do processo. O catálogo do Rancher orienta o usuário, fazendo as perguntas certas e apresentando padrões sensíveis e valores de múltipla escolha.

 O Rancher 2.3 funciona com qualquer sistema de CI / CD que se integre ao Kubernetes. Por exemplo, Jenkins, Drone e GitLab continuarão trabalhando com o Rancher 2.3, como fizeram com o Rancher 1.0.  O Rancher 2.3 também inclui um serviço de CI / CD gerenciado, construído no Jenkins. O serviço de CI / CD do Rancher 2.3 se integra perfeitamente à interface do usuário do Rancher.

 O Rancher 2.3 trabalha com qualquer sistema de monitoramento e registro que se integre ao Kubernetes. Para uma experiência imediata, os usuários podem usar a funcionalidade Prometheus incorporada. Se sistemas existentes como DataDog, Sysdig ou ELK estiverem em vigor, eles continuarão a trabalhar com o Rancher 2.3. Para agregação de logs, o Rancher possui um serviço Fluentd integrado que enviará logs dos hosts.

## Arquitetura de alto nível
 O software Rancher 2.3 consiste em duas partes. Os componentes do servidor Rancher gerenciam toda a implantação do Rancher. O Rancher também implanta componentes do agente nos clusters e nós do Kubernetes.
 
  ![Image 3](/images/image7.png)

# Componentes do servidor Rancher
 Nesta seção, descrevemos as funcionalidades de cada componente do servidor Rancher.

## Rancher API Server
 O servidor da API do Rancher é construído sobre um servidor da API do Kubernetes incorporado e um banco de dados etcd. Todos os recursos específicos do Rancher que estão sendo criados usando a API do Rancher são traduzidos para objetos CRD (Custom Resource Definition), com seu ciclo de vida sendo gerenciado por um ou vários controladores do Rancher.

 O Rancher API Server é a camada fundamental para todos os controladores no servidor Rancher. Inclui as seguintes funcionalidades:
 * Geração de esquema de API voltada para o usuário com capacidade de conectar formatadores e validadores personalizados.
 * Geração de interfaces do controlador para CRDs e tipos de objetos nativos do Kubernetes.
 * Estrutura de gerenciamento do ciclo de vida do objeto.
 * Estrutura de gerenciamento de condições.
 * Implementação genérica simplificada do controlador, encapsulando a lógica TaskQueue e SharedInformer em uma única interface.

## Controladores de gerenciamento
 Os controladores de gerenciamento executam as atividades que acontecem no nível do servidor Rancher, não específicas para um cluster individual. As atividades incluem: * Configurando políticas de controle de acesso para clusters e projetos.
 * Gerenciando modelos de política de segurança de pod.
 * Provisionar clusters chamando os drivers de máquina do Docker necessários e chamando os mecanismos Kubernetes como RKE e GKE.
 * Gerenciando usuários - operações CRUD nos usuários.
 * Gerenciamento de catálogo em nível global, busca de conteúdo do repositório Helm upstream, etc.
 * Gerenciando catálogos de cluster e em nível de projeto.
 * Agregando e exibindo estatísticas e eventos de cluster.
 * Gerenciamento de drivers, modelos e conjuntos de nós.
 * Gerenciando a limpeza de cluster quando o cluster é removido do Rancher.

## Controladores de Cluster de Usuário
 Os controladores de cluster de usuários realizam atividades específicas para um cluster. Os controladores de cluster de usuários estão espalhados pelos pods de servidor Rancher em execução para dimensionamento horizontal. As atividades incluem:
 * Gerenciando cargas de trabalho, que inclui, por exemplo, criação de pods e implantações em cada cluster.
 * Aplicar funções e ligações definidas em políticas globais em cada cluster.
 * Propagando informações do cluster para o servidor do Rancher: eventos, estatísticas, informações do nó e integridade.
 * Gerenciando diretivas de rede.
 * Gerenciamento de alertas, monitoramento, agregação de logs e pipelines de CI / CD.
 * Gerenciando cota de recursos.
 * Propagando segredos do servidor Rancher para clusters individuais.
 Os controladores de cluster de usuário se conectam diretamente aos servidores de API nos clusters GKE, mas passam pelo agente de cluster para conectar-se aos servidores de API nos clusters RKE.

## Proxy de autenticação
 O proxy de autenticação se integra aos serviços de autenticação como autenticação local, Active Directory e GitHub. Em todas as chamadas da API do Kubernetes, o proxy de autenticação autentica o chamador e define os cabeçalhos de representação do Kubernetes adequados antes de encaminhar a chamada para os masters do Kubernetes. O Rancher se comunica com os clusters Kubernetes usando uma conta de serviço.
 
 O proxy de autenticação se conecta diretamente aos servidores API nos clusters GKE, mas faz um túnel através do agente de cluster para conectar-se aos servidores API nos clusters RKE.

 No Rancher 2.2, o ponto de extremidade do cluster de autenticação foi introduzido nos clusters baseados em RKE para trazer autenticação centralizada ao cluster local. Isso fornece maior disponibilidade removendo o servidor de gerenciamento Rancher 2.3 do caminho de autenticação. Permitindo gerenciamento e operações desconectados dos seus clusters Kubernetes.

# Componentes do agente do Rancher
 Nesta seção, descrevemos os componentes de software implantados nos clusters Kubernetes gerenciados pelo Rancher.

## Agentes de cluster
O Rancher implanta um agente de cluster para cada cluster Kubernetes sob gerenciamento. O agente de cluster abre um túnel WebSocket de volta ao servidor Rancher para que os controladores de cluster do usuário e o proxy de autenticação possam se comunicar com o servidor da API Kubernetes do cluster de usuários. Observe que apenas os clusters RKE e os importados utilizam o agente de cluster para encapsular a API do Kubernetes. Os serviços do Cloud Kubernetes como o GKE já expõem o ponto de extremidade da API na Internet pública e, portanto, não exigem que o agente de cluster funcione como um encapsulamento.

 Os agentes de cluster cumprem duas funções adicionais:
 * Eles servem como proxy para outros serviços no cluster, como os alertas internos do Rancher, agregação de logs e pipelines de CI / CD. De fato, qualquer serviço em execução em clusters de usuários pode ser exposto por meio dos agentes de cluster. Esse recurso às vezes é chamado de proxy mágico.
 * Durante o registro, os agentes de cluster obtêm credenciais da conta de serviço do cluster Kubernetes e enviam as credenciais da conta de serviço ao servidor Rancher.

## Agentes de nós
 Os agentes do nó são usados principalmente pelo RKE para implantar os componentes durante a instalação inicial e as atualizações subsequentes. Os agentes do nó, no entanto, são implantados em clusters Kubernetes na nuvem como o GKE, mesmo que não sejam necessários para a instalação e atualização do Kubernetes. Os agentes do nó cumprem várias funções adicionais para todos os clusters: 
 * **Fallback para agentes de cluster**: se o agente de cluster não estiver disponível por qualquer motivo, o servidor Rancher usará o agente do nó para conectar-se ao servidor da API Kubernetes.
 * **Proxy para o shell kubectl**: O servidor Rancher se conecta através de agentes do nó para encapsular o shell kubectl na interface do usuário. O agente do nó é executado com mais privilégios que o agente de cluster e esse privilégio adicional é necessário para encapsular o shell kubectl.

# Melhoria
 Os usuários podem atualizar para novas versões do Rancher 2.3, atualizando o servidor do Rancher. O Rancher 2.3 lida com atualizações de cluster RKE. O Rancher 2.3 se integra a provedores de nuvem como o GKE para atualizar os clusters do GKE. O Rancher 2.3 não tenta atualizar os clusters Kubernetes importados. Como parte do Rancher 2.3, os lançamentos do Kubernetes agora podem ser executados fora de um ciclo de lançamento do Rancher. Isso permite um tempo de entrega mais rápido para os usuários finais e minimiza o escopo da mudança.
 
 O Rancher 1.0 foi desenvolvido no Docker e não pode ser atualizado para um cluster Kubernetes sem interromper a carga de trabalho. Os usuários do Rancher 1.0 devem configurar um cluster Rancher 2.3 separado, migrar sua carga de trabalho e descomissionar o cluster Rancher 1.0.

# Alta disponibilidade
 Os usuários podem usar um cluster RKE dedicado para executar o servidor Rancher. O guia de instalação padrão do Rancher 2.3, por exemplo, cria uma implantação do RKE com 3 nós, cada um executando uma instância do servidor de API e o banco de dados etcd. O servidor Rancher importa automaticamente o cluster Kubernetes em que é executado. É chamado de cluster local. O Rancher aproveitará a API do Kubernetes e indiretamente usará esses clusters etcd como o armazenamento de dados primário.

# Escalabilidade
## Escalabilidae de clusters Kubernetes
 A partir do Kubernetes versão 1.6, um cluster Kubernetes pode escalar para 5.000 nós e 150.000 pods. O usuário pode esperar que o Rancher 2.3 gerencie e provisione clusters RKE nessa escala também.

## Escalabilidade de servidor Rancher
 Não há limite inerente para quantos clusters Kubernetes cada servidor do Rancher pode gerenciar. Não esperamos que o Rancher 2.3 tenha problemas para gerenciar até 1.000 clusters.

 Os limites reais de escalabilidade do servidor Rancher são:
 * Total de nós em todos os clusters.
 * Usuários e grupos.
 * Eventos coletados de todos os clusters.
O servidor Rancher armazena todas as entidades acima no banco de dados Kubernetes etcd subjacente. Melhoraremos a escalabilidade dessas dimensões ao longo do tempo para atender às necessidades do usuário.



