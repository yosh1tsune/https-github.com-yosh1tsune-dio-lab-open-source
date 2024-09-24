# Governança e Conformidade

## Azure Policy

Ajuda a impor padrões organizacionais e a avaliar a conformidade em escala. Policies estão acima de qualquer permissionamento.
Fornece governança e consistência de recursos com conformidade regulatória, segurança, custo e gerenciamento.
Não afeta recursos já existentes, apenas recursos criados após a política.

- Avalia e identifica os recursos do Azure que não atendem às suas políticas.
- Fornece definições de políticas e iniciativas integradas, em categorias como armazenamento, rede, computação, central de segurança e monitoramento.

### Modify Effect

Non-compliant: Informa se os recursos já ativos obedecem a política descrita.
Remediation: Permite atualizar configurações que podem entrar no padrão da política descrita.
Compliant: Tudo está dentro do padrão descrito.

Ex.: Uma política de bloqueio da criação de recursos em uma região que a empresa não queira trabalhar. 

## Bloqueios de Recursos

- Protege os recursos de exclusão ou modificação acidental.
- Gerenciados na Assinatura, Grupo de Recursos ou níveis de recursos individuais dentro do Portal do Azure.

Bloqueios são herdáveis.

Tipos de bloqueio:

![image](https://github.com/user-attachments/assets/100759aa-9373-4f6e-8b7e-1d413ebc16ad)

Excluir é o mais recomendado pois em alguns casos a atualização de recursos é necessária, e esse tipo de bloqueio permite isso, por ex.: uma máquina virtual desligada não pode ser religada caso exista um bloqueio ReadOnly.

Mas o ReadOnly também é utilizado, em caso por exemplo de um projeto que esteja pronto e haja a certeza de que seus recursos não precisarão ser modificados.

## Portal de Confiança do Serviço

Portal informativo com as certificações, padrões de serviços e diretrizes da Microsoft. Úteis para consultas em momentos de auditoria.

## Microsoft Purview

É uma família de soluções de governança, risco e conformidade de dados que ajudam a obter uma exibição unificada dos dados. O Purview reúne insights sobre dados locais, multinuvem e de SaaS.
Apresenta os dados e os permissionamentos garantidos para gerenciar dados específicos nos minimos detalhes, como uma linha do banco de dados.
Em caso de um alerta de problemas com algum dado, o Purview oferece a visualização do que aconteceu com aquele dado e por quem foi feita uma possível alteração.

- Descoberta de dados automatizada.
- Classificação de dados confidenciais.
- Linhagem de dados de ponta a ponta.
