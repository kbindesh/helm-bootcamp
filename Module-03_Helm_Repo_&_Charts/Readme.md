# Helm Repo and Helm Charts

## 01. Helm Repo

#### 1.1 List Helm Repo

```
# List Helm Repo
helm repo list
```

#### 1.2 Add a Helm Repo

```
# Add helm repo - Syntax
helm repo add <repo_name> <repo_url>

# Add helm repo - Example
helm repo add bitnami https://charts.bitnami.com/bitnami
```

#### 1.3 Search Chart in a Repo

```
# Search a apache helm chart in bitnami Repo
helm search repo apache

# Search a mysql helm chart in bitnami Repo
helm search repo mysql

# Search all the versions of a particular helm chart (e.g. mysql)
helm search repo mysql --versions
```

#### 1.5 Remove a Helm Repo

```
# Syntax - Delete helm repo
helm repo remove <repo_name>

# Example - Delete helm repo
helm repo remove bitnami
```

## 02. Helm Charts
