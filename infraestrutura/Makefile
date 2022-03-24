PROJECT=group001-fiap

criarprojeto:
	oc new-project $(PROJECT)
	oc project $(PROJECT)

criarambiente:
	oc apply -k kustomization.yml

build: criarprojeto
	criarambiente
	
