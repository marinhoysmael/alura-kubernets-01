# Curso de Kubernetes: Pods, Services e ConfigMaps

## Faça esse curso de Containers e:
* Conheça a arquitetura Kubernetes
* Saiba como o Kubernetes gerencia os containers
* Use e gerencie os famosos Pods com o kubectl
* Entenda os tipos de serviço e exponha seus Pods
* Defina variáveis de ambiente utilizando ConfigMaps

## Comandos kubectl:

iniciar kubernetes: $ minikube start

listar IPs do minikube: $ kubectl get nodes -o wide
### pods
criar ou atualizar um pod: $ kubectl apply -f <nome do arquivo yaml>

mostrar configuracao do pod: $ kubectl describe pod <nome do pod>

listar pods: $ kubectl get pods

entrar no terminal de comando de um pod: kubectl exec -it <nome do pod> -- bash

deletar pod pelo arquivo: $ kubectl delete -f <nome do arquivo yaml>
deletar pode pelo nome: $ kubectl delete pod <nome do pod>
deletar todos os pods: $ kubectl delete pods --all

### services:

criar ou atualizar um serviço: $ kubectl apply -f <nome do service>

listar servicos: $ kubectl get service


deletar todos os serviços: $ kubectl delete svc --all
## Doc:
SVC:
	ClusterIP
		"Apenas para comunicação interna"
	NodePort
	LoadBalancer
	"Serviços funcionam unilateralmente"

