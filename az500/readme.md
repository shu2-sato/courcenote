## 1. **AZ-500**

**リンク一覧およびメモ**

- [AZ-500 ラボコンテンツ](https://microsoftlearning.github.io/AZ-500JA-AzureSecurityTechnologies/)
    - [ラボファイルをローカルにダウンロードする](https://github.com/MicrosoftLearning/AZ-500JA-AzureSecurityTechnologies/archive/master.zip)

- [トレーニングで使用するテキスト](https://docs.microsoft.com/ja-jp/users/msftofficialcurriculum-4292/collections/neqjf5m83e37x4?wt.mc_id=esi_m2l_content_wwl)

- [ラボ環境準備　PDF](pdf/ラボ環境準備.pdf)
    - InPrivte モードでブラウザを起動
    - [Microsoftアカウント作成](https://signup.live.com/?lic=1)
    - ラボ環境[LODS](https://esi.learnondemand.net/User/Login?ReturnUrl=%2F)**今回新しく作ったMSアカウントでログインしてください。**
    - トレーニングコードは、講師から案内があります。
    - AzurePass サブスクリプションはラボ環境からアクティベートします。
    - ラボ環境が英語の場合[ラボ環境キーボード変更](pdf/ラボ環境キーボード変更.pdf)
    
- [support使用法](pdf/support.pdf)

## 1.1. モジュール01
- [Azure Active Directory とは](https://docs.microsoft.com/ja-jp/azure/active-directory/fundamentals/active-directory-whatis)
- [Azure Active Directory の価格](https://www.microsoft.com/ja-jp/security/business/identity-access-management/azure-ad-pricing?rtc=1)
- [Azure Active Directory の基礎のドキュメント](https://docs.microsoft.com/ja-jp/azure/active-directory/fundamentals/)
- [Azure Active Directory を使用して基本グループを作成してメンバーを追加する](https://docs.microsoft.com/ja-jp/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal?context=azure/active-directory/users-groups-roles/context/ugr-context)
- [自己管理型の Active Directory Domain Services、Azure Active Directory、およびマネージド Azure Active Directory Domain Services の比較](https://docs.microsoft.com/ja-jp/azure/active-directory-domain-services/compare-identity-solutions)
- [Azure AD の組み込みロール](https://docs.microsoft.com/ja-jp/azure/active-directory/roles/permissions-reference)
- [Azure Active Directory の管理単位](https://docs.microsoft.com/ja-jp/azure/active-directory/roles/administrative-units?msclkid=96ef8dc1b80111ecb3108ac36c0152b9)
- [チュートリアル:グループ メンバーを自動的に追加/削除する](https://docs.microsoft.com/ja-jp/azure/active-directory/enterprise-users/groups-dynamic-tutorial)
- [Passwordless authentication is now generally available!](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/passwordless-authentication-is-now-generally-available/ba-p/1994700?msclkid=cb0f57efb80211ecb781b280a97fba33)
  
**HybridID**
- [Azure AD Connect とは](https://docs.microsoft.com/ja-jp/azure/active-directory/hybrid/whatis-azure-ad-connect)
- [Azure AD Connect クラウド同期とは](https://docs.microsoft.com/ja-jp/azure/active-directory/cloud-sync/what-is-cloud-sync)
- [Azure Active Directory ハイブリッド ID ソリューションの適切な認証方法を選択する](https://docs.microsoft.com/ja-jp/azure/active-directory/hybrid/choose-ad-authn)
- [チュートリアル:オンプレミス環境への Azure Active Directory のセルフサービス パスワード リセットのライトバックを有効にする](https://docs.microsoft.com/ja-jp/azure/active-directory/authentication/tutorial-enable-sspr-writeback)
  
**Identity** **Protection**
- [Identity Protection とは](https://docs.microsoft.com/ja-jp/azure/active-directory/identity-protection/overview-identity-protection)
- [リスクの種類と検出](https://docs.microsoft.com/ja-jp/azure/active-directory/identity-protection/concept-identity-protection-risks#risk-types-and-detection)
- [動作のしくみ: Azure AD Multi-Factor Authentication](https://docs.microsoft.com/ja-jp/azure/active-directory/authentication/concept-mfa-howitworks)
- [条件付きアクセスとは](https://docs.microsoft.com/ja-jp/azure/active-directory/conditional-access/overview)
- [Azure AD アクセス レビューとは](https://docs.microsoft.com/ja-jp/azure/active-directory/governance/access-reviews-overview)
- [Azure AD のセキュリティの既定値群](https://docs.microsoft.com/ja-jp/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

**PIM**
- [ゼロトラストという戦術の使い方(IPA)](https://www.ipa.go.jp/icscoe/program/core_human_resource/final_project/zero-trust.html?msclkid=ca679eb7b9de11ec95013ea55f031876)
- [ゼロトラスト導入指南書(IPA) 上記リンクのPDF](https://www.ipa.go.jp/files/000092243.pdf)
- [先回り型のセキュリティをゼロ トラストで取り入れる](https://www.microsoft.com/ja-jp/security/business/zero-trust)
- [Microsoft 365 を用いたゼロ トラスト ネットワークの実現](https://docs.microsoft.com/ja-jp/archive/blogs/jpazureid/building-zero-trust-networks-with-microsoft-365)
- [Azure AD Privileged Identity Management とは](https://docs.microsoft.com/ja-jp/azure/active-directory/privileged-identity-management/pim-configure)
- [PIM ダッシュボード](https://portal.azure.com/#blade/Microsoft_Azure_PIMCommon/ResourceMenuBlade/aadoverview/resourceId//resourceType/tenant/provider/aadroles/defaultId/roles)
- [Security best practices for Azure solution](https://azure.microsoft.com/mediahandler/files/resourcefiles/security-best-practices-for-azure-solutions/Azure%20Security%20Best%20Practices.pdf)
- [Azure Policy とは](https://docs.microsoft.com/ja-jp/azure/governance/policy/overview)
- [Azure Blueprint とは](https://docs.microsoft.com/ja-jp/azure/governance/blueprints/overview)

**エンターブライズ**  **ガバナンス**
- [サブスクリプション決定ガイド](https://docs.microsoft.com/ja-jp/azure/cloud-adoption-framework/decision-guides/subscriptions/#modeling-your-organization)
- [Azure 管理グループのドキュメント](https://docs.microsoft.com/ja-jp/azure/governance/management-groups/)
- [Azure Policy のドキュメント](https://docs.microsoft.com/ja-jp/azure/governance/policy/)
- [従来のサブスクリプション管理者ロール、Azure ロール、および Azure AD ロール](https://docs.microsoft.com/ja-jp/azure/role-based-access-control/rbac-and-directory-admin-roles)

**memo**
- [AZ-500 Azure ADまとめ](pdf/AZ-500%20Azure%20ADまとめ.pdf)
- [Azure AD Connect](pdf/Azure%20AD%20Connect.pdf)

**参考AAD関連**
- [Azure AD Webinar ](http://aka.ms/azureadwebinar)
- [Japan Azure Identity Support Blog ](https://github.com/jpazureid/blog)
- [EMS Blog ](http://aka.ms/emsblog/)
- [Azure AD Tips 集](http://aka.ms/aadtips)
- [Microsoft ID プラットフォームのドキュメント](https://docs.microsoft.com/ja-jp/azure/active-directory/develop/)

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
- [負荷分散のオプション](https://docs.microsoft.com/ja-jp/azure/architecture/guide/technology-choices/load-balancing-overview?toc=%2fazure%2ffrontdoor%2fstandard-premium%2ftoc.json)
- [Azure での負荷分散のデシジョン ツリー](https://docs.microsoft.com/ja-jp/azure/architecture/guide/technology-choices/load-balancing-overview?toc=%2fazure%2ffrontdoor%2fstandard-premium%2ftoc.json#decision-tree-for-load-balancing-in-azure)
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
- [Azure Container Instances とは](https://docs.microsoft.com/ja-jp/azure/container-instances/container-instances-overview)
- [Azure Kubernetes Serviceについて](https://docs.microsoft.com/ja-jp/azure/aks/intro-kubernetes)
- [チュートリアル: Azure Kubernetes Service (AKS) でのアプリケーションに対するネットワークの概念](https://docs.microsoft.com/ja-jp/azure/aks/concepts-network)
- [サービス](https://docs.microsoft.com/ja-jp/azure/aks/concepts-network#services)
- [イングレス コントローラー](https://docs.microsoft.com/ja-jp/azure/aks/concepts-network#ingress-controllers)
- [Azure Kubernetes Service (AKS) でのアプリケーションのストレージ オプション](https://docs.microsoft.com/ja-jp/azure/aks/concepts-storage)
- [Azure Kubernetes Service (AKS) でのアクセスと ID オプション](https://docs.microsoft.com/ja-jp/azure/aks/concepts-identity)
- [Japan Azure IaaS Core Support Blog](https://jpaztech.github.io/blog/tags/Containers/)
- [https://azure.github.io/application-gateway-kubernetes-ingress/ 詳しい資料](https://azure.github.io/application-gateway-kubernetes-ingress/)

**K8S参考資料**
- [Serviceを使ったアプリケーションの公開](https://kubernetes.io/ja/docs/tutorials/kubernetes-basics/expose/expose-intro/)
- [Service(上の資料より詳しい説明資料)](https://kubernetes.io/ja/docs/concepts/services-networking/service/)
- 

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
- [クイック スタート:Azure Storage Explorer を使用して BLOB を作成する](https://docs.microsoft.com/ja-jp/azure/storage/blobs/quickstart-storage-explorer)

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
- [意図](https://docs.microsoft.com/ja-jp/azure/security-center/alerts-reference#intentions
)
- [Microsoft Defender for Cloud とは](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-cloud-introduction)
- [Microsoft Defender for Cloud の強化されたセキュリティ機能](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/enhanced-security-features-overview)
- [Azure セキュリティ ベンチマークの概要](https://docs.microsoft.com/ja-jp/security/benchmark/azure/introduction)
- [セキュリティ ポリシーの管理](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/tutorial-security-policy)
- [セキュリティの推奨事項 - リファレンス ガイド](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/recommendations-reference)
- [Just-In-Time アクセスを使用して管理ポートをセキュリティで保護する](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/just-in-time-access-usage?tabs=jit-config-asc%2Cjit-request-asc)
- [セキュリティ アラート - リファレンス ガイド](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/alerts-reference)
- [クラウドトリガーに対する Microsoft Defender への応答を自動化する](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/workflow-automation)
- [Microsoft Power Automate と Azure Logic Apps の比較](https://docs.microsoft.com/ja-jp/azure/azure-functions/functions-compare-logic-apps-ms-flow-webjobs?msclkid=edcdfb9fb7d211ecaa09f53cbbd86280#compare-microsoft-power-automate-and-azure-logic-apps)

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


## ラボ　補足

**ラボ環境IME不整合**
- [WindowsPCの場合、キー入力で不整合がある場合の対応](pdf/ラボ環境IME不整合.pdf)

**LAB4テナント削除**
- [テナント削除の注意](pdf/テナント削除.pdf)
 無効化できないので、期限切れまで削除できません。

**LAB13のVMメモリー使用状況**
- タスク 4: 仮想マシン イベントおよびパフォーマンス データを収集する
  Perf用のメモリーカウンターが正しくないので
  - Memory(*)\Available Memory Mbytes を追加
 
    ```KQL
    Perf
    | where ObjectName == "Memory" and
    (CounterName == "Available MBytes Memory" or // the name used in Linux records
    CounterName == "Available MBytes") // the name used in Windows records
    | summarize avg(CounterValue) by bin(TimeGenerated, 15min), Computer, _ResourceId // bin is used to set the time grain to 15 minutes
    | render timechart
    ```
  
- [VM拡張診断の診断設定](pdf/LAB13VM診断設定が必要.pdf)
 Event Tracing for Windows\Total Memory Usage --- Non-Paged Pool
Event Tracing for Windows\Total Memory Usage --- Paged Pool

**LAB13でエラーが出る時の対応**
- 2.7.5                 Az.Accounts 
- 4.25.0                Az.Compute       

のバージョンで復旧しています。
以前古いモジュールをInstallしていた場合は、
get-moduleで確認して古いバージョンであれば、
>.local/share/powershell/Modules/Az.Accounts/
.local/share/powershell/Modules/Az.Compute/
のから古いバージョンのディレクトリを削除しPowershellを再起動してください。

[Azure PowerShell でのモジュールの読み込みのトラブルシューティング](https://github.com/Azure/azure-powershell/blob/main/documentation/troubleshoot-module-load.md#potential-reason-1-older-version-stored-in-user-or-global-scope)

**以下は、2022/4/7現在復旧しています**
> New-AzVm -ResourceGroupName "AZ500LAB131415" -Name "myVM" -Location 'EastUS' -VirtualNetworkName "myVnet" -SubnetName "mySubnet" -SecurityGroupName   "myNetworkSecurityGroup" -PublicIpAddressName "myPublicIpAddress" -OpenPorts 80,3389

VMを作るときにAZ CLIのバグで以下のエラーが場合があります

> New-AzVM: 'VMCustomization' is not enabled for the Subscription. Please register the Subscription for 'Microsoft.Compute/VMCustomizationPreview' to use the feature.

**対応**
CLiのAz.Computeのバージョンを4.23.0に戻します。

> 1 Check your current Az.Compute version number using either Get-Module Az.Compute (this will return nothing if the module hasn't been loaded) or Get-Module -ListAvailable -Name Az.Compute -Refresh
>
> **2** Install Az.Compute version 4.23: Install-Module Az.Compute -RequiredVersion 4.23.0 -Force
>
> 3 Switch to Az.Compute version 4.23: Import-Module Az.Compute -RequiredVersion 4.23.0
>
> 4 Import-Module: Assembly with same name is already loaded エラーが出ますが
>
> **5** Cloudshellを再起動します
