# Argo CD and Helm Practice

This repository contains Helm charts and configurations for practicing Kubernetes deployments with Argo CD and Helm.

#### Purpose
- Learn and experiment with Argo CD for continuous delivery.
- Create and manage Kubernetes applications using Helm charts.
- Test various deployment scenarios and best practices.

#### Structure
- /charts: Contains custom Helm charts for Kubernetes deployments.
- /manifests: Kubernetes YAML manifests for experimentation.
- /argo: Argo CD configuration files, including Application definitions.

#### Prerequisites
- Helm installed on your local machine.
- Argo CD set up on a Kubernetes cluster.

## Getting Started
1. Clone the repository:
```bash
git clone https://github.com/dshmmd/helmargo-lab.git
cd helmargo-lab
```

2. Add this repository to Argo CD:
```bash
argocd repo add https://github.com/dshmmd/helmargo-lab.git --username <username> --password <password>
```

3. Deploy a Helm chart:
```bash
helm install my-app ./charts/my-chart
```

4. Sync with Argo CD:
```bash
argocd app sync my-app
```

#### Contributing
Feel free to open issues or submit pull requests to improve the repository!

#### License
This repository is licensed under the MIT License.
