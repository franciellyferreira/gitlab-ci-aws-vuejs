# AWS + Gitlab + Vue.js

Deploy automatizado de app frontend Vue.Js com Gitlab CI + AWS S3 e CloudFront.

## AWS: Criar Bucket S3 (Ex: exemplo.meudominio.com.br)
- Propriedades > Hospedagem de site estático > *Usar este bucket para hospedar um site*
- Permissões >  Política de Bucket > Editorpolítica de bucket > *Adicionar política*

## AWS: Criar certificado SSL em Certificate Manager
- Solicitar um certificado público
- Adicionar DNS ao Route 53

## AWS: Criar Cloudfront
- Criar distribuição -> Web

## AWS: Route53
- Criar apontamento Alias (Clodfront) - A

## IAM: Criar usuário com permissão

## Gitlab: Criar arquivo .gitlab-ci.yml
- Adicionar conteúdo no arquivo

## Gitlab: 
- Settings -> CI/CD -> Variables
- Adicionar variável: AWS_ACCESS_KEY_ID
- Adicionar variável: AWS_SECRET_ACCESS_KEY
- Adicionar variável: CLOUD_FRONT_ID
- Adicionar variável: S3_BUCKET_NAME


* Espero que este código seja útil.
* Para maiores informações consultar documentação.


## Referências:
- Using Gitlab CI/CD to Auto Deploy Your Vue.js Application to AWS: https://hackernoon.com/using-gitlab-ci-cd-to-auto-deploy-your-vue-js-application-to-aws-s3-9affe1eb3457
- How to use GitLab CI/CD for Vue.js https://about.gitlab.com/blog/2017/09/12/vuejs-app-gitlab/
