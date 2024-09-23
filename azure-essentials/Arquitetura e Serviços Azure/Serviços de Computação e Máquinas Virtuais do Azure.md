# Computação e Rede

# Serviços de Computação do Azure

Serviços sob demanda que fornecem recursos de computação, como discos, processadores, memória, rede e SOs.

Ex.: Máquinas Virtuais, Serviços de Aplicativos, Instâncias de Conteiners, AKS, Área de Trabalho Virtual.

## Máquinas Virtuais

Emulaões de software de computadores físicos. Incluem processador virtual, memória, armazenamento e rede. É uma oferta de IaaS que oferece personalização e controle total.

#### Conjuntos de Dimensionamento de VMs

Oferecem oportunidade de balanceamento de carga para dimensionar os recursos automaticamente: disponibiliza VMs identicas e distribui as requisições entre elas.

#### Conjuntos de Disponibilidade de VMs

Máquinas virtuais distribuidas em vários dominios de falha (racks), idealmente pelo menos 3 racks diferentes. Também existe a denominação "dominio de atualização" que são grupos de máquinas relacionadas que podem ser reiniciadas juntas.

## Área de Trabalho Virtual

Virtualização da área de trabalho, utilizando um sistema Windows (atualmente 10 ou 11) hospedado em nuvem em que o usuário pode acessar como um desktop local.
Aumenta a agilidade no acesso de usuários, pulando a etapa de envio e uso de um hardware físico.

## Serviços de Conteinêres do Azure

Fornecem um ambiente leve e virtualizado que não exige o gerenciamento do SO e pode responder a alterações sob demanda. Compatível com Docker, que é o lider de mercado de conteinerização atualmente.

#### Instâncias de Contêiner do Azure

Oferta de PaaS que executa um contêiner ou pod de contêineres no Azure.

#### Aplicativos de Contêiner do Azure

Oferta de PaaS, como instâncias de contêiner, que pode balancear e escalar carga. Não necessita do gerenciamento dos contêineres.

#### AKS (Serviço de Kubernetes do Azure)

Orquestração de contêineres utilizando Kubernetes para contêineres com arquitetura distribuida e grandes volumes de contêineres.

## Azure Functions

Oferta de PaaS. Operações serverless executadas através de requisições REST. A função é dimensionada baseada em demanda e não demanda infraestrutuas de servidor enquanto estiver inativa. Execução baseada em eventos.

## Comparação das opções de computação do Azure

Máquinas Virtuais:

- Servidor baseado em nuvem que da suporte a ambientes Windows ou Linux.
- Util para migrações.
- Pacote completo do SO, incluindo o SO do host.

Área de Trabalho Virtual:

- Experência de área de trabalho do Windows hospedada em Nuvem.
- Aplicativos dedicados para conexão e uso ou acessíveis em qualquer navegador.
- Controle de acesso e permissões.
- Logon de vários usuários no mesmo computador ao mesmo tempo.

Comtêineres:

- Ambientes leves, adequados para execução de microsserviços.
- Projetado para escalabilidade.

## Serviços de Aplicativo do Azure

Criar, implantar e dimensionar aplicativos Web e APIs rapidamente. Trabalha com diversas linguagens. PaaS com nível comportativo de desempenho, segurança e conformidade.

## Serviços de Rede do Azure

A VNet permite a conunicação entre os recursos dentro do Azure.
Pontos de extremidade públicos: acessíveis de qualquer lugar da internet. Pontos de extremidade privados: acessíveis apenas dentro da rede.
Para conexão entre duas VNets é necessário um emparelhamento.
Tomar cuidado com o overlapping.

#### Gateway de VPM

Usado para enviar tráfego criptografado entre uma VNet e uma rede local pela internet pública. Muito útil para modelos de nuvem híbrida.

#### ExpressRoute

Conexão cabeada entre o cliente e o Data Center da nuvem pública.

#### DNS

Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS usando a rede Anycast.
A segurança baseia-se no gerenciador de recursos do Azure, habilitando ol controle de acesso baseado em função e o monitoramente e registro em log.
Facilidade de uso para gerenciar recursos externos com um único serviço DNS.
Redes virtuais personalizáveis permitem o uso de nomes de domínio privados e totalmente personalizado nas VNet privadas.
