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
 * Rancher: **++++**
 * OpenShift: **--++**
 * PKS: **---+**

#### Rancher
 O Rancher expõe todos os RBAC do Kubernetes e, em seguida, permite a configuração e manutenção das políticas do RBAC no nível global em nossa interface do usuário. Existem políticas para os níveis Global, Cluster e Projeto e, além dos modelos que Rancher fornece, os usuários podem criar um número infinito de modelos para definir novas funções. Os modelos de usuário podem herdar dos modelos existentes para criar uma hierarquia de permissões que são facilmente mantidas.

#### OpenShift
 O OpenShift renomeia os objetos de política do Kubernetes para clusterPolicy e localPolicy e usa um formato de configuração proprietário que remove a compatibilidade com outras implantações do Kubernetes. O gerenciamento das políticas é feito através do comando oc. Nenhum gerenciamento está disponível através da interface do usuário.

#### PKS
 O PKS opera através do sistema Kubernetes RBAC, mas como o esquema de autenticação existe fora do PKS, os administradores do operador e do cluster devem executar etapas adicionais e executar componentes de integração adicionais para ativar a autenticação do usuário e do grupo.

## Ferramentas e serviços compartilhados
### Catálogo de aplicativos
 * Rancher: **-+++**
 * OpenShift: **++++**
 * PKS: **--++**

#### Rancher
 O Catálogo de aplicativos da Rancher estende o Helm para fornecer aos usuários um processo de instalação facilmente baseado em formulário para aplicativos. Ele se integra a qualquer repositório Helm externo, oferecendo aos usuários os meios para instalar aplicativos de qualquer sistema. O Tiller, o componente interno de Helm, é frequentemente citado como um risco de segurança, porque geralmente é implantado com privilégios de nível de administrador em um cluster. O catálogo de aplicativos do Rancher não requer Tiller e, como tal, é uma implementação mais segura do Helm.

#### OpenShift
 O OpenShift se integra ao Operator Hub da Red Hat, uma lista com curadoria de aplicativos que atendem aos requisitos de inclusão da Red Hat. A Red Hat incentiva os usuários a converter gráficos Helm em Operators. Muitos gráficos Helm não serão executados nativamente devido à incompatibilidade com as permissões padrão no OCP4. Mesmo se implantado manualmente, o Helm não é suportado pelo OCP4 e pode invalidar o suporte ao cluster.

#### PKS
 O PKS suporta a instalação e uso padrão do Helm.

### Provisão com Terraform / Ansible / Outros
 * Rancher: **-+++**
 * OpenShift: **--++**
 * PKS: **-+++**

#### Rancher
 O Rancher mantém o provedor Terraform, que permite aos usuários implantar e gerenciar o Rancher usando os princípios de IaC. Embora não esteja oficialmente integrada a outras soluções, a API aberta do Rancher e o uso de contêineres do Docker para RKE facilitam a integração com soluções como Ansible, Puppet, Chef, grupos de dimensionamento automático da AWS, init na nuvem ou outras estratégias de provisionamento.

#### OpenShift
 O OpenShift usa o Terraform para sua instalação, mas o faz agrupando o instalador do Terraform e todos os scripts no binário do instalador. Eles não são visíveis ao usuário ou estão disponíveis para inclusão em um fluxo de trabalho IaaS corporativo.

#### PKS
 O Pivotal usa o Terraform como o método suportado para instalar o PCF e o PKS. Repositórios do Github existem para os principais provedores de nuvem, OpenStack e vSphere.

### Recursos de CI/CD
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **--++**

#### Rancher
 O Rancher se integra a qualquer sistema de CI / CD que funcione com o Kubernetes. Se um usuário ainda não possui um sistema de CI / CD, ele pode usar o sistema Pipeline incorporado ao Rancher para começar a usar os fluxos de trabalho de CI / CD. O Rancher Pipelines é baseado no Jenkins e se conecta a repositórios do GitHub, Gitlab e Bitbucket.

#### OpenShift
 O OpenShift funcionará com qualquer sistema de CI / CD que funcione com o Kubernetes. Além disso, com a versão 4.1, a Red Hat lançou uma prévia do OpenShift Pipelines, baseado no Tekton.

#### PKS
 O PKS funcionará com qualquer sistema de CI / CD que funcione com o Kubernetes.

### Monitoramento avançado
 * Rancher: **++++**
 * OpenShift: **++++**
 * PKS: **---+**

#### Rancher
 O Rancher é enviado com o monitoramento básico ativado por padrão. Os administradores de cluster podem ativar o monitoramento avançado com um único clique na interface do usuário do Rancher. Isso implanta o Prometheus e o Grafana nos níveis do projeto e do cluster e instala painéis pré-configurados que permitem visibilidade imediata nas operações do cluster. Os usuários podem acessar o Grafana e visualizar as métricas dos recursos aos quais têm acesso. Eles também podem anotar suas cargas de trabalho para que o Prometheus comece a extrair métricas personalizadas deles.

#### OpenShift
 O OpenShift é enviado com o Prometheus e o Grafana ativados por padrão, com painéis Grafana pré-configurados. Esta instalação está disponível apenas para monitorar componentes OpenShift. Os usuários devem instalar sua própria solução para monitorar as cargas de trabalho do usuário.

#### PKS
 O PKS não possui nenhum monitoramento ou visualização instalado por padrão. Os usuários podem acessar manualmente os dados de telemetria e uso do banco de dados PKS no ambiente PCF. O BOSH monitora os nós do PKS e destruirá e recriará os nós que julgar não responderem. A única solução suportada para monitoramento adicional do PKS requer uma cópia licenciada do VMware Wavefront.

### Alertas e Notificações
 * Rancher: **++++**
 * OpenShift: **--++**
 * PKS: **---+**

#### Rancher
 O monitoramento básico padrão e o monitoramento avançado opcional configuram alertas para componentes críticos do cluster. Os usuários precisam apenas criar destinos de notificação. O Rancher suporta o envio de alertas para Slack, PagerDuty, WeChat, email ou qualquer destino de webhook. Os notificadores podem ser configurados nos níveis de cluster e projeto, permitindo a delegação de responsabilidades por eventos de aplicativos para as equipes responsáveis.

#### OpenShift
 Os destinos de notificação do OpenShift exigem configuração manual do AlertManager e proíbem expressamente o desvio de um pequeno subconjunto da funcionalidade do AlertManager.

#### PKS
 O PKS suporta o uso de Sinks para interceptar e encaminhar dados métricos para um coletor externo. O coletor externo deve ser instalado e mantido externo ao PKS.

### Envio de log externo
 * Rancher: **-+++**
 * OpenShift: **-+++**
 * PKS: **--++**

#### Rancher
 O Rancher é enviado com conectores para Elasticsearch, Fluentd, Splunk, Kafka e syslog.

#### OpenShift
 O OpenShift pode implantar uma pilha EFK (Elasticsearch, Fluentd, Kibana) dentro do cluster e usá-la para log.

#### PKS
 O PKS suporta a configuração de Sinks, que interceptam e encaminham dados de log para um destino syslog ou webhook.

### Suporte para contêiners no Windows
 * Rancher: **-+++**
 * OpenShift: **----**
 * PKS: **--++**

#### Rancher
 O Rancher suporta nós worker do Windows começando com o Rancher 2.3 e o Kubernetes 1.14. Os nós worker do Windows e Linux podem existir juntos (os nós do Linux executam o control plane, etcd e ingress) no mesmo cluster do Kubernetes e o Rancher implementará a carga de trabalho apropriada no nó apropriado.

#### OpenShift
 O OpenShift (OCP4) não contém suporte de produção para o uso de servidores Windows em clusters do Kubernetes ou para a implantação de contêineres do Windows no Kubernetes.

#### PKS
 O PKS contém suporte beta para contêineres do Windows no vSphere. Os clusters PKS que usam contêineres do Windows devem conter apenas nós worker do Windows.

### Suporte integrado ao Service Mesh
 * Rancher: **-+++**
 * OpenShift: **-+++**
 * PKS: **---+**

#### Rancher 
 O Rancher contém a ativação com um clique do Istio upstream com visualização no painel do Rancher por meio do Kiali. Os usuários podem usar imediatamente os benefícios da malha de serviço nos clusters implantados no Rancher ou, se desejarem usar uma alternativa diferente do Istio, poderão implantá-lo no catálogo de aplicativos.

#### OpenShift
 O OpenShift instala uma versão do Istio modificada pelo Red Hat para funcionar no OpenShift. Embora seja funcionalmente semelhante ao Istio, não se moverá tão rapidamente quanto a Istio de liberação de cadência a montante.

#### PKS
 O PKS não contém suporte nativo para nenhuma malha de serviço. A funcionalidade de malha de serviço está disponível no VMware NSX-T e CloudFoundry, mas elas são fundamentalmente diferentes da funcionalidade que uma malha de serviço fornece para implantações do Kubernetes.

### SLA corporativo
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **-+++**

#### Rancher
 O Rancher Labs fornece uma assinatura corporativa que abrange o Rancher, Docker, Kubernetes e todos os softwares nativos da nuvem que o Rancher inclui. Ele também inclui garantia e indenização de IP e está disponível em pacotes configuráveis para suporte em horário comercial ou 24x7. A assinatura do Rancher é avaliada por nó, independentemente do número de núcleos.

#### OpenShift
 A Red Hat fornece suporte para o OpenShift e a pilha de software da Red Hat. Muitos dos componentes do OpenShift não podem ser modificados ou usados fora dos parâmetros ditados pelo Red Hat sem invalidar o suporte. O modelo de suporte da Red Hat é precificado por núcleo virtual, tornando cada atualização do ambiente do cliente um aumento no custo de suporte.

#### PKS
 O PKS, como parte do PCF, é a versão suportada dos produtos de código aberto do Cloud Foundry. As versões do Pivotal, bem como as versões do VMware, incluem suporte para operação em determinadas plataformas. Em alguns casos, o suporte está incluído no custo da assinatura (como no VMware Cloud PKS) ou em outros casos, o suporte é licenciado externamente.

### Comunidade
 * Rancher: **++++**
 * OpenShift: **-+++**
 * PKS: **++++**

#### Rancher
 O Rancher possui uma comunidade próspera de usuários e colaboradores em todos os seus produtos e projetos. Com mais de 100 milhões de downloads e +25.000 implantações, é a solução de código aberto mais popular para implantar e gerenciar clusters Kubernetes.

#### OpenShift
 A Red Hat possui uma grande comunidade de usuários de código aberto em toda a sua linha de produtos. Embora o OpenShift Container Platform seja uma oferta comercial, os componentes da solução existem em um formulário de código aberto. A dificuldade em implantar e manter componentes díspares pode levar as pessoas a comprar a versão comercial do OCP4 ou usar soluções alternativas.

#### PKS
 A origem de código aberto do PKS é o Cloud Foundry Container Service. O Cloud Foundry foi criado originalmente pela VMware e agora é mantido pela Pivotal. O Cloud Foundry possui uma sequência de código aberto grande e robusta, além da certificação da plataforma, todos os recursos do Pivotal PKS estão disponíveis no Serviço de Contêiner do Cloud Foundry.

# Sobre o autor
 A Rancher Labs é a empresa por trás dos seguintes produtos de código aberto:
 
 * Rancher - a plataforma de gerenciamento Kubernetes de nível empresarial mais popular do mundo;
 * RKE - um instalador Kubernetes simples e extremamente rápido que funciona em qualquer lugar;
 * K3s - uma distribuição Kubernetes leve, de nível de produção, criada para sistemas embarcados e para o Edge;
 * Rio - um MicroPaaS que oferece uma experiência de desenvolvimento totalmente integrada do pipeline às operações sem assumir o controle do cluster.

 Juntos, esses produtos ajudam as equipes de ITOps e DevOps a enfrentar os desafios operacionais e de segurança do gerenciamento de clusters Kubernetes certificados em qualquer infraestrutura. Eles também fornecem aos desenvolvedores uma pilha integrada de ferramentas para criar e executar cargas de trabalho em contêiners em escala.

 Para saber mais sobre o Rancher Labs, visite <https://rancher.com/>

# Glosário
 ## Operações consistentes de cluster
 * Facilidade de instalação, configuração e manutenção
   * Uma plataforma de gerenciamento Kubernetes deve ser fácil e rápida de implementar. A implantação deve ser medida em minutos, em vez de horas ou, em alguns casos, dias.
 
 * UI Intuitivo
   * Uma interface de usuário intuitiva e refinada deve permitir operações que abranjam vários clusters em execução em diferentes regiões, datacenters e provedores de nuvem.
 
 * Multi-cloud
   * O suporte a ambientes de nuvem populares como AWS, Azure e GCP minimiza os riscos comerciais e técnicos associados ao bloqueio em um único provedor de nuvem.
 
 * Multi-cluster
   * Para executar o Kubernetes em produção sem o bloqueio do fornecedor, você precisa gerenciar vários clusters do Kubernetes usando a mesma experiência de usuário unificada, local ou em qualquer ambiente em nuvem.

 * Suporte gerenciado ao Kubernetes
   * Há muitos bons motivos para os usuários favorecerem a velocidade de implantação, a resiliência e as ferramentas de provedores de serviços gerenciados como AKS, EKS e GKE. Uma plataforma de gerenciamento Kubernetes deve oferecer aos usuários a escolha do ambiente de implantação sem favorecer nenhum fornecedor.

 * Bare Metal, Cloud, OpenStack & vSphere
   * Para dar suporte às implantações híbridas do Kubernetes, a plataforma de gerenciamento Kubernetes escolhida também deve oferecer suporte a virtualização comum, nuvem privada e ambientes bare metal.

 * Importar clusters existentes
   * A capacidade de importar clusters Kubernetes existentes é particularmente importante para aqueles que iniciaram sua jornada no Kubernetes usando o Kubernetes Vanilla ou um serviço Kubernetes gerenciado, mas desejam consolidar seu gerenciamento com uma única interface.

 * Alta disponibilidade
   * As plataformas de gerenciamento Kubernetes devem facilitar a implantação de um cluster Kubernetes com control plane de controle empilhado ou o uso de um cluster etcd externo sem a necessidade de implantar ferramentas adicionais, como o kops.

 * Load balancing
   * O Kubernetes carrega automaticamente solicitações de balanceamento para serviços de aplicativos dentro de um cluster Kubernetes. No entanto, alguns serviços precisam ser expostos externamente para consumo por clientes externos. O Kubernetes não fornece uma solução de balanceamento de carga pronta para uso para esse tipo de serviço. Uma plataforma de gerenciamento Kubernetes deve incluir uma solução robusta de balanceamento de carga externa ou integrar-se perfeitamente aos balanceadores de carga comerciais existentes.

 * Auditoria centralizada
   * Os usuários devem poder ver o registro cronológico das chamadas que foram feitas para o servidor da API Kubernetes. As entradas do log de auditoria do Kubernetes são úteis para investigar solicitações de API suspeitas, coletar estatísticas ou criar alertas de monitoramento para chamadas de API indesejadas.

 * Provisionamento de autoatendimento
   * Os desenvolvedores devem ter acesso de autoatendimento a um ou mais clusters Kubernetes com níveis adequados de isolamento, para que apenas membros com os privilégios certos possam acessar cargas de trabalho de produção.

 * Gerenciamento privado de registro e imagem
   * Um registro de imagem de contêiner é um serviço como o Docker Hub que armazena imagens de contêiner. Um registro privado permite que você compartilhe suas imagens de base personalizadas dentro da sua organização, mantendo uma fonte de verdade consistente, privada e centralizada para os elementos básicos de sua arquitetura.

 * Atualizações de cluster e gerenciamento de versão
   * Novas versões do Kubernetes estão disponíveis a cada 3 meses. Uma plataforma de gerenciamento Kubernetes deve suportar atualizações contínuas de clusters, de modo que o cluster e a API do cluster estejam sempre disponíveis, mesmo enquanto o cluster estiver sendo atualizado. Além disso, fornecerá a capacidade de reverter para a versão estável anterior em caso de falha.

 * Suporte de armazenamento
   * A integração com o armazenamento de nível corporativo é um componente essencial da execução de clusters Kubernetes na produção. As empresas normalmente desejam que a implantação do Kubernetes se integre às soluções de armazenamento já implementadas (NetApp, EMC etc.) ou que desejam integrar-se a uma tecnologia de armazenamento nativa do contêiner, como Longhorn, OpenEBS, StorageOS ou Portworx.

 * Suporte Arn
   * O suporte a chipsets Arm é particularmente importante ao executar clusters Kubernetes em ambientes com recursos limitados, como dispositivos IoT ou na rede edge.

 * Suporte Airgap
   * Os clusters Kubernetes usados para aplicativos internos podem ser instalados e operados em ambientes com airgapped. Um cluster airgap não tem acesso à Internet de saída e, portanto, não pode extrair as imagens do aplicativo de um registro público do Docker.

 * Backup e restauração do Etcd
   * Para alguns, a idéia de backups para aplicativos sem estado é contra-intuitiva. Mas o estado ainda é necessário para restaurar um nó principal com falha e é especialmente importante se você executar um cluster com apenas um único master.

## Política de segurança e gerenciamento de usuários
 * Active Directory e suporte LDAP
   * Fora da caixa, a autenticação do Kubernetes não é muito fácil de usar para os usuários finais. Uma plataforma de gerenciamento Kubernetes deve integrar-se perfeitamente ao Microsoft Active Directory e outros serviços LDAP comuns para oferecer a experiência de autenticação mais fácil aos usuários finais.

 * Políticas de segurança de pod e rede
   * Uma política de segurança de rede é uma especificação de como os recursos do Kubernetes podem se comunicar entre si e com outros pontos de extremidade da rede. Uma Política de Segurança de Pod (PSP) define regras de segurança com as quais os Pods devem estar em conformidade para serem executados no cluster.

 * Adesão configurável às referências de segurança
   * Os benchmarks do Center for Internet Security (CIS) podem ser usados por administradores de sistema, profissionais de segurança e auditoria e outras funções de TI para estabelecer e manter uma linha de base de configuração segura para o Kubernetes.

 * Políticas RBAC
   * As políticas de controle de acesso baseado em funções (RBAC) são vitais para o gerenciamento correto do seu cluster, pois permitem especificar quais tipos de ações são permitidos, dependendo do usuário e sua função na organização. As políticas RBAC comuns incluem a proteção do cluster concedendo operações privilegiadas (acessando segredos, por exemplo) apenas para usuários administrativos; forçando a autenticação do usuário no seu cluster; e limitar a criação de recursos (como pods, volumes persistentes, implantações) a namespaces específicos ou fazer com que um usuário veja apenas recursos em seu namespace autorizado.

## Ferramentas e serviços compartilhados
 * Catálogo de aplicações
   * O catálogo de aplicativos fornece implantação fácil com um clique para um conjunto de aplicativos pré-empacotados que são executados dentro do Kubernetes. Ele também fornece aos desenvolvedores um veículo para criar e publicar seus próprios aplicativos, para que outras pessoas em sua equipe ou organização possam implantá-los de maneira rápida e confiável. O catálogo de aplicativos permite que as organizações padronizem um conjunto de receitas ou blueprints de implantação de aplicativos, evitando a expansão da configuração e instalações não autorizadas.

 * Provisão com Terraform / Ansible / Outros
   * Terraform e Ansible são ferramentas populares de infraestrutura como código de software que permitem aos usuários definir, provisionar e gerenciar uma infraestrutura de datacenter usando uma linguagem de configuração de alto nível, como YAML ou JSON. O suporte a essas ferramentas significa que as equipes podem trabalhar com sua plataforma de gerenciamento Kubernetes da mesma maneira que o restante de sua infraestrutura.

 * Capacidades de CI / CD
   * Uma das cargas de trabalho mais críticas executadas pelos desenvolvedores é o Continuous Integration e / ou Continuous Delivery. Um pipeline robusto de CI / CD é fundamental para garantir o desenvolvimento ágil e a entrega rápida de novos lançamentos de software para os clientes.

 * Monitoramento avançado
   * Um cluster Kubernetes de produção sempre deve ser monitorado para detectar problemas que podem afetar a disponibilidade do cluster e do aplicativo para os usuários. Uma plataforma de gerenciamento Kubernetes deve fornecer esse recurso imediatamente, com monitoramento avançado disponível por meio de integrações com soluções de monitoramento de cloudnative e de código aberto, como Prometheus e Grafana.

 * Alertas e Notificações
   * Notificações e alertas são os principais pilares da observabilidade no DevOps. Embora o monitoramento e o registro proporcionem uma maneira de obter informações sobre o estado de um cluster Kubernetes, notificações e alertas são usados para informar aos operadores sobre eventos potencialmente problemáticos quando eles ocorrem.

 * Envio de log externo
   * As cargas de trabalho em seus clusters gravam informações nos logs, mas sem um ponto central de agregação, a análise dos dados do log é mais desafiadora. Um cluster eficaz oferecerá suporte ao envio de logs para sistemas externos como Splunk, Logstash ou Fluentd. Esses sistemas permitem uma visão mais ampla de vários fluxos de dados e podem detectar mais facilmente anomalias na imagem maior.

 * Suporte de contêiner do Windows
   * Com inúmeras cargas de trabalho em execução em várias versões, o Windows continua sendo um dos sistemas operacionais mais populares nos datacenters. Se o requisito é criar e desmontar rapidamente ambientes de desenvolvimento ou teste ou elevar e transferir aplicativos herdados para a nuvem, o suporte a contêineres do Windows na plataforma de gerenciamento Kubernetes é um requisito para qualquer empresa que use o Windows na produção.

 * Service Mesh
   * O Service Mesh adiciona tolerância a falhas, implantações de canários, testes A / B, monitoramento e métricas, rastreamento e observabilidade e autenticação e autorização ao Kubernetes. Isso elimina a necessidade de os desenvolvedores criarem códigos personalizados para ativar esses recursos. Os desenvolvedores podem se concentrar em sua lógica de negócios, e todos os aplicativos se beneficiam de uma cadeia de ferramentas padrão para serviços de rede complexos.

 * SLA Corporativo
   * À medida que mais organizações executam seus aplicativos de negócios no Kubernetes, as equipes de operações de TI devem garantir que possam oferecer suporte aos SLAs (acordos de nível de serviço) exigidos pela empresa. Para ajudar os clientes a entender isso, cada fornecedor fornece conhecimento técnico e informações 24/7/365 por meio de alguma forma de assinatura anualizada. Acessibilidade e confiança são variáveis-chave na avaliação de ofertas concorrentes.

 * Comunidade
   * Frequentemente usadas como clima de inovação e maturidade da plataforma, as tecnologias de código aberto mais bem-sucedidas são prontamente adotadas por suas respectivas comunidades e amplamente implementadas.




