PROJECT=group001-fiap

criarprojeto:
	oc new-project $(PROJECT)
	oc project $(PROJECT)

criardatabase:
	oc new-app postgresql-persistent --name sample-database --param DATABASE_SERVICE_NAME=sample-database --param POSTGRESQL_USER=sampledb --param POSTGRESQL_PASSWORD=sampledb --param POSTGRESQL_DATABASE=sampledb

criarambiente:
	oc apply -k kustomization.yml

build: criarprojeto criarambiente criardatabase
	
