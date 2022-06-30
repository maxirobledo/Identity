Deployment example
https://github.com/peterzandbergen/keycloak-kubernetes

HELM Install
Add helm chart
helm repo add codecentric https://codecentric.github.io/helm-charts
Update helm chart
helm repo update
Download values.yml
https://github.com/codecentric/helm-charts/blob/master/charts/keycloak/values.yaml
Install 
helm install keycloak codecentric/keycloak --values values.yaml
 
Keycloak Apps configuration
client-id=oauth2-proxy
client-secret=86Bm84a8ITX6JTiGJtNCR0YXYn4vbgyQ
URL callback: https://test.snappypreview.com/oauth2/callback

Apps set-up
helm repo add bitnami https://charts.bitnami.com/bitnami
helm upgrade --install my-release bitnami/nginx -f values.yaml

Source research
https://www.talkingquickly.co.uk/installing-keycloak-kubernetes-helm
https://www.talkingquickly.co.uk/webapp-authentication-keycloak-OAuth2-proxy-nginx-ingress-kubernetes
https://www.youtube.com/watch?v=0TiRsueDmO4
