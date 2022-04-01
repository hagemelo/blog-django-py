PROJECT=group001fiap

criarprojeto:
	oc new-project $(PROJECT)
	oc project $(PROJECT)

criardatabase:
	oc new-app postgresql-persistent --name sample-database --param DATABASE_SERVICE_NAME=sample-database --param POSTGRESQL_USER=sampledb --param POSTGRESQL_PASSWORD=sampledb --param POSTGRESQL_DATABASE=sampledb

criarenv:
	oc set env deployment/blog-django-py-git DATABASE_URL=postgresql://sampledb:sampledb@sample-database:5432/sampledb

criarambiente:
	oc apply -k .

criarhpa:
	oc autoscale deployment/blog-django-py-git --min 1 --max 10 --cpu-percent=80

build: criarprojeto criardatabase criarambiente criarenv criarhpa
	
