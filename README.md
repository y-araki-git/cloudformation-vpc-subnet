# CloudFormationでVPC,Subnet自動設定

AWSアカウントを多く発行する環境では、ネットワーク構成に規則を決めて
自動で構築すると運用面でもよいと思います。

以下内容でVPC、サブネットを作成するCloudFormationのサンプルです。

  - VPCセグメントが10.XXX.0.0/16' ※対話形式で設定
  - アカウント
  - Dev,Prdに分けてVPCセグメントを作成
  - 更にap-northeast-1a,ap-northeast-1cにひとつずつパブリックサブネットを作成
  - 最初にアカウント名を対話形式で入力。testと入力した場合、prd-test-vpcなどと反映される。

※最下部SSHの設定で許可したいIPを修正してください。
