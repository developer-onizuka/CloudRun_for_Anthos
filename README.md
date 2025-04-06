# CloudRun_for_Anthos

Cloud Run for Anthos と Cloud Run (fully managed) の違いを簡単にまとめると、Cloud Run for Anthos は Kubernetes（GKE）上で動作する のに対し、Cloud Run (fully managed) は Google Cloud による完全なサーバーレス環境 で動作する。

* 主な違い

| 特徴 |	Cloud Run (fully managed) |	Cloud Run for Anthos |
| :--- | :--- | :--- |
| 実行環境 |	Google Cloudのサーバーレス環境 |	Anthos GKEクラスタ上 |
| 管理方式 | 完全にGoogleが管理 | Kubernetesクラスタ内で管理 |
| スケーリング | リクエストベースで自動スケール | Kubernetesのオートスケーリング機能を利用 |
| ネットワーク | VPCアクセス可能（Serverless VPC Access）| Kubernetesのネットワーク機能を利用 |
| カスタマイズ性 | 限られた設定変更のみ可能 | Kubernetesの柔軟な設定が可能 |
| GPU・カスタムマシンタイプ | 利用不可 | Anthos GKEの機能を活用可能 |
| 用途 | シンプルなサーバーレスアプリ| Kubernetesベースの高度なアプリ |

* どちらを選ぶべきか？<br>
Cloud Run (fully managed) は、シンプルなサーバーレスアプリ をすぐにデプロイしたい場合に最適。<br>
Cloud Run for Anthos は、既存のKubernetes環境を活用しながらサーバーレスの利点を得たい場合 に適している。<br>

もし Kubernetesの管理が不要で、完全なサーバーレス環境を求めるなら Cloud Run (fully managed)、 Kubernetesの柔軟性を活かしながらサーバーレスを導入したいなら Cloud Run for Anthos が適している。
