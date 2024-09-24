# Gerenciamento de Custos na Azure

## Fatores que afetam os custos

### Tipo de recurso

Os custos são específicos do recurso, portanto, o uso que um medidor rastreia e o número de medidores associados a um recurso, dependendo do tipo de recurso.

Ex.: Máquinas virtuais e bancos de dados tem custos específicos. As famílias de máquinas virtuais tem custos diferentes de acordo com sua especificação, mesmo todas sendo máquinas virtuais.

### Consumo

Com um modelo de pago conforme o uso, o consume é um dos maiores geradores de custos. Modelos de reserva podem ser mais baratos, mas dependem de análise e nem todos os recursos estão disponíveis nesse modelo.

Ex.: Quantidade de tempo em que um recurso fica disponível, quantidade de requisições que recebe, etc.

### Manutenção

Monitorar o seu volume do Azure e manter seu ambiente pode ajudá-lo a identificar e reduzir os custos que não são necessários.

Ex.: Desligar máquinas virtuais que não precisam estar sempre disponíveis.

### Área geográfica

Valores dos mesmos recursos são diferentes em diferentes regiões, especialmente por questões de tributação local.

### Tráfego de rede

Embora algumas transferências de dados de entrada sejam gratuitas, o custo para dados de saída ou dados entre recursos do Azure é afetado por zonas de cobrança.

Ex.: Numa migração de dados locais para nuvem, o tráfego está incluso no preço da migração. Numa migração de dados de uma região para outra, um custo adicional é cobrado.

### Assinatura

O tipo e a configuração da assinatura também pode afetar o custo.

Ex.: A avaliação gratuito permite explorar alguns recursos do Azure gratuitamente.

## Azure Marketplace

Permite que os clientes encontrem, experimentem, comprem e provisionem aplicativos e serviços de centenas de provedores de serviços líderes, que são todos certificados para execução no Azure.

## Cálculo de custos

### Calculadora de preços

Ferramenta que ajuda a estimar o custo dos produtos do Azure.

As opções configuraveis na calculadora variam entre os proutos, mas as opções de configuração básica incluem:

- Região.
- Camada.
- Opções de cobrança.
- Opções de suporte.
- Programas de oferta (clientes grandes podem negociar valores diferentes diretamente com a Microsoft).
- Preço de desenvolvimento/teste.

### Calculadora de Custo Total de Propriedade (TCO)

Ferramenta para estimar a economia de custos possível ao migrar para o Azure.
Um relatório compara os custos das infraestruturas locais com os custos de uso de produtos e serviços do Azure na nuvem.

### Gerenciamento de Custos do Azure

Ferramenta do portal que apresenta relatórios de cobranças e dados sobre os custos. Permite criação de orçamentos, e para este, alertas disparados quando a cobrança atingir um valor fixo informado.
Fornece recomendações sobre melhoria de custos.

## Marcas (Tags)

Informações inseridas nos recursos que ajudam a agrupa-los.
Tags não são obrigatórias nativamente e nem herdaveis, policies podem ser criadas para exigir que os recursos tenha uma tag quando forme criados.

- Fornecem metadados aos recursos do Azure.
- Organizam os recursos em uma taxonomia de maneira lógica.
- Consistem em um par nome-valor.
- Úteis para reunir informações de cobrança.
