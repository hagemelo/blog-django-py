Repositório para entrega Solution Sprint da Fase 4 com foco total em microsserviços, containers, k8s (Kubernets) e OpenShift.

## Grupo 1
#### Alexsander Hage de Melo - @hagemelo
#### Andre Luis de Almeida Melo - @andreluismelo
#### Caio Ricciardi - @caiera2022

# ENTREGAS

  Para a Etapa 1 --> Foi construindo entrega01/, aqui contido, atendendo os critérios solicitados

  Para a Etapa 2 --> Foi construindo infraestrutura/, onde o script de construção do ambiente consta no aquivo MakeFile

  Para a Etapa 3 -->  e HPA cosntra no infraestrutura/MakeFile na instrução criarhpa

  Para a Etapa 4 --> Foi desenvolvido o repositório https://github.com/hagemelo/blog-django-py.git

# CONSTRUÇÃO

## Pré requisitos:
  1 - Install Make:  yum install make

  2 - Install git :  yum install git

## Instruções:

Entrega 01 - Dockerfile
```  
git clone https://github.com/hagemelo/blog-django-py.git
cd entrega01/ 
podman build . 
podman run -dt -p 8080:8080/tcp --name my-running-app localhost/<user>/node-web-app
```

Entregas 2-4 - OpenShift
  
  git clone https://github.com/hagemelo/blog-django-py.git

  cd blog-django-py/infraestrutura

  oc login --token=<token> --server=https://api.na46.prod.nextcle.com:6443

  make build
```

