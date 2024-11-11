# Fake Shop


## Variável de Ambiente
DB_HOST	=> Host do banco de dados PostgreSQL.

DB_USER => Nome do usuário do banco de dados PostgreSQL.

DB_PASSWORD	=> Senha do usuário do banco de dados PostgreSQL.

DB_NAME	=>	Nome do banco de dados PostgreSQL.

DB_PORT	=>	Porta de conexão com o banco de dados PostgreSQL.

Aula 05 - Prometheus e Grafana

Arquivo de manifesto para o Prometheus e o Grafana:

https://gist.githubusercontent.com/fabricioveronez/3ffbc3ddf826a75c508d5bca9b5a6adb/raw/8677f2ac7a3d9df2d43f63213b936e2a6248592c/deploy-prometheus.yaml

Arquivo com o Flask Dashboard:

https://gist.githubusercontent.com/fabricioveronez/3ffbc3ddf826a75c508d5bca9b5a6adb/raw/8677f2ac7a3d9df2d43f63213b936e2a6248592c/flask-dashboard.json

Comando para obter a senha do Grafana:

kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo


