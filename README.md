# Инфраструктура Kubernetes

Перед применением файла `wordpress-k8s.yaml` обязательно создайте секрет с паролями от базы данных:

\`\`\`bash
kubectl create secret generic db-passwords \
  --from-literal=root-pass="SuperSecretRoot2024" \
  --from-literal=wp-pass="MyAwesomeWP2024"
\`\`\`
