# AWS + Gitlab + Vue.js

Deploy automatizado de app frontend Vue.Js com Gitlab CI + AWS S3 e CloudFront.

## AWS: Criar Bucket S3 (Ex: exemplo.meudominio.com.br)
-> Propriedades > Hospedagem de site estático > *Usar este bucket para hospedar um site*
-> Permissões >  Política de Bucket > Editorpolítica de bucket > *Adicionar política*

## AWS: Criar certificado SSL em Certificate Manager
-> Solicitar um certificado público
-> Adicionar DNS ao Route 53

## AWS: Criar Cloudfront
-> Criar distribuição -> Web

## AWS: Route53
-> Criar apontamento Alias (Clodfront) - A

## IAM: Criar usuário com permissão

## Gitlab: Criar arquivo .gitlab-ci.yml
-> Adicionar conteúdo no arquivo

## Gitlab: 
-> Settings -> CI/CD -> Variables -> *Adicionar variáveis*

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- CLOUD_FRONT_ID
- S3_BUCKET_NAME


Este é o processo resumido, para maiores informações consultar documentação.


Referências:
- Using Gitlab CI/CD to Auto Deploy Your Vue.js Application to AWS: https://hackernoon.com/using-gitlab-ci-cd-to-auto-deploy-your-vue-js-application-to-aws-s3-9affe1eb3457
- How to use GitLab CI/CD for Vue.js https://about.gitlab.com/blog/2017/09/12/vuejs-app-gitlab/
