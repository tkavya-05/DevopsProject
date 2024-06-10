# DevOps Assessment Project

This repository contains the necessary files to deploy a Ruby on Rails application with PostgreSQL using Docker, Kubernetes, ArgoCD, and Tekton.

## Step 1: Docker

1. **Create a Rails application**:
    ```sh
    rails new myapp -d postgresql
    cd myapp
    ```

2. **Dockerize the application**:
    - Create a `Dockerfile`:
      ```Dockerfile
      # Content of Dockerfile
      ```
    - Create a `docker-compose.yml`:
      ```yaml
      # Content of docker-compose.yml
      ```

3. **Build and run containers**:
    ```sh
    docker-compose up --build
    ```

## Step 2: Kubernetes

1. **Create Kubernetes YAML files**:
    - `k8s/postgres-statefulset.yaml`
    - `k8s/rails-deployment.yaml`
    - `k8s/rails-service.yaml`

2. **Deploy to Kubernetes**:
    ```sh
    kubectl apply -f k8s/
    ```

## Step 3: ArgoCD

1. **Install ArgoCD**:
    Follow the [official documentation](https://argo-cd.readthedocs.io/en/stable/getting_started/).

2. **Create ArgoCD application file**:
    - `argocd/application.yaml`

3. **Apply the ArgoCD application**:
    ```sh
    kubectl apply -f argocd/application.yaml
    ```

## Step 4: Tekton

1. **Install Tekton**:
    Follow the [official documentation](https://tekton.dev/docs/getting-started/).

2. **Create Tekton pipeline**:
    - `tekton/pipeline.yaml`

3. **Run the Tekton pipeline**:
    ```sh
    kubectl apply -f tekton/pipeline.yaml
    ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
