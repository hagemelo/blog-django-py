PROJECT=group001_fiap

criarprojeto:
	oc project $(PROJECT)

criarambiente:
	oc apply -k kustomization.yml

build:
	criarprojeto
	criarambiente
	
