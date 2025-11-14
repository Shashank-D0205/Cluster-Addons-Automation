# Cluster Addons Installer (GitHub Actions + Ansible)

This repo automates installing essential Kubernetes cluster addons using GitHub Actions and Ansible.  
It ensures any new cluster gets a standard baseline setup.

## 🚀 Addons Installed
- Cert-Manager
- ClusterIssuer 
- NGINX Ingress Controller  
- External-DNS    

## ⚙️ How It Works
1. Push to `main` → GitHub Actions workflow triggers.  
2. Workflow prepares an Ansible environment.  
3. Ansible connects to the Kubernetes cluster using kubeconfig from secrets.  
4. Each addon role applies its manifests/Helm charts.


## ▶️ Run Manually
You can run the workflow by going to  
**Actions → Install Cluster Addons → Run Workflow**.


## 📜 License
MIT License
