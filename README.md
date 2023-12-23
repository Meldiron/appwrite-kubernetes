# 📦 Appwrite Kubernetes

## ⚡ Running

1. `brew install kubectl`
2. `brew install minikube`
3. `minikube start`
4. `minikube addons enable ingress`
5. `minikube tunnel -c` (run in background)
6. `kubectl create namespace appwrite`
7. `cd kubernetes && kubectl apply -R -f .`

> To wipe, do `minikube stop && minikube delete && minikube start`

---

TODO:

- New Usage worker
- Proper commands for mysql deploy
- Proper commands for redis deploy
- Proper commands for api (appwrite) deploy
- Add traefik
- Ensure traefik certificates works, ensure traefik labels works
- Add Open Runtimes Executor & Open Runtimes Proxy
- Ensure function builds and executions work
- Ensure custom domains work, with wildcard certificate
- Ensure local Storage works, large files too

QA:

- All Appwrite tests must run and pass
- Deploy to DigitalOcean and do manual QA