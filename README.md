# Desafio_CodeGirl_AWS CloudFormation
AWS CloudFormation — Resumo Code Girl

## O que é o CloudFormation?
O AWS CloudFormation é um serviço que permite criar, atualizar e gerenciar recursos AWS usando templates (YAML ou JSON).  Em vez de criar tudo manualmente na console, descrevemos a infraestrutura em arquivo e o CloudFormation monta tudo para nós. Isso é Infraestrutura como Código (IaC).


## Quando usar?
Utilizamos CloudFormation quando queremos:

- automatizar criação de infraestrutura
- padronizar ambientes (dev / stage / prod)
- evitar diferenças “manuais” entre ambientes
- versionar a infraestrutura junto com o código
- facilitar a replicação de ambientes



## Benefícios
- cria ambientes reprodutíveis
- facilita versionamento com Git
- facilita rollback (voltar versão se algo der errado)
- ideal para ambientes complexos (muitos serviços envolvidos)
- melhora governança e padronização



##  Como funciona o template?
O template é um arquivo declarativo. Nele descrevemos o que queremos que exista, e o CloudFormation:

1) lê o template  
2) compara com o que já existe  
3) cria / atualiza / remove o que for necessário

   Template é o plano, Stack é o resultado.

   



## 📚Conceitos importantes do CloudFormation

Template: Arquivo (YAML/JSON) que descreve os recursos e configurações.

Stack: Resultado da execução de um template, é o “conjunto” de recursos criados.

Resource: Cada item criado pelo template (S3, Lambda, DynamoDB, VPC, etc). 

Parameter: Valores dinâmicos que podemos passar para o template (ex: nome de bucket, tamanho de instância). 

Output: Informações que o template devolve após a criação (ex: URL de um bucket).

Change Set: Prévia das mudanças antes de aplicar. Isso ajuda a evitar erro e prever impactos. 





