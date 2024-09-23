# Identidade, Acesso e Segurança

## Microsoft Entra ID (Active Directory)

Serviço de gerenciamento de identidades e acesso baseado em nuvem do Azure.

- Autenticação (os funcionários entram para acessar os recursos).
- Login único (SSO).
- Gerenciamento de aplicativos.
- Negócios para Negócios (B2B).
- Gerenciamento de dispositivos.

### Domain Services

- Benefícios dos serviços baseados em nuvem sem gerenciar os controladores de domínio.
- Execute aplicativos herdados (que não podem utilizar os padrões de autenticalção mordernos) na nuvem.
- Sincronizar automaticamente a partir do Microsoft Entr ID.

## Autenticação

- Identifica a pessoa ou serviço buscando acesso a um recurso.
- Solicita credenciais de acesso legítimo.
- Base para criar princípios de identidade e controle de acesso seguros.

## Autorização

- Determina o nível de acesso de uma pessoa ou serviço autenticado.
- Define quais dados eles podem acessar e o que podem fazer com eles.

## Autenticação Multifator

Fornece segurança adicional para as identidades, exigindo dois ou mais elementos para autenticação completa.

## B2B do Microsoft Entra External ID

Parceiros, fornecedores ou outros colaboradores convidados a acessar o ambiente.

## B2C do Indentidades Externas do Azure AD

Consumidores do aplicativo publicado. Ex.: OAuth.

## Acesso Condicional

Monitora mais detalhadamente se a requisição de login segue um padrão apresentado anteriormente. Por exemplo, uma conta que loga sempre em um país recebe uma requisição de login de um país diferente e distante gera um aviso e possível bloqueio.

Fatores considerados:

- Associação de usuário ou grupo.
- Local do IP.
- Dispositivo.
- Aplicativo.
- Detecção de Risco.

## Controle de acesso baseado em função (RBAC)

- Gerenciamento de acesso de granularidade fina (conceder acesso somente e conforme o necessário).
- Divida as tarefas dentro da equipe e conceda somenta a quantidade de acesso de que os usuários precisam para trabalhar.
- Habilite o acesso ao portal do Azure e o controle de acesso aos recursos.

## Confiança Zero

- Restringir ao máximo o acesso aos recursos, pressupondo sempre que algo pode ser violado.
- Utiliza várias camadas de segurança.

## Proteção Completa

- Abordagem em camadas para proteger sistemas de computador.
- Fornece vários níveis de proteção.
- Ataques contra uma camada são isolados das camadas subsequentes.

## Microsoft Defender para Nuvem

É um Serviço de monitoramente que fornece proteçã contra ameaças nos datacenters do Azure e locais. Também funciona com outros providers como AWS e GCP.
