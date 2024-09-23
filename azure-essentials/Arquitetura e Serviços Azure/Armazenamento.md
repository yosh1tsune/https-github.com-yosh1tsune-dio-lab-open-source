# Armazenamento

## Contas de Armazenamento

- Precisam ter um nome globalmente exclusivo.
- Fornecer acesso à internet em todo o mundo.
- Determinar os serviços de armazenamento e as opções de redundância.

## Redundância de Armazenamento

Quantidade de disponibilidade das contas de armazenamento.

LRS (redundância local): Cópias apenas em um datacenter da região primária.

ZRS (redundância de zona): Cópias em três zonas de disponibilidade da região primária.

GRS (redundância geográfica): Cópias em uma zona nas regiões primária e secundária.

GZRS (redundância de zona geográfica): Cópias em três zonas na região primária e uma zona na região secundária.

As cópias são feitas de forma assíncrona, ou seja, não são escritas em todas as zonas no mesmo tempo. As cópias não são feitas para serem diretamente consumidas, apenas em caso de indisponibilidade na zona principal.

## Serviços de Armazenamento do Azure

### Blob

Otimizado para armazenamento de quantidades massivas de dados não estruturados, como texto ou dados binários.

### Disco do Azure

Fornece discos para máquinas virtuais, aplicativos e outros serviços acessarem e utilizarem.

### Fila do Azure

Serviço de armazenamento de mesnsagens que fornece armazenamento e recuperação para grandes quantidade de mensagens, cada uma con até 64 KB.

### Arquivos do Azure

Configura um compartilhamento de arquivos de rede altamente disponível que pode ser utilizano usando o protocolo Bloco de Mensagens de Servidor.

### Tabelas do Azure

Fornece uma opção de chave/atributo para o armazenamento de dados estruturados relacionais com um design sem esquema.

## Pontos de Extremidades Públicos do Serviço de Armazenamento

Endereço público das camadas de armazenamento (URL).

Exemplo de URL: https://<storage-account-name>.<service>.core.windows.net

## Camadas de Acesso do Armazenamento

Frequenta: Otimizado para armazenamento de dados acessador com frequência. Custo maior por armazenamento e menor por consulta.

Esporádico: Otimizado para armazenamento de dados acessador com poca frequência e armazenados por pelo menos 30 dias. Custo menor por armazenamento e maior por consulta.

Frio: Otimizado para armazenamento de dados acessador com poca frequência e armazenados por pelo menos 90 dias. Custo menor por armazenamento e maior por consulta.

Arquivo Morto: Otimizado para armazenamento de dados acessador com poca frequência e armazenados por pelo menos 180 dias com requisitos de latência flexíveis. Direcionado para camadas de backup. Custo menor por armazenamento e maior por consulta.

## Migrações para o Azure

Utilizado para migração de arquivos em nuvem privada para nuvem pública.

- Plataforma de migração unificada.
- Intervalo de ferramentas integradas e autônomas.
- Avaliação e migração.

### Azure Data Box

Serviço de migração física para altos volumes de dados, que não seriam viáveis movimentar via internet. Capaz de armazenar até 80TB e utilizado para transmitir dados a partir de 40TB. Os dados ficam totalmente criptografados e são transportados em uma "caixa robusta" até o data center.

### AzCopy

- Utilitário de CLI.
- Copiar blobs ou arquivos de OU para sua conta de armazenamento.
- Sincronização em uma direção (da origem para o serviço).

### Gerenciador de Armazenamento do Azure

Interface gráfica familiar para usuários sem experiência com CLI. Por trás utiliza os mesmos comandos do AzCopy.

- Interface gráfica semelhante ao Windows Explorer.
- Compátivel com Windows, MacOS e Linux.

### Sincronização de Arquivos do Azure.

Ideal para servidores locais que ainda estão em utilização, mas necessitam reduzir a sobrecarga.

- Sincroniza os arquivos do Azure e locais de forma bidirecional.
- A camada de nuvem mantém os arquivos acessador com frequência no local.

