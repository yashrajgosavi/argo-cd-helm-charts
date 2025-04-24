# argo-cd-helm-charts


kubectl apply -f release/root-apps/test.yaml -n argocd

kubectl delete -f release/root-apps/test.yaml -n argocd



kubectl apply -f release/root-apps/prod.yaml -n argocd

kubectl delete -f release/root-apps/prod.yaml -n argocd



kubectl apply -f release/rolebinding/test-rb.yaml

kubectl delete -f release/rolebinding/test-rb.yaml

kubectl get rolebinding test-rb -n test



kubectl apply -f release/rolebinding/prod-rb.yaml

kubectl delete -f release/rolebinding/prod-rb.yaml

kubectl get rolebinding prod-rb -n prod




kubectl port-forward svc/argocd-server -n argocd 8080:443

kubectl port-forward svc/selenoid-grid -n argocd 4444:443