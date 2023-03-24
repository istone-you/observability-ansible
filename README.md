# ansible-observablity
<img width="600" alt="ansible-observablity.drawio.png" src="ansible-observablity.drawio.png">

PrometheusのNode ExporterとOpenTelemetry、Fluent Bitをサーバーにインストールして、メトリクスとログをそれぞれPrometheusとLokiに送信する設定をするAnsibleのPlaybookです。

roles/fluent-bit/var/main.ymlを作成して以下の変数を指定する必要があります。
- GrafanaLokiUser
- GrafanaLokiPass

roles/opentelemetry/var/main.ymlを作成して以下の変数を指定する必要があります。
- PrometheusEndpoint

