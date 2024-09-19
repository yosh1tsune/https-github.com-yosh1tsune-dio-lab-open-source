# Componentes de Arquitetura do Azure

## Regiões

- Locais espalhados pelo planeta onde o provedor tem datacenters físicos e disponibiliza a criação de recursos.
- Quanto mais perto o serviço estiver do usuário, menor o tempo de delay.
- O preço e a disponibilidade de serviços não é igual para todas as regiões.
- Regiões compostos contam com um ou mais datacenters próximos (geralmente 3); na ocasião de multiplos datacenters, eles se comunicam entre si para manter a região ativa em caso de falha em um deles. Caso todos os datacenters fiquem inátivos, ocorre uma falha de região.
- Fornecem flexibilidade de escala para reduzir a latência do cliente.
- As regiões preservam a residências dos dados com uma oferta abrangente de conformidade.

## Zonas de Disponibilidade

São os datacenters dentro de uma região.

- Fornece proteção contra tempo de invatividade.
- Ideal separar fisicamente os datacenters dentro de uma mesma região.
- Conectados por redes privadas de fibra ótica.

## Pares de regiões

Regiões que são utilizadas como backup uma da outra em caso de indisponibilidade.

- Regiões separadas por no minimo 300 milhas.
- Replicação automatica para alguns serviços.
- Recuperação de região priorizada em caso de reutilização.

## Regiões Soberanas do Azure

Regiões exclusivas, que não são disponibilizadas para clientes comuns.

#### Serviços Governamentais dos EUA

Atende às necessidades de segurança e conformidade das agências federais, governos estaduais e locais dos EUA e seus provedores de soluções.

Azure Governamental:

- Instância separada do Azure
- Fisicamente isolada de implementações que não sejam do governo dos EUA
- Acessível somenta a pessoal verificado e autorizado

#### Azure China

A Microsoft é o primeiro provedor estrangeiro de serviços de nuvem pública da China, em conformidade com as regulamentações governamentais.

- Instância fisicamente separada dos serviços de nuvem do Azure operados pela 21Vianet.
- Todos os dados permanecem dentro da China para garantir conformidade.

## Recursos do Azure

- Máquinas virtuais, serviços de aplicativos, funções, Bancos de Dados, redes virtuais, etc.

## Grupos de Recursos

É um contêiner utilizado para agrupar e gerenciar recursos.

- Todos os recursos criados no Azure precisam estar dentro de um Grupo de Recursos. Utilizado para organizar recursos que se relacionam ou recursos do mesmo tipo, de acordo com o decidido pelo cliente.
- Recursos podem existir apenas em um Grupo.
- Recursos podem ser migrados para outros Grupos, mas Grupos não podem ser renomeados.
- Recursos não precisam estar na mesma Região para estarem no mesmo Grupo.
- Aplicativos podem consumir recursos de diversos Grupos de Recursos.

## Assinaturas do Azure

- Agrupamento de recursos para cobrança.
- Uma conta pode ter diversas Assinaturas, mas uma Assinatura é relacionada a apenas uma conta.
- Cada Assinatura tem uma Conta de Cobrança individual, que responde pelos recursos criados sob aquela Assinatura. Ideal para organizar o orçamento.
- Fornece acesso autenticado e autorizado às contas do Azure. Define limites de cobrança, e controle de acesso aos recursos.

## Grupos de Gerenciamento

- Grupos que englobam as Assinaturas.
- Grupos de Gerenciamento podem incluir várias Assinaturas.
- Assinaturas herdam as condições aplicadas ao Grupo de Gerenciamento.
