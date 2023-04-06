# ansible-observability
<img width="600" alt="ansible-observability.drawio.png" src="ansible-observability.drawio.png">

PrometheusのNode ExporterとOpenTelemetry、Fluent Bitをサーバーにインストールして、メトリクスとログをそれぞれPrometheusとLokiに送信する設定をするAnsibleのPlaybookです。

roles/node-exporter/var/main.ymlを作成して以下の変数を指定する必要があります。
- node_exporter_version
- prometheus_textfile_directory

roles/fluent-bit/var/main.ymlを作成して以下の変数を指定する必要があります。
- loki_user
- loki_passwd

roles/opentelemetry/var/main.ymlを作成して以下の変数を指定する必要があります。
- prometheus_endpoint
- otel_version

