Algumas observações sobre subir esse ambiente:

1 - Criação do usuário na AWS console com as devidas permissões e, logo após, executar o comando no terminal:

$ aws configure

2 - O nome do bucket, por questões d eboas práticas, será executado via terminal conforme abaixo:

$ export AWS_DEFAULT_REGION="us-east-1"
$ terraform init -backend-config="bucket=poc-automation-devops" -backend-config="key=terraform-aws.tfstate" -backend-config="region=us-east-1" 
