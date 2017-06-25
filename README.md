# Solution B

Deploy in sequence

aws cloudformation create-stack --stack-name adt-solb-network --template-body file://adt-solb-network.json

aws cloudformation create-stack --stack-name adt-solb-database --template-body file://adt-solb-database.json

aws cloudformation create-stack --stack-name adt-solb-webserver --template-body file://adt-solb-webserver.json

aws cloudformation create-stack --stack-name adt-solb-jumpbox --template-body file://adt-solb-jumpbox.json
