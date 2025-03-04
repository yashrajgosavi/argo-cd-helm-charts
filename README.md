# argo-cd-helm-charts


kubectl apply -f release/root-apps/product-test.yaml -n argocd

kubectl delete -f release/root-apps/product-test.yaml -n argocd



kubectl apply -f release/root-apps/product-prod.yaml -n argocd

kubectl delete -f release/root-apps/product-prod.yaml -n argocd



kubectl apply -f release/rolebinding/product-test-rb.yaml

kubectl delete -f release/rolebinding/product-test-rb.yaml

kubectl get rolebinding product-test-rb -n product-test



kubectl apply -f release/rolebinding/product-prod-rb.yaml

kubectl delete -f release/rolebinding/product-prod-rb.yaml

kubectl get rolebinding product-prod-rb -n product-prod




kubectl port-forward svc/argocd-server -n argocd 8080:443

kubectl port-forward svc/selenoid-grid -n argocd 4444:443