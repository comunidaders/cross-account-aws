# Modelo Cross-Account na AWS

## O que é o Modelo Cross-Account?

O modelo cross-account na AWS é uma prática de usar **múltiplas contas AWS** para segmentar recursos, gerenciar permissões e isolar ambientes para diferentes propósitos ou estágios do ciclo de desenvolvimento de software. Esta estratégia divide os recursos e operações em várias contas, cada uma com seu próprio conjunto de permissões, políticas e limites.

## Importância do Modelo Cross-Account

### 1. Isolamento de Ambientes
- **DEV**, **HML**, **PRD** são diferentes estágios do desenvolvimento.
- Cada estágio tem requisitos únicos de configuração, acesso e permissões.
- Contas separadas permitem isolamento, reduzindo riscos de alterações indevidas.

### 2. Segurança e Controle de Acesso
- Aplica políticas de segurança e IAM específicas para cada ambiente.
- Minimiza o risco de acesso indevido.
- Garante permissões apropriadas para cada usuário.

### 3. Gerenciamento de Custos e Faturamento
- Facilita o rastreamento e gerenciamento de custos por ambiente.
- Ajuda na alocação de custos, orçamento e otimização de recursos.

### 4. Flexibilidade e Escalabilidade
- Cada ambiente pode ser otimizado individualmente.
- Permite escalabilidade mais eficiente para cada fase do desenvolvimento.

### 5. Simplificação de Compliance e Auditoria
- Facilita a implementação de controles de compliance.
- Simplifica o processo de auditoria para regulamentações específicas.

### 6. Desastre e Recuperação
- Limita o impacto de falhas a apenas uma conta.
- Facilita a recuperação e reduz riscos em operações críticas.

## Implementação do Modelo Cross-Account

- Criação de uma conta central (gerenciamento ou "master").
- Acesso às outras contas (DEV, HML, PRD) através de roles do IAM.
- Administração centralizada com separação e isolamento de ambientes.

## Diagrama do modelo
![Diagrama](https://github.com/comunidaders/cross-account-aws/blob/main/Diagrama.png)



O modelo cross-account na AWS oferece uma abordagem robusta e flexível para gerenciar múltiplos ambientes na nuvem, melhorando a segurança, eficiência e a gestão de recursos e operações de TI.
