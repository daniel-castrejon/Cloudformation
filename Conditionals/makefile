empty: 
	@echo ""


delete-staging:
	aws cloudformation delete-stack --stack-name staging-conditionals
deploy-staging:
	aws cloudformation deploy --stack-name staging-conditionals --template-file stack-conditionals.yaml --parameter-overrides VpcIdParameter=vpc-48bbd723 KeyPairParameter=keypair_personal_dcm AmiIdParameter=ami-024e6efaf93d85776 Enviroment=staging



delete-prod:
	aws cloudformation delete-stack --stack-name prod-conditionals
deploy-prod:
	aws cloudformation deploy --stack-name prod-conditionals --template-file stack-conditionals.yaml --parameter-overrides VpcIdParameter=vpc-48bbd723 KeyPairParameter=keypair_personal_dcm AmiIdParameter=ami-024e6efaf93d85776 Enviroment=prod
