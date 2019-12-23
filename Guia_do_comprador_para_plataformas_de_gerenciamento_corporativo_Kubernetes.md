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

