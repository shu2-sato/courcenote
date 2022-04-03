## 1. **AZ-500**

**リンク一覧およびメモ**

- [AZ-500 ラボコンテンツ](https://microsoftlearning.github.io/AZ-500JA-AzureSecurityTechnologies/)
    - [ラボファイルをローカルにダウンロードする](https://github.com/MicrosoftLearning/AZ-500JA-AzureSecurityTechnologies/archive/master.zip)

- [トレーニングで使用するテキスト](https://docs.microsoft.com/ja-jp/users/msftofficialcurriculum-4292/collections/neqjf5m83e37x4?wt.mc_id=esi_m2l_content_wwl)

- [ラボ環境準備　PDF](pdf/ラボ環境準備.pdf)
    - InPrivte モードでブラウザを起動
    - [Microsoftアカウント作成](https://signup.live.com/?lic=1)
    - [LODS](https://esi.learnondemand.net/User/Login?ReturnUrl=%2F)
    - トレーニングコードは、講師から案内があります。
    - AzurePass サブスクリプションはラボ環境からアクティベートします。

- [support使用法](pdf/support.pdf)

## 1.1. モジュール01
- [Azure Active Directory の価格](https://www.microsoft.com/ja-jp/security/business/identity-access-management/azure-ad-pricing?rtc=1)
- [自己管理型の Active Directory Domain Services、Azure Active Directory、およびマネージド Azure Active Directory Domain Services の比較](https://docs.microsoft.com/ja-jp/azure/active-directory-domain-services/compare-identity-solutions)
- [Azure AD の組み込みロール](https://docs.microsoft.com/ja-jp/azure/active-directory/roles/permissions-reference)
  
**HybridID**
- [Azure AD Connect とは](https://docs.microsoft.com/ja-jp/azure/active-directory/hybrid/whatis-azure-ad-connect)
- [Azure AD Connect クラウド同期とは](https://docs.microsoft.com/ja-jp/azure/active-directory/cloud-sync/what-is-cloud-sync)
- [Azure Active Directory ハイブリッド ID ソリューションの適切な認証方法を選択する](https://docs.microsoft.com/ja-jp/azure/active-directory/hybrid/choose-ad-authn)
- [チュートリアル:オンプレミス環境への Azure Active Directory のセルフサービス パスワード リセットのライトバックを有効にする](https://docs.microsoft.com/ja-jp/azure/active-directory/authentication/tutorial-enable-sspr-writeback)
  
**Identity** **Protection**
- [Identity Protection とは](https://docs.microsoft.com/ja-jp/azure/active-directory/identity-protection/overview-identity-protection)
- [動作のしくみ: Azure AD Multi-Factor Authentication](https://docs.microsoft.com/ja-jp/azure/active-directory/authentication/concept-mfa-howitworks)
- [条件付きアクセスとは](https://docs.microsoft.com/ja-jp/azure/active-directory/conditional-access/overview)
- [Azure AD アクセス レビューとは](https://docs.microsoft.com/ja-jp/azure/active-directory/governance/access-reviews-overview)
- [Azure AD のセキュリティの既定値群](https://docs.microsoft.com/ja-jp/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

**PIM**
- [Security best practices for Azure solution](https://azure.microsoft.com/mediahandler/files/resourcefiles/security-best-practices-for-azure-solutions/Azure%20Security%20Best%20Practices.pdf)
- [Azure Policy とは](https://docs.microsoft.com/ja-jp/azure/governance/policy/overview)
- [Azure Blueprint とは](https://docs.microsoft.com/ja-jp/azure/governance/blueprints/overview)

**memo**
- [AZ-500 Azure ADまとめ](pdf/AZ-500%20Azure%20ADまとめ.pdf)
- [Azure AD Connect](pdf/Azure%20AD%20Connect.pdf)

## 1.2. モジュール02

**境界セキュリティ**
- [Azure DDoS Protection Standard の概要](https://docs.microsoft.com/ja-jp/azure/ddos-protection/ddos-protection-overview)
- [Azure Firewall に関する FAQ](https://docs.microsoft.com/ja-jp/azure/firewall/firewall-faq)
- [強制トンネリングについて](https://docs.microsoft.com/ja-jp/azure/vpn-gateway/vpn-gateway-forced-tunneling-rm)
- [チュートリアル: Azure portal を使用して Azure Firewall とポリシーをデプロイして構成する](https://docs.microsoft.com/ja-jp/azure/firewall/tutorial-firewall-deploy-portal-policy)
- [Azure Firewall Manager とは](https://docs.microsoft.com/ja-jp/azure/firewall-manager/overview)

**NetworkSecurity**

- [ネットワーク セキュリティ グループ](https://docs.microsoft.com/ja-jp/azure/virtual-network/network-security-groups-overview)
- [アプリケーション セキュリティ グループ](https://docs.microsoft.com/ja-jp/azure/virtual-network/application-security-groups)
- [仮想ネットワーク サービス エンドポイント](https://docs.microsoft.com/ja-jp/azure/virtual-network/virtual-network-service-endpoints-overview)
- [Azure Private Link とは](https://docs.microsoft.com/ja-jp/azure/private-link/private-link-overview?toc=/azure/virtual-network/toc.json)
- [サービス エンドポイント](https://docs.microsoft.com/ja-jp/azure/virtual-network/vnet-integration-for-azure-services#compare-private-endpoints-and-service-endpoints)
- [Azure Application Gateway とは](https://docs.microsoft.com/ja-jp/azure/application-gateway/overview)
- [Azure Web アプリケーション ファイアウォールとは](https://docs.microsoft.com/ja-jp/azure/web-application-firewall/overview)
- [Azure Front Door とは](https://docs.microsoft.com/ja-jp/azure/frontdoor/front-door-overview)
- [Azure ExpressRoute とは](https://docs.microsoft.com/ja-jp/azure/expressroute/expressroute-introduction)
- [ExpressRoute 接続モデル](https://docs.microsoft.com/ja-jp/azure/expressroute/expressroute-connectivity-models)
- [ExpressRoute Direct について](https://docs.microsoft.com/ja-jp/azure/expressroute/expressroute-erdirect-about)
- [ExpressRoute の暗号化](https://docs.microsoft.com/ja-jp/azure/expressroute/expressroute-about-encryption)
  
**HOSTSecurity**
- [特権アクセス ストーリーの一部としてのデバイスのセキュリティ保護](https://docs.microsoft.com/ja-jp/security/compass/privileged-access-devices)
- [Azure Bastion とは](https://docs.microsoft.com/ja-jp/azure/bastion/bastion-overview)
- [Update Management の概要](https://docs.microsoft.com/ja-jp/azure/automation/update-management/overview)
- [Windows VM 用の Azure Disk Encryption](https://docs.microsoft.com/ja-jp/azure/virtual-machines/windows/disk-encryption-overview)
- [Linux VM に対する Azure Disk Encryption](https://docs.microsoft.com/ja-jp/azure/virtual-machines/linux/disk-encryption-overview)
- [Azure セキュリティ ベンチマークの概要](https://docs.microsoft.com/ja-jp/security/benchmark/azure/introduction)
- [資産インベントリを使用してリソースのセキュリティ態勢を管理する](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/asset-inventory)
  
**コンテナセキュリティ**
- [コンテナーと仮想マシン](https://docs.microsoft.com/ja-jp/virtualization/windowscontainers/about/containers-vs-vm)
- [Azure Container Instances のセキュリティに関する考慮事項](https://docs.microsoft.com/ja-jp/azure/container-instances/container-instances-image-security)
- [チュートリアル: Azure Kubernetes Service (AKS) でのアプリケーションに対するネットワークの概念](https://docs.microsoft.com/ja-jp/azure/aks/concepts-network)
- [Azure Kubernetes Service (AKS) でのアプリケーションのストレージ オプション](https://docs.microsoft.com/ja-jp/azure/aks/concepts-storage)
- [Azure Kubernetes Service (AKS) でのアクセスと ID オプション](https://docs.microsoft.com/ja-jp/azure/aks/concepts-identity)



## 1.3. モジュール03
**KeyVault**
- [Key Vault の価格](https://azure.microsoft.com/ja-jp/pricing/details/key-vault/)
- [Azure Key Vault の認証](https://docs.microsoft.com/ja-jp/azure/key-vault/general/authentication)
- [キーについて](https://docs.microsoft.com/ja-jp/azure/key-vault/keys/about-keys)
- [HSM で保護されたキーを Key Vault にインポートする](https://docs.microsoft.com/ja-jp/azure/key-vault/keys/hsm-protected-keys)
  
**APP**
- [Microsoft ID プラットフォームとは](https://docs.microsoft.com/ja-jp/azure/active-directory/develop/v2-overview)
- [Microsoft Graph セキュリティ API の概要](https://docs.microsoft.com/ja-jp/graph/security-concept-overview)
- [Azure リソースのマネージド ID とは](https://docs.microsoft.com/ja-jp/azure/active-directory/managed-identities-azure-resources/overview)
- [Graph Exploer](https://developer.microsoft.com/en-us/graph/graph-explorer)
- [Microsoft Graph API で Postman を使用する](https://docs.microsoft.com/ja-jp/graph/use-postman)
- [動画：Getting started with Microsoft Graph Postman workspace](https://www.youtube.com/watch?v=3RTHY3jScmA)
- [JWT Decoder(JSTOOLSET)](https://www.jstoolset.com/jwt)
  
**Storage**
- [すべての地域の Azure リージョン間レプリケーションのペアリング](https://docs.microsoft.com/ja-jp/azure/availability-zones/cross-region-replication-azure#azure-cross-region-replication-pairings-for-all-geographies)
- [Azure Storage に対する要求を承認する](https://docs.microsoft.com/ja-jp/rest/api/storageservices/authorize-requests-to-azure-storage)
- [Shared Access Signatures (SAS) を使用して Azure Storage リソースへの制限付きアクセスを許可する](https://docs.microsoft.com/ja-jp/azure/storage/common/storage-sas-overview)
- [保存データに対する Azure Storage 暗号化](https://docs.microsoft.com/ja-jp/azure/storage/common/storage-service-encryption)

**SQLServer**
- [SQLServerでAzure Active Directory 認証を使用する](https://docs.microsoft.com/ja-jp/azure/azure-sql/database/authentication-aad-overview)
- [Azure SQL Database および Azure Synapse Analytics の監査](https://docs.microsoft.com/ja-jp/azure/azure-sql/database/auditing-overview)
- [Microsoft Defender for SQL の概要](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-sql-introduction)
- [動的データ マスク](https://docs.microsoft.com/ja-jp/azure/azure-sql/database/dynamic-data-masking-overview)
- [Always Encrypted](https://docs.microsoft.com/ja-jp/sql/relational-databases/security/encryption/always-encrypted-database-engine?view=sql-server-ver15)
- [Azure SQL Analytics (プレビュー) を使用した Azure SQL Database の監視](https://docs.microsoft.com/ja-jp/azure/azure-monitor/insights/azure-sql)
  

## 1.4. モジュール04
**Monitor**
- [Azure Monitor メトリックの概要](https://docs.microsoft.com/ja-jp/azure/azure-monitor/essentials/data-platform-metrics)
- [Azure Monitor ログの概要](https://docs.microsoft.com/ja-jp/azure/azure-monitor/logs/data-platform-logs)
- [アラート概要](https://docs.microsoft.com/ja-jp/azure/azure-monitor/alerts/alerts-overview)
- [Azure Monitor の Log Analytics の概要](https://docs.microsoft.com/ja-jp/azure/azure-monitor/logs/log-analytics-overview)
- [Kusto クエリ言語 (KQL) の概要](https://docs.microsoft.com/ja-jp/azure/data-explorer/kusto/query/)
- [Azure プラットフォーム ログの概要](https://docs.microsoft.com/ja-jp/azure/azure-monitor/essentials/platform-logs-overview)
- [Azure Monitor の Log Analytics エージェントのデータ ソース](https://docs.microsoft.com/ja-jp/azure/azure-monitor/agents/agent-data-sources)
- [azure monitoring log demo](https://portal.azure.com/#blade/Microsoft_Azure_Monitoring_Logs/DemoLogsBlade)

**Defender**
- [Microsoft Defender for Cloud とは](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-cloud-introduction)
- [Microsoft Defender for Cloud の強化されたセキュリティ機能](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/enhanced-security-features-overview)
- [Azure セキュリティ ベンチマークの概要](https://docs.microsoft.com/ja-jp/security/benchmark/azure/introduction)
- [セキュリティ ポリシーの管理](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/tutorial-security-policy)
- [セキュリティの推奨事項 - リファレンス ガイド](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/recommendations-reference)
- [Just-In-Time アクセスを使用して管理ポートをセキュリティで保護する](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/just-in-time-access-usage?tabs=jit-config-asc%2Cjit-request-asc)
- [セキュリティ アラート - リファレンス ガイド](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/alerts-reference)
- [クラウドトリガーに対する Microsoft Defender への応答を自動化する](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/workflow-automation)

**Sentinel**
- [Microsoft Sentinel とは](https://docs.microsoft.com/ja-jp/azure/sentinel/overview)
- [すべてのデータに接続する](https://docs.microsoft.com/ja-jp/azure/sentinel/overview#connect-to-all-your-data)
- [Workbooks](https://docs.microsoft.com/ja-jp/azure/sentinel/overview#workbooks)
- [Microsoft セキュリティ アラートからインシデントを自動的に作成する](https://docs.microsoft.com/ja-jp/azure/sentinel/create-incidents-from-alerts)
- [チュートリアル: Microsoft Sentinel でオートメーション ルールとプレイブックを使用する](https://docs.microsoft.com/ja-jp/azure/sentinel/tutorial-respond-threats-playbook)
- [Microsoft Sentinel を使用して脅威を追求する](https://docs.microsoft.com/ja-jp/azure/sentinel/hunting)

**Memo**
- [Microsoft Defender for Cloud まとめ](pdf/Microsoft%20Defender%20for%20Cloud%20まとめ.pdf)
- [Microsoft Sentinel まとめ](pdf/Microsoft%20Sentinel%20まとめ.pdf)

**LAB13でエラーが出る時の対応**

> New-AzVm -ResourceGroupName "AZ500LAB131415" -Name "myVM" -Location 'EastUS' -VirtualNetworkName "myVnet" -SubnetName "mySubnet" -SecurityGroupName   "myNetworkSecurityGroup" -PublicIpAddressName "myPublicIpAddress" -OpenPorts 80,3389

VMを作るときにAZ CLIのバグで以下のエラーが場合があります

> New-AzVM: 'VMCustomization' is not enabled for the Subscription. Please register the Subscription for 'Microsoft.Compute/VMCustomizationPreview' to use the feature.

**対応**
CLiのAz.Computeのバージョンを4.23.0に戻します。

> 1 Check your current Az.Compute version number using either Get-Module Az.Compute (this will return nothing if the module hasn't been loaded) or Get-Module -ListAvailable -Name Az.Compute -Refresh
>
> 2 Install Az.Compute version 4.23: Install-Module Az.Compute -RequiredVersion 4.23.0 -Force
>
> 3 Switch to Az.Compute version 4.23: Import-Module Az.Compute -RequiredVersion 4.23.0
>
> 4 Import-Module: Assembly with same name is already loaded エラーが出ますが
>
> 5 Cloudshellを再起動します
