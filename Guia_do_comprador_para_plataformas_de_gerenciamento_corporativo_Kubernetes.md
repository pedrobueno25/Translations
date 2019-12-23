# Guia do comprador para plataformas de gerenciamento corporativo Kubernetes

# Sumário Executivo
> De acordo com a 451 Research, 76% das empresas padronizarão o Kubernetes nos próximos 3 anos, pois promete um conjunto consistente de recursos em qualquer infraestrutura - do datacenter à nuvem e até a borda - “Kubernetes and Beyond – Effective Implementation of Cloud Native Software in the Enterprise” por Jay Lyman, Analista Principal 451 Research.

 Ao unificar suas operações de TI com o Kubernetes, as empresas obtêm benefícios importantes, como maior confiabilidade, segurança aprimorada e maior eficiência com automação padronizada.

 No entanto, depender do Kubernetes upstream geralmente não é suficiente para as equipes implementarem o Kubernetes na produção. As instalações do Vanilla Kubernetes são atormentadas pela falta de visibilidade central, práticas de segurança inconsistentes e processos de gerenciamento complexos. Portanto, as plataformas de gerenciamento Kubernetes são adotadas pelas empresas para oferecer:

* **Operações consistentes de cluster**: Maior eficiência do DevOps com operações simplificadas de cluster.
* **Política de segurança e gerenciamento de usuários**: Melhores práticas de aplicação de políticas de segurança e gerenciamento avançado de usuários em qualquer infraestrutura.
* **Ferramentas e serviços compartilhados**: Um alto nível de confiabilidade com acesso fácil e consistente a ferramentas e serviços compartilhados.

 Dado o potencial transformador do Kubernetes, não surpreende que a batalha pela liderança no mercado de gerenciamento do Kubernetes esteja esquentando rapidamente.

 A Rancher Labs, que se concentra no gerenciamento do Kubernetes desde a sua fundação em 2014, está experimentando um crescimento rápido. Enquanto isso, os fabricantes de TI, incluindo IBM e VMware, estão reivindicando esta enorme oportunidade de mercado.

 Em julho de 2019, a IBM concluiu a aquisição da Red Hat por US $ 34 bilhões e, mais recentemente, a VMware anunciou a aquisição da Pivotal por US $ 2,7 bilhões, juntamente com dois novos projetos Kubernetes: Project Pacific e Project Tanzu Mission Control. O Project Pacific permitirá que os usuários do vSphere criem clusters Kubernetes, enquanto o Tanzu Mission Control pretende fornecer um plano de controle central para o gerenciamento de clusters. Embora nenhum desses projetos estivesse disponíve quando este guia foi publicado, a VMware indicou claramente sua intenção estratégica.

 Embora existam outros players menores no mercado, o escopo deste guia é limitado à comparação dos recursos das três principais plataformas de gerenciamento Kubernetes: **Red Hat OpenShift Container Platform 4.1** (OpenShift / OCP4), **Pivotal PKS 1.5** (PKS) e **Rancher 2.3** (Rancher).

# Resumo dos Recursos

## Visão Global

* O indicador **++++** é aplicado à plataforma que é a melhor nessa categoria.
* O indicador **-+++** é aplicado ao segundo colocado nessa categoria.
* O indicador **--++** ilustra a capacidade aceitável nessa categoria.
* O indicador **---+** mostra fraca capacidade nessa categoria.
* O indicador **----** indica que a plataforma não tem capacidade nessa categoria.

## Operações consistentes de cluster

 Ao simplificar e automatizar as operações de cluster, as Plataformas de Gerenciamento Kubernetes buscam melhorar a eficiência do DevOps.

 Rancher:
 * Facilidade de instalação, configuração e manutenção: **++++**
 * Intuitive UI: **++++**
 * Multi-cloud: **++++**
 * Multi-cluster: **++++**
 * Suporte para Kubernetes hospedado: **++++**
 * Bare Metal, OpenStack & vSphere: **++++**
 * Importar Clusters Existentes: **++++**
 * Alta disponibilidade: **++++**
 * Load Balancing: **++++**
 * Auditoria centralizada: **++++**
 * Provisionamento de autoatendimento: **++++**
 * Gerenciamento Privado de Registro e Imagem: **-+++**
 * Atualizações de cluster e gerenciamento de versões: **-+++**
 * Suporte de armazenamento: **++++**
 * Arm Support: **++++**
 * Airgap Support: **++++**
 * Backup e restauração do Etcd: **++++**

OpenShift:
 * Facilidade de instalação, configuração e manutenção: **--++**
 * Intuitive UI: **++++**
 * Multi-cloud: **-+++**
 * Multi-cluster: **--++**
 * Suporte para Kubernetes hospedado: **----**
 * Bare Metal, OpenStack & vSphere: **--++**
 * Importar Clusters Existentes: **----**
 * Alta disponibilidade: **++++**
 * Load Balancing: **-+++**
 * Auditoria centralizada: **-+++**
 * Provisionamento de autoatendimento: **---+**
 * Gerenciamento Privado de Registro e Imagem: **++++**
 * Atualizações de cluster e gerenciamento de versões: **++++**
 * Suporte de armazenamento: **-+++**
 * Arm Support:  **----**
 * Airgap Support: **----**
 * Backup e restauração do Etcd: **--++**

PKS:
 * Facilidade de instalação, configuração e manutenção: **---+**
 * Intuitive UI: **--++**
 * Multi-cloud: **-+++**
 * Multi-cluster: **---+**
 * Suporte para Kubernetes hospedado: **----**
 * Bare Metal, OpenStack & vSphere: **---+**
 * Importar Clusters Existentes: **----**
 * Alta disponibilidade: **-+++**
 * Load Balancing: **--++**
 * Auditoria centralizada: **--++**
 * Provisionamento de autoatendimento: **-+++**
 * Gerenciamento Privado de Registro e Imagem: **--++**
 * Atualizações de cluster e gerenciamento de versões: **---+**
 * Suporte de armazenamento: **--++**
 * Arm Support: **----**
 * Airgap Support: **--++**
 * Backup e restauração do Etcd: **---+**

## Política de segurança e gerenciamento de usuários
 Um dos principais benefícios da implantação da Plataforma de Gerenciamento Kubernetes é a capacidade de implementar a aplicação das melhores práticas de segurança e o gerenciamento avançado de usuários em qualquer infraestrutura.

Rancher:
 * Active Directory e suporte LDAP: **++++**
 * Políticas de Pod e Segurança de Rede: **++++**
 * Adesão ao benchmark do CIS: **++++**
 * Políticas globais de RBAC: **++++**

OpenShift:
 * Active Directory e suporte LDAP: **++++**
 * Políticas de Pod e Segurança de Rede: **-+++**
 * Adesão ao benchmark do CIS: **--++**
 * Políticas globais de RBAC: **--++**

PKS:
 * Active Directory e suporte LDAP: **++++**
 * Políticas de Pod e Segurança de Rede: **--++**
 * Adesão ao benchmark do CIS: **--++**
 * Políticas globais de RBAC: **---+**

## Ferramentas e serviços compartilhados
 Uma vez implantadas, as Plataformas de Gerenciamento Kubernetes incentivam a adoção do usuário com acesso fácil, confiável e consistente a ferramentas e serviços compartilhados.

Rancher:
 * Catálogo de aplicativos: **-+++**
 * Provisão com sistemas de gerenciamento de configuração: **++++**
 * Solução CI / CD integrada: **++++**
 * Monitoramento avançado: **++++**
 * Alertas e notificações: **++++**
 * Envio de Log Externo: **-+++**
 * Suporte a contêiner do Windows: **-+++**
 * Suporte de malha de serviço integrado: **-+++**
 * Enterprise SLA: **++++**
 * Tração da comunidade: **++++**

OpenShift:
 * Catálogo de aplicativos: **++++**
 * Provisão com sistemas de gerenciamento de configuração: **--++**
 * Solução CI / CD integrada: **-+++**
 * Monitoramento avançado: **++++**
 * Alertas e notificações: **--++**
 * Envio de Log Externo: **-+++**
 * Suporte a contêiner do Windows: **----**
 * Suporte de malha de serviço integrado: **-+++**
 * Enterprise SLA: **-+++**
 * Tração da comunidade: **-+++**

PKS:
 * Catálogo de aplicativos: **--++**
 * Provisão com sistemas de gerenciamento de configuração: **-+++**
 * Solução CI / CD integrada: **--++**
 * Monitoramento avançado: **---+**
 * Alertas e notificações: **---+**
 * Envio de Log Externo: **--++**
 * Suporte a contêiner do Windows: **--++**
 * Suporte de malha de serviço integrado: **---+**
 * Enterprise SLA: **-+++**
 * Tração da comunidade: **++++**

# Análide de Recurso
## Operações consistentes de cluster
### Facilidade de instalação, configuração e manutenção
 * Rancher: **++++**
 * OpenShift: **--++**
 * PKS: **---+**

#### Rancher
 O Rancher oferece distribuições certificadas do Kubernetes para datacenter, nuvem e edge. Cada distribuição requer o mínimo de configuração do host, geralmente não mais do que uma versão suportada do Docker. Para instalações que desejam uma superfície de ataque ainda menor, o Rancher oferece dois sistemas operacionais de contêinere projetados expressamente para executar o Kubernetes da maneira mais eficiente possível.
 O Kubernetes do Rancher usa uma sintaxe de configuração projetada para clareza e reconfiguração dinâmica de cluster sem tempo de inatividade.

#### OpenShift
 O OpenShift (OCP4) envia um grande binário de instalação que inclui o Terraform e um conjunto de scripts para implantar o OCP4 em um provedor. Atualmente, os únicos fornecedores suportados são AWS, Azure e vSphere. Somente o instalador da AWS foi avaliado para este guia. O instalador requer acesso irrestrito à AWS para criar e gerenciar recursos que consumirá. A execução do binário de instalação é fácil porque não há opções disponíveis para a configuração do cluster no momento da inicialização. Toda a configuração acontece no OCP4 após o cluster estar online. No entanto, a pegada que o OCP4 cria na AWS é grande e dificulta a solução de problemas. Não está claro se as alterações no ambiente da AWS serão substituídas durante as atualizações do cluster no OCP4. Se o usuário desejar desviar-se dos padrões fornecidos pelo OCP4, poderá encontrar dificuldades em fazê-lo.

#### PKS
 O PKS requer pré-requisitos do Ops Manager, BOSH Director e PKS Manager. Se estiver usando recursos opcionais, também poderá ser necessária uma instalação de vários nós do plano de controle NSX-T e do Harbor. A instalação e configuração desses componentes levará de oito a 16 horas.
 A implantação do cluster PKS real pode levar até 30 minutos para implantar um cluster básico. As alterações na configuração do PKS também demoram 30 minutos para seremaplicadas e requerem um relançamento dos clusters a jasante.

### Intuitive UI
 * Rancher: **++++**
 * OpenShift: **++++**
 * PKS: **--++**

#### Rancher
 A interface do usuário orientada por intenção do Rancher permite que os usuários implantem e iniciem rapidamente o gerenciamento de clusters Kubernetes com quase nenhuma curva de aprendizado. Ele suaviza e agiliza conceitos e fluxos de trabalho complexos do Kubernetes, possibilitando o aproveitamento do Kubernetes em uma organização sem a necessidade de treinamento extensivo antecipadamente.

#### OpenShift
 A interface do usuário do OpenShift é nítida e rápida. Existem fluxos de trabalho comuns na parte superior dos menus, e o acesso aos fluxos de trabalho padrão do Kubernetes e aos exclusivos do OpenShift está prontamente disponível.

#### PKS
 Além do bloco que inicia um cluster PKS, não há interface do usuário. Os usuários podem optar por instalar o painel Kubernetes de código aberto. Nenhuma outra opção é fornecida.

### Multi-cloud
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **-+++**

#### Rancher
 O Rancher apresenta mais opções de onde implantar o Kubernetes. Ele pode provisionar soluções hospedadas de todos os principais fornecedores. Ele pode provisionar recursos de computação em qualquer provedor para o qual existem drivers para o Docker Machine e instalar o Kubernetes nesse ambiente. Ele pode importar clusters Kubernetes existentes em execução em qualquer provedor. Ele também apresenta uma opção personalizada para instalar o Kubernetes em qualquer sistema provisionado por qualquer outro meio, como Ansible, Terraform, Puppet, Chef, etc.

#### OpenShift
 O OpenShift suporta implantações em nuvem na AWS ou através de um serviço especial do Azure. Como o OpenShift não é uma solução com vários clusters ou várias nuvens, ele não contém nenhuma funcionalidade para gerenciar várias nuvens ou reduzir o risco de aprisionamento em uma única nuvem.

#### PKS
 O PKS Manager implanta recursos de nuvem, mas está bloqueado para um único provedor de nuvem. Embora seja possível instalar várias instâncias do PKS Manager para várias nuvens, cada uma delas é diferente e requer sua própria configuração independente. Clusters lançados pelo PKS Manager está sob o guarda-chuva do PKS Manager e não oferece portabilidade entre nuvens, configuração compartilhada ou outras estratégias para reduzir a carga de trabalho do operador. O PKS segue as versões do KCP do Kubernetes, que permitem que as cargas de trabalho do PKS sejam reimplantadas manualmente no GCP, sem problemas com acompatibilidade de recursos.

### Multi-cluster
 * Rancher: **++++**
 * OpenShift: **--++**
 * PKS: **---+**

#### Rancher
 O Rancher disponibiliza a funcionalidade Kubernetes por meio de uma interface do usuário e API avançadas. Isso, por sua vez, possibilita aos usuários interagir com o Kubernetes sem precisar saber onde ele está ou como está configurado. O Rancher abstrai recursos específicos da nuvem, como Gerenciamento de identidade e acesso, e reduz o bloqueio, permitindo que os operadores apliquem políticas de segurança padrão em clusters executados em nuvens diferentes. O Rancher Longhorn abstrai o armazenamento e permite a portabilidade de aplicativos entre nuvens, apresentando uma interface padrão às primitivas subjacentes do Kubernetes.

#### OpenShift
 O OpenShift não suporta vários clusters além de uma interface da web que implanta e gerencia clusters OpenShift individuais.

#### PKS
 O PKS não suporta vários clusters, além de permitir que os usuários iniciem vários clusters que são completamente independentes.

### Suporte gerenciado ao Kubernetes
 * Rancher: **++++**
 * OpenShift: **----**
 * PKS: **----**

#### Rancher
 O Rancher suporta a implantação em soluções Kubernetes gerenciadas da Amazon (EKS), Google (GKE) e Azure (AKS), bem como soluções da Alibaba, Baidu, Huawei e Tencent. Se um usuário desejar implantar um cluster com um novo provedor, ele poderá importar um driver para esse provedor diretamente da interface do usuário.

#### OpenShift
 O OpenShift não suporta nenhum provedor hospedado do Kubernetes.

#### PKS
 O PKS não suporta nenhum provedor hospedado do Kubernetes.


### Bare Metal, OpenStack & vSphere 
 * Rancher: **++++**
 * OpenShift: **--++**
 * PKS: **---+**

#### Rancher
 O Rancher é fornecido com drivers para implantação em provedores comuns de nuvem, como AWS, GCP, Azure, DigitalOcean, Rackspace e outros, além de oferecer suporte a qualquer provedor de nuvem para o qual exista um driver da Docker Machine. Ele também é fornecido com drivers para OpenStack e vSphere, possibilitando aos usuários dessas tecnologias implantar o Kubernetes junto com suas máquinas virtuais existentes. O Rancher Kubernetes Engine requer apenas uma versão suportada do Docker, tornando-o adequado para implantações bare-metal de qualquer distribuição Linux. Os usuários que procuram um sistema operacional leve e seguro para implantações bare metal o encontrarão no RancherOS ou no k3OS.

#### OpenShift
 O OpenShift suporta a implantação no bare metal e no vSphere.

#### PKS
 O PKS suporta a implantação apenas no vSphere.

### Importar clusters existentes
 * Rancher: **++++**
 * OpenShift: **----**
 * PKS: **----**

#### Rancher
 O Rancher importa clusters Kubernetes existentes, disponibilizando-os para gerenciamento na interface do usuário do Rancher. Esses clusters podem estar em execução na nuvem, em um provedor hospedado, em bare metal ou máquinas virtuais ou em qualquer outra plataforma. Se o cluster estiver executando uma versão não adulterada do Kubernetes, o Rancher poderá importá-lo sem nenhuma etapa extra necessária. Se o cluster estiver executando uma versão não padrão do Kubernetes (OpenShift, PKS, etc), será necessária uma configuração extra para o Rancher gerenciá-lo.

#### OpenShift
 O OpenShift não pode importar clusters externos de nenhum provedor.

#### PKS
 O PKS não pode importar clusters externos de nenhum provedor.

### Alta disponibilidade
 * Rancher: **++++**
 * OpenShift: **++++**
 * PKS: **-+++**

#### Rancher
 As implantações do Rancher nos fornecedores hospedados do Kubernetes utilizam a configuração do fornecedor para alta disponibilidade. Ao implantar em outras soluções, o Rancher permite que o usuário escolha a configuração do nó para o control plane, etcd e workers, permitindo que eles escolham a configuração de alta disponibilidade que melhor se adequa à função do cluster na organização. Também permitirá que o usuário escolha em qual zona de disponibilidade os nós serão executados. Os clusters implantados com o RKE podem ser reconfigurados dinamicamente para configurações de alta disponibilidade de 3, 5 e 7 nós à medida que as necessidades da organização evoluem. A alta disponibilidade no nível da máquina virtual é fornecida pelo provedor, onde uma solução como AutoScaling Groups (ASGs) e CloudWatch recriam máquinas virtuais que não respondem.

#### OpenShift
 O OpenShift sempre implanta um cluster Kubernetes altamente disponível com cinco nós para o control plane e etcd, independentemente de qualquer nó worker.

#### PKS
 A alta disponibilidade do Kubernetes no PKS é ativada no momento da implantação, implantando vários nós de control plane ou etcd. A disponibilidade da máquina virtual é gerenciada pelo BOSH, que substitui a solução de monitoramento do provedor. O BOSH detectará uma máquina que esteja inativa por mais de um minuto e usará uma chamada de API para instruir o provedor a substituí-la. Como o monitoramento não está no nível do provedor, existe o risco de uma partição de rede do servidor BOSH resultar na recriação de sistemas que não estão realmente inoperantes.

### Load Balancing
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **--++**

#### Rancher
 Os clusters instalados pelo Rancher nas instâncias de computação incluem o Nginx Ingress Controller para balanceamento de carga. Se o Rancher implantar um cluster em um provedor hospedado que não instala um controlador de entrada por padrão (como o EKS), a integração do Rancher App Catalog e Helm permite a instalação com um clique de um controlador do Ingress. Isso também provisionará um Serviço LoadBalancer específico do provedor, quando apropriado. Todos os clusters Kubernetes implantados em um provedor de nuvem conhecido também suportam a implantação de balanceadores de carga específicos do provedor por meio do Serviço do tipo LoadBalancer. Todas as soluções padrão de entrada e balanceamento de carga (incluindo gateways de API e malha de serviço) são compatíveis com os clusters implementados pelo Rancher.

#### OpenShift
 Além do Kubernetes Ingress padrão, o OpenShift usa um balanceador de carga de software proprietário chamado Route. Ele se comporta de maneira semelhante a um Ingress, mas existe apenas no OpenShift e não é portátil para outros serviços do Kubernetes. Os controladores do OpenShift Ingress são gerenciados pelo operador do Ingress. Ele implementa um balanceador de carga padrão baseado em HAProxy para lidar com as solicitações de Route e de entrada.

#### PKS
 As instalações do PKS que não usam o driver de rede VMWare NSX-T exigem a implantação manual de um balanceador de carga externo. As instalações na AWS exigem configuração manual adicional de sub-redes e etiquetas de VPC antes que o balanceador de carga possa ser usado com o PKS. As instalações com o NSX-T possuem uma solução robusta de balanceamento de carga para a API do Kubernetes e cargas de trabalho do usuário, incluindo suporte ao tráfego TCP e UDP para os serviços do LoadBalancer. O NSX-T não suporta serviços do tipo NodePort.

### Auditoria centralizada
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **--++**

#### Rancher
 O Rancher pode registrar toda a interação com a API do Rancher, incluindo o corpo e os metadados da solicitação e resposta. Essas informações são registradas no stdout ou podem ser enviadas para um endpoint externo por meios padrão disponíveis na plataforma (Fluentd, syslog, etc.). O Rancher também suporta o log de API padrão disponível no Kubernetes.

#### OpenShift
 O OpenShift pode registrar toda a interação com a API do OCP, incluindo o corpo e os metadados da solicitação e resposta. Esta informação é registrada nos arquivos e pode ser consultada através do comando oc. Requer conhecer o host e o arquivo de log a serem consultados. O OpenShift também suporta o log de API padrão disponível no Kubernetes.

#### PKS
 A natureza distribuída da infraestrutura de suporte necessária para o PKS significa que os logs de auditoria também são distribuídos entre diferentes componentes e máquinas diferentes. Os componentes PCF suportam logs de eventos e logs de eventos de segurança. Isso requer um ponto final syslog para arquivamento e processamento.
 Uma vez implantado, o PKS é o Kubernetes. Ele suporta o log e a API padrão da API que o Kubernetes oferece.

### Provisionamento de autoatendimento
 * Rancher: **++++**
 * OpenShift: **---+**
 * PKS: **-+++**

#### Rancher
 O Rancher usa um esquema de permissões granulares para conceder ou negar acesso a recursos nos níveis Global, Cluster e Projeto (namespace). Os usuários com acesso ao servidor Rancher verão apenas seus próprios clusters ou projetos, e o isolamento opcional do espaço para nome garante que os clusters com vários inquilinos permaneçam seguros. Delegação de privilégios significa que um administrador global pode conceder a outro usuário a permissão para criar clusters que somente eles ou sua equipe podem ver. Essa delegação de responsabilidades, juntamente com os parâmetros de como e onde os clusters são implantados, fornece aos desenvolvedores acesso aos recursos necessários, garantindo ao mesmo tempo que todo o ambiente permaneça seguro. O provisionamento de clusters Kubernetes pode ser feito por meio da interface do usuário, CLI ou API.

#### OpenShift
 O OpenShift é uma solução de cluster único que deve ser implantada por meio do programa instalador. Ele não contém meios para iniciar novos clusters.

#### PKS
 O Pivotal Ops Manager, necessário para o PKS, permite que os usuários da plataforma implementem clusters PKS a partir de uma lista de até 10 configurações de cluster (chamadas Planos). Cada plano contém as instruções de como um cluster será implantado, incluindo parâmetros como configuração de alta disponibilidade, tamanho da instância, VPC e zona de disponibilidade. Embora o PKS permita algumas alterações nos planos, qualquer alteração no número de nós etcd ou master exige primeiro que todos os clusters que usam o plano sejam destruídos.

### Gerenciamento privado de registro e imagem
 * Rancher: **-+++**
 * OpenShift: **++++**
 * PKS: **--++**

#### Rancher
 O Rancher contém suporte completo para registros particulares. Apresenta uma guia na interface do usuário em que os usuários podem inserir suas credenciais de registro.Eles são salvos como segredos do Kubernetes e usados ao extrair de registros particulares.

#### OpenShift
 O OpenShift contém suporte completo para registros particulares e inclui um registro local usado para imagens criadas localmente. O acesso ao registro local usa as credenciais do usuário solicitante ao determinar as permissões. O acesso a registros externos usa a OC CLI para criar o ImagePullSecrets e, opcionalmente, anexá-los às contas de serviço.

#### PKS
 O PKS usa os recursos disponíveis no Kubernetes para acessar registros privados e autenticados. Os usuários devem criar manualmente objetos de credencial do registro e vinculá-los a cargas de trabalho que os usarão.

### Atualizações de cluster e gerenciamento de versão
 * Rancher: **-+++**
 * OpenShift: **++++**
 * PKS: **---+**

#### Rancher
 O Rancher Kubernetes Engine (RKE) executa o Kubernetes upstream nos contêineres do Docker. As atualizações nos serviços individuais do Kubernetes podem ser executadas atomicamente, com suporte completo para reversão para versões anteriores. Todas as atualizações do Kubernetes são executadas com zero tempo de inatividade para a execução de cargas de trabalho. Uma atualização completa contínua de um cluster de 3 nós levará aproximadamente 10 minutos. O Rancher libera atualizações de segurança para o RKE dentro de duas semanas da liberação upstream da equipe Kubernetes e atualizações não urgentes do Kubernetes dentro de quatro semanas.

#### OpenShift
 O OpenShift usa operadores Kubernetes para implantar e atualizar os componentes de cluster Kubernetes. Todas as atualizações do Kubernetes são executadas com zero tempo de inatividade para a execução de cargas de trabalho. Uma atualização completa de um cluster de 3 nós levará aproximadamente 15 minutos.

#### PKS
 O PKS executa atualizações com tempo de inatividade zero para as cargas de trabalho em execução. Uma atualização completa de um cluster de três nós levará aproximadamente 30 minutos. O aumento do tempo é uma função da primeira atualização dos componentes BOSH Director, PKS Manager e Ops Manager antes de executar uma atualização dos clusters PKS. As atualizações de cluster podem ser automatizadas com o Concourse, outro produto Pivotal.

### Suporte de armazenamento
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **--++**

#### Rancher 
 O Rancher desenvolve o Longhorn e mantém parcerias com Portworx, StorageOS e OpenEBS. Esses fornecedores certificam seu software nas versões do Rancher, para que os usuários de ambos os produtos possam ter certeza de que trabalham bem juntos.

#### OpenShift
 A Red Hat mantém o Operator Hub e possui um processo de certificação projetado para reduzir problemas de compatibilidade entre produtos de terceiros e o OpenShift. Entre outras coisas, a certificação exige que os Operators sejam construídos usando a pilha de software da Red Hat.

#### PKS
 O PKS não oferece certificação oficial de produtos de armazenamento, mas qualquer fornecedor certificado para trabalhar com o Kubernetes provavelmente trabalhará com o PKS.

### Suporte Arm
 * Rancher: **++++**
 * OpenShift: **----**
 * PKS: **----**

#### Rancher
 O RKE e o k3s suportam a instalação no ARM64 e ARMv7. O Rancher tem uma parceria com a Arm e trabalha em estreita colaboração com sua equipe de engenharia em novos lançamentos.

#### OpenShift
 O OpenShift não suporta a implantação em processadores ARM.

#### PKS
 O PKS não suporta a implantação em processadores ARM.

### Suporte Airgap
 * Rancher: **++++**
 * OpenShift: **----**
 * PKS: **--++**

#### Rancher
 O Rancher suporta instalações com airgap e inclui documentação sobre como provisionar um servidor de registro privado e preenchê-lo com todas as imagens necessárias para a instalação.

#### OpenShift
 O OpenShift suportou instalações de airgap, que eles chamaram de Instalações Desconectadas, na versão 3.5, mas não no OCP4.

#### PKS
 O Pivotal Cloud Foundry, um dos componentes fundamentais do PKS, suporta instalações de airgap em vários cenários. A necessidade de oferecer suporte ao airgap para todos os pré-requisitos do PKS aumenta a complexidade da instalação e configuração do PKS.

### Backup e restauração do Etcd
 * Rancher: **++++**
 * OpenShift: **--++**
 * PKS: **---+**

#### Rancher
 Todos os clusters RKE implantados no Rancher são automaticamente copiados para o armazenamento local em intervalos regulares. O operador pode mudar isso para um terminal compatível com S3. Os clusters podem ser restaurados para qualquer captura instantânea da interface do usuário ou da CLI. As implantações de alta disponibilidade do servidor Rancher exigem
configuração manual do cluster RKE para executar backups. Eles também podem gravar no armazenamento local ou em um terminal compatível com S3. A restauração de um cluster de alta disponibilidade requer a implantação de um novo cluster Kubernetes, a restauração do backup e a execução de uma nova instalação do Rancher.
Após a conclusão, todos os clusters remotos do Kubernetes serão reconectados ao novo cluster.

#### OpenShift
 O backup de um cluster OCP4 requer login manual em um host etcd e execução de um script. Embora isso possa ser automatizado com o cron, ele não inclui nenhuma provisão para salvar em um terminal remoto. Como resultado, uma solução de backup eficaz dependerá do operador para projetar, instalar e manter a solução.

#### PKS
 É possível fazer backup dos clusters PKS usando o BOSH Backup and Restore (BBR), mas o backup deve ser executado manualmente. A configuração do BBR inclui dezenas de etapas e o armazenamento de credenciais de acesso remoto em uma conta de usuário na máquina em que o backup é executado.
Restaurar um cluster PKS requer restaurar todo o cluster PCF, o PKS Manager e os clusters PKS. O processo também requer dezenas de pré-requisitos e avisa que pode levar muito tempo para ser concluído. Nem backup nem restauração são aprovados para uso com clusters em execução no vSphere with NSX-T.

## Segurança, Política e Gerenciamento de Usuários
### Active Directory e suporte LDAP 
 * Rancher: **++++**
 * OpenShift: **++++**
 * PKS: **++++**

#### Rancher
 O Rancher se integra diretamente aos fornecedores do Active Directory, Azure AD, OpenLDAP, FreeIPA, OAuth, como GitHub e SAML, como Keycloak e Okta. A configuração da integração ocorre no nível Global, após o qual usuários e grupos do provedor estão disponíveis para atribuição às funções RBAC e clusters de recebimento de dados.

#### OpenShift
 O OpenShift executa um servidor OAuth interno e proxy de comunicação para vários provedores de back-end. Mantém a compatibilidade com provedores baseados em LDAP, Keystone, OpenID e OAuth, além de fornecer uma interface para autenticação básica e sistemas de autenticação externos capazes de definir um cabeçalho de solicitação.

#### PKS
 A autenticação PKS é gerenciada pelo Ops Manager, que se comunica nativamente com qualquer provedor de back-end que fale SAML. Existem várias integrações de parceiros para habilitar a autenticação com sistemas como Aqua e CredHub.

### Políticas de segurança de pod e rede
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **--++**

#### Rancher
 O Rancher oferece suporte à configuração da Política de Segurança do Pod no nível Global. Os modelos PSP são então atribuídos a clusters a jusante. Isso garante a conformidade e reduz o risco de erro humano ao alterar políticas. PSPs podem ser criados e editados através da interface do usuário.

#### OpenShift
 O OpenShift usa restrições de contexto de segurança para executar a função de um objeto de Política de Segurança de Pod no Kubernetes. Ele contém uma implementação robusta do SCC para o cluster. Os SCCs podem ser editados apenas através do comando oc na CLI.

#### PKS
 O PKS suporta políticas de segurança de pod nativas no Kubernetes. Não oferece nenhum benefício ou gerenciamento adicional em torno da implementação do Kubernetes.

### Adesão configurável às referências de segurança
 * Rancher: **++++**
 * OpenShift: **--++**
 * PKS: **--++**

#### Rancher
 O Rancher mantém um guia de fortalecimento e uma autoavaliação que referencia os benchmarks do CIS com ações específicas que um usuário pode executar para satisfazer os requisitos.

#### OpenShift
 O OpenShift não oferece informações adicionais em sua documentação sobre aderência ou orientação do benchmark da CIS para seus clientes. Os clientes podem usar testes públicos para a adesão ao Kubernetes, mas isso não cobre nada exclusivo do OpenShift.

#### PKS
 A Pivotal não oferece orientação sobre o fortalecimento das implantações do PKS. Uma solicitação de suporte de março de 2019 relata que o kube-bench não funciona com clusters PKS, deixando os usuários a encontrar sua própria solução.

### Políticas RBAC












