<h3 align="center">
  Pipeline de Infraestrutura (AWS + Terraform + Github Actions + Multi Env)
</h3>

## Fluxo da Pipeline

<p align="center" width="100%">
    <img width="100%" src="https://github.com/joaoalves-dev/buildrun-infra-terraform-pipeline/blob/main/images/fluxo.png"> 
</p>

<p align="center" width="100%">
    <img width="100%" src="https://github.com/joaoalves-dev/buildrun-infra-terraform-pipeline/blob/main/images/fluxo-detail.png"> 
</p>

## Como começar?
- Crie o Identity Provider do Github em sua conta AWS
- Crie uma IAM Role em sua conta AWS (Permissão mínimia de S3 e DynamoDB)
- Crie um Bucket S3 em sua conta AWS (Habilite o Bucket Versioning)
- Crie uma tabela no DynamoDB na sua conta AWS (PartitionKey com o nome "LockID")
- Clone esse repositório
- Configure os arquivos workflow 
- Pronto! Você já está habilitado para implantar infras na AWS com Terraform via pipeline

### Referências

- [How to connect Github Actions to AWS](https://aws.amazon.com/blogs/security/use-iam-roles-to-connect-github-actions-to-actions-in-aws/)