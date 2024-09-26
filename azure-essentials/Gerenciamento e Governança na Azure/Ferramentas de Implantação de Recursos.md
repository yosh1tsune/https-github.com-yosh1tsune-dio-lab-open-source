# Ferramentas de Implantação de Recursos

## Portal

Interface web de gerenciamento, funcional em todos os navegadores modernos. 

## Azure CloudShell

Opções de linha de comando para gerenciamento e criação de recursos.

### Azure PowerShell

Terminal com comandos Windows.

### CLI

Terminal com comandos Linux.

## Azure Arc

Ferramenta multicloud que permite gerenciamento de recursos dentro e fora do Azure, como ambientes de nuvem privada.

- Painel unico de gerenciamento para diversos ambientes de cloud.
- Controle de acesso baseado em função (RBAC).
- Práticas nativas de nuvem.
- Segurança e conformidade.

## Azure Resource Manager

Fornece uma camada de gerenciamento que permite criar, atualizar e excluir recursos. Todas as Ferramentas de Implantação (Portal, CLI, etc.) utilizam os comandos do ARM, direta ou indiretamente para o usuário.

## IaC (Infraestutura como código)

Ferramentas de escrita de código para gerenciamento e criação de recursos.

- Garante consistência na implantação em todo o ecossistema de nuvem.
- Gerencia a configuração em escala.
- Provisiona rapidamente ambientes adicionais com base em uma configuração e um build padrão.

Ex.: Terraforms

## Modelos do ARM

São arquivos JSON que podem ser usados para criar e implantar a insfraestrutura do Azure sem a necessidade de escrever comandos de programação.

- Sintaxe declarativa.
- Resultados repetíveis.
- Orquestração.
- Arquivos modulares.
- Validação integrada.
- Código exportável.
