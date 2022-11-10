`tutorial`(https://levelup.gitconnected.com/how-to-deploy-apache-kafka-with-kubernetes-9bd5caf7694f)
`instruction`(https://github.com/bitnami/charts/tree/main/bitnami/kafka)

helm install kafka bitnami/kafka --set externalAccess.enabled=true,externalAccess.service.type=NodePort,externalAccess.autoDiscovery.enabled=true,serviceAccount.create=true,rbac.create=true,persistence.size=1Gi,externalAccess.service.domain=192.168.99.101,externalAccess.service.ports.external=30204 --namespace=star-bank-ns