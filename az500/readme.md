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

- [1. **AZ-500**](#1-az-500)
- [1.1. モジュール01](#11-モジュール01)
  - [1.1.1. Azure Active Directory](#111-azure-active-directory)
  - [1.1.2. ハイブリッド ID](#112-ハイブリッド-id)
  - [1.1.3. Azure AD Identity Protection](#113-azure-ad-identity-protection)
  - [1.1.4. Azure AD Pricileged Identity Management](#114-azure-ad-pricileged-identity-management)
  - [1.1.5. エンタープライズ ガバナンス](#115-エンタープライズ-ガバナンス)
  - [1.1.5. エンタープライズ ガバナンス](#115-エンタープライズ-ガバナンス-1)
- [1.2. モジュール02](#12-モジュール02)
- [1.3. モジュール03](#13-モジュール03)
- [1.4. モジュール04](#14-モジュール04)
- [ラボ　補足](#ラボ補足)

## 1.1. モジュール01
### 1.1.1. [Azure Active Directory](https://docs.microsoft.com/ja-jp/learn/modules/azure-active-directory/?wt.mc_id=esi_m2l_content_wwl)

[Azure AD の組み込みロール](https://docs.microsoft.com/ja-jp/azure/active-directory/roles/permissions-reference)
- **グローバル管理者は5人未満に割り当てるのが推奨**
- 緊急アクセス用管理者アカウント（Break Glass アカウント）も含む

**特権管理者**：テナントの強い権限のこと
- グローバル管理者（全体管理者）
- Exchange サービス管理者
- SharePoint サービス管理者
- パスワード管理者/ヘルプデスク管理者
- ユーザーアカウント管理者
- その他

**特権アカウント保護のためにやるべきこと**
- 原則として普段使いアカウントと特権アカウントは分ける
- 特権アカウント数はできるだけ少なく
- 特権アカウントを共有しない
- 必要最小限の権限を付与
- 多要素認証を有効にする
- 使うときだけ有効化
  
**試験対策**

[Azure サブスクリプションの課金所有権を譲渡する](https://docs.microsoft.com/ja-jp/azure/cost-management-billing/manage/billing-subscription-transfer)

**グループの種類は2つある**
- **セキュリティ**
  - ユーザー、デバイス、グループ、およびサービス プリンシパルをメンバーとして設定でき、ユーザーとサービス プリンシパルを所有者として設定できます。

- **Microsoft365（メールアドレスあり）**
  - ユーザーのみをメンバーとして設定することができます。 ユーザーとサービス プリンシパルはどちらも、Microsoft 365 グループの所有者にすることができます。
   - メンバーシップの動的は反映するまでに若干のタイムラグがある
   - メンバーシップの種類がグレーアウトした場合、一旦グループの種類を変更して戻すと選択できるようになる

**所有者**は、そのグループの責任者的な意味合いを持つ

> グループやポリシーなどは、まず最初に名前付け規則を作成することを推奨。特に、グループなどの管理責任者と利用目的は明確化しておくと後々の管理運用が容易になります。

[名前付け規則を定義する](https://docs.microsoft.com/ja-jp/azure/cloud-adoption-framework/ready/azure-best-practices/resource-naming)

[Azure Active Directory の価格](https://www.microsoft.com/ja-jp/security/business/identity-access-management/azure-ad-pricing?rtc=1)

[Azure Active Directory を使用して基本グループを作成してメンバーを追加する](https://docs.microsoft.com/ja-jp/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal?context=azure/active-directory/users-groups-roles/context/ugr-context)

[自己管理型の Active Directory Domain Services、Azure Active Directory、およびマネージド Azure Active Directory Domain Services の比較](https://docs.microsoft.com/ja-jp/azure/active-directory-domain-services/compare-identity-solutions)

[Azure Active Directory の管理単位](https://docs.microsoft.com/ja-jp/azure/active-directory/roles/administrative-units?msclkid=96ef8dc1b80111ecb3108ac36c0152b9)

[チュートリアル:グループ メンバーを自動的に追加/削除する](https://docs.microsoft.com/ja-jp/azure/active-directory/enterprise-users/groups-dynamic-tutorial)

| 属性名                     | 表示上の名前          |
| :------------------------- | :-------------------- |
| userPrincipalName          | ユーザー名            |
| DisplayName                | 名前                  |
| GivenName                  | 名                    |
| surName                    | 姓                    |
| userType                   | ユーザータイプ        |
| ObjectID                   | オブジェクトID        |
| dirsyncEnabled             | ソース                |
| jobTitle                   | 役職                  |
| department                 | 部署                  |
|                            | 管理者*               |
| BlockCredential            | サインインのブロック* |
| UsageLocation              | 利用場所              |
| StreetAddress              | 番地                  |
| State                      | 都道府県              |
| Country                    | 国/リージョン         |
| PhysicalDeliveryOfficeName | 会社                  |
| City                       | 市区町村              |
| PostalCode                 | 郵便番号              |
| telephoneNumber            | 会社電話              |
| Mobile                     | 携帯電話              |
|                            | 年齢グループ*         |
|                            | 未成年および同意*     |
|                            | ライセンス*           |

[PowerShell Microsoft 365ユーザー アカウントのプロパティを構成する](https://docs.microsoft.com/ja-jp/microsoft-365/enterprise/configure-user-account-properties-with-microsoft-365-powershell?view=o365-worldwide)

```powershell
Get-AzureADUser -SearchString user01 | Set-AzureADUser -Department IT
Get-AzureADUser -SearchString user01 | fl *
```

**パスワードレス認証方法**
- Windows Hello for Business
- FIDO2 セキュリティ キー
- Microsoft Authenticator アプリ
- 一時アクセスパス 

[Azure Active Directory でパスワードレス認証のデプロイを計画する](https://docs.microsoft.com/ja-jp/azure/active-directory/authentication/howto-authentication-passwordless-deployment)

***
### 1.1.2. [ハイブリッド ID](https://docs.microsoft.com/ja-jp/learn/modules/hybrid-identity/?wt.mc_id=esi_m2l_content_wwl)

**Azure AD Connect**
[Azure AD Connect:アカウントとアクセス許可](https://docs.microsoft.com/ja-jp/azure/active-directory/hybrid/reference-connect-accounts-permissions)

Azure AD Connect では、オンプレミス (Windows Server Active Directory) から Azure Active Directory に情報を同期させるために 3 つのアカウントが使用されます。 それらのアカウントを次に示します。
- AD DS コネクタ アカウント
- ADSync サービス アカウント
- Azure AD コネクタ アカウント

Azure AD Connect を実行するためのこれら 3 つのアカウントに加え、Azure AD Connect をインストールするには、次のアカウントが別途必要となります。 次のとおりです。
- ローカル管理者アカウント
- **AD DS エンタープライズ管理者（Enterprise Admins）アカウント**
- **Azure AD 全体（グローバル）管理者アカウント**
- SQL SA アカウント (任意) 

[Azure Active Directory Connect クラウド同期の FAQ](https://docs.microsoft.com/ja-jp/azure/active-directory/cloud-sync/reference-cloud-sync-faq)

[Azure AD Connect とクラウド同期の比較](https://docs.microsoft.com/ja-jp/azure/active-directory/cloud-sync/what-is-cloud-sync)

[Azure AD Connect クラウド同期の前提条件](https://docs.microsoft.com/ja-jp/azure/active-directory/cloud-sync/how-to-prerequisites)

[Azure AD Connect の通信要件](https://docs.microsoft.com/ja-jp/azure/active-directory/hybrid/reference-connect-ports)

**認証オプション**
- パスワードハッシュ同期
- パススルー認証
- AD FS
  
[チュートリアル:オンプレミス環境への Azure Active Directory のセルフサービス パスワード リセットのライトバックを有効にする](https://docs.microsoft.com/ja-jp/azure/active-directory/authentication/tutorial-enable-sspr-writeback)

[NIST SP800-207 「ゼロトラスト・アーキテクチャ」の解説と日本語訳](https://www.pwc.com/jp/ja/knowledge/column/awareness-cyber-security/zero-trust-architecture-jp.html)

[ゼロトラストという戦術の使い方(IPA)](https://www.ipa.go.jp/icscoe/program/core_human_resource/final_project/zero-trust.html?msclkid=ca679eb7b9de11ec95013ea55f031876)

[Microsoft 365 を用いたゼロ トラスト ネットワークの実現](https://docs.microsoft.com/ja-jp/archive/blogs/jpazureid/building-zero-trust-networks-with-microsoft-365)

***
### 1.1.3. [Azure AD Identity Protection](https://docs.microsoft.com/ja-jp/learn/modules/azure-ad-identity-protection/?wt.mc_id=esi_m2l_content_wwl)

[Azure AD Identity Protection のリスク](https://docs.microsoft.com/ja-jp/azure/active-directory/identity-protection/concept-identity-protection-risks)

**リスクの種類**
- ユーザー（リアルタイムとオフライン）
  - **漏洩されていないかを確認する。** 具体的には、MSが様々な情報を（ダークウェブなど）監視して合致するものがあるか？
- サインイン（リアルタイムとオフライン）
  - **本来のユーザーとは異なるユーザーからサインインしている可能性がある。** 匿名IPアドレスなど（上記リンク参照）を使用しているなどがある。

**認証の3要素**
- 知識情報（Something You Know）
- 所有情報（Something You Have)
- 生体情報（Something You Are）

[セキュリティの既定値群](https://docs.microsoft.com/ja-jp/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

[Azure AD で緊急アクセス用管理者アカウントを管理する](https://docs.microsoft.com/ja-jp/azure/active-directory/roles/security-emergency-access)

**条件付きアクセスポリシー(CA)**
-

**条件付きアクセスの動作**
- 動作はブラックリスト方式であるため、設計時に要考慮
  - <span style="color: red; ">明示的にポリシーを設定しない限り、アクセス許可</span>
  - CAポリシーで設定できるのは
    - アクセスのブロック
    - アクセス権の付与
- [割り当て] と [アクセス制御] の二つの要素でユーザー動作を制御
  - [割り当て]で「すべてのユーザー」、「すべてのクラウドアプリ」を対象にすると、管理者を締め出してしまう可能性あり（Azure AD Connect の同期用アカウントにも要注意）
  - 「すべてのユーザー」、「すべてのクラウドアプリ」 に対し、社外からのアクセスをブロックすると、Intune 登録、Graph などがブロックされてしまう
    - Microsoft Intune Enrollment クラウドアプリを除外してもダメ
- アクセスポリシーに順序はなく、すべてが評価される
    - CAポリシーに優先順位という概念はない
    - すべてのポリシーが評価され、割り当て条件に合致したサインインイベントに対し、制御がすべて適用される
    - <span style="color: red; ">許可よりもブロックが勝つ</span>
- [対象外] うまく使って割り当て条件を指定する
  - <span style="color: red; ">対象外が勝つ</span>（すべてのユーザーが対象でも対象外に設定したユーザーが勝つ）
- 問題があったら “サインインログ” を確認すると知りたいことはほぼすべてわかる
  - AADの監視＞サインイン（**条件付きアクセス項目**を参照する）

> **CAのポイント**
> - CAポリシーに優先順位という概念はない
> - すべてのポリシーが評価され、割り当て条件に合致したサインインイベントに対し、制御がすべて適用される
> - 許可よりもブロックが勝つ


- [割り当て] ベストプラクティス
  - すべてを対象にする際には細心の注意を
  - 対象を除外し、管理者は別ポリシーで保護
  - 除外には、ディレクトリ ロール を利用する
  - 不測の事態に備え、Break Glass アカウントを用意

- [アクセス制御] ベストプラクティス
  - ブロックの代わりに、「要 準拠デバイス」をお奨め
    - Intune 登録はブロックされない

**Break Glass アカウントとは**
- 不測の事態に影響を受けない緊急用 全体管理者アカウント
  - フェデレーションサービスの障害によるログイン不可
  - MFA 利用不可 - 電話網障害等
  - 管理者アカウント保持者の退職等

**ベストプラクティス**
- クラウドアカウント（例: bg@contoso.onmicrosoft.com）を利用
- 永続管理者（PIMの対象ロールにしない）を利用
- すべての 条件付きアクセス、MFA 対象から除外
- 16 文字以上のランダムに生成されたパスワードを利用
- パスワードは紙に書いて、2つ以上に切ってそれぞれ金庫に保管
- アカウント利用を定期的に監査
- アカウントを最低 90 日に一度、利用可能か確かめる

**管理者に MFA 強制するとバッチが動かなくなる？**
- 管理者アカウントでバッチを動かすことは、セキュリティリスクが高いため、すぐにやめましょう

**ベストプラクティス(この順番で実装を検討)**
1. Managed Identity を利用する（モジュール3で説明）
2. サービスプリンシパル を利用した証明書認証を利用する
3. やむなくユーザーアカウントを利用する場合にも要保護対策

[Azure AD アクセス レビューとは](https://docs.microsoft.com/ja-jp/azure/active-directory/governance/access-reviews-overview)

[条件付きアクセス:デバイス プラットフォーム](https://docs.microsoft.com/ja-jp/azure/active-directory/conditional-access/concept-conditional-access-conditions#device-platforms)
  
***
### 1.1.4. [Azure AD Pricileged Identity Management](https://docs.microsoft.com/ja-jp/learn/modules/azure-ad-privileged-identity-management/?wt.mc_id=esi_m2l_content_wwl)

**ゼロトラストの指導原則**
- 明示的に確認（常に認証と承認）
- 最低特権アクセス（JIT、JEA）、リスクベースの適応型ポリシー、データ保護によるユーザーアクセス制限
- 侵害の想定（ネットワークセグメンテーションによる横移動の防止）

**特権アカウント保護のためにやるべきこと**
- 原則として普段使いアカウントと特権アカウントは分ける
- 特権アカウント数はできるだけ少なく
- 特権アカウントを共有しない
- **必要最小限の権限を付与**
- **多要素認証を有効にする**
- **使うときだけ有効化**

**PIMの主な機能の確認**
- JIT（Just-In-Time）によって、作業時のみ権限を割り当てる。これは0.5～24時間まで
- リソースへの期限付きアクセス（権限を割り当てる際にあらかじめ有効期間を設定する）
- その権限を有効にするための承認プロセス
- 特権アカウントを使用する際に、MFAを確実に使用（全ユーザーがMFAを使用している場合＜すでにMFAにてログインしている＞は再度サインインする必要なし）
- そのアカウントのロールが必要な理由を明確化する。これによって、監査が容易になります。
- 特権アカウントが割り当てられた際の通知
- アクセスレビューによる、特権アカウントの割り当て把握
- 監査履歴をしようすることで、PIMイベントを継続的に追跡可能。外部監査にも利用できる。

[Azure AD Privileged Identity Management とは](https://docs.microsoft.com/ja-jp/azure/active-directory/privileged-identity-management/pim-configure)

**アクセスレビュー**

Identity Governanceは、「適切なユーザーに」 「適切なアクセス権を」 「適切な期間のみ」 を実現するもの。

- アクセスライフサイクル
  - エンタイトルメント管理（アクセス権の付与をプロセス化）
  - **アクセスレビュー（アクセス権のはく奪をプロセス化）**

**MFA の検証結果**

MFAを要求する設定は以下の通り
1. AAD>セキュリティ>MFA>追加のクラウドベースのMFA設定（各ユーザーに対して多要素認証を要求する）
1. AAD>セキュリティ>サインインリスクポリシー（ポリシーで多要素認証を要求する）
1. AAD>セキュリティ>条件付きアクセス（アクセス制御で多要素認証を要求する）

> - サインインリスクポリシーでMFAを要求した場合、追加のクラウドベースのMFA設定で許可していない場合は **Block** される。
> - 条件付きアクセスで多要素認証を要求する場合は、追加のクラウドベースのMFA設定で無効状態でもMFA認証を要求される（MFA設定画面に遷移する）。

***
### 1.1.5. [エンタープライズ ガバナンス](https://docs.microsoft.com/ja-jp/learn/modules/enterprise-governance/?wt.mc_id=esi_m2l_content_wwl)

**Azure ポリシー**
Azureポリシーを使用して、あるべき姿を強制する（コンプライアンス）ことができる。そのポリシーをまとめたものがイニシアティブとなる。

Azureポリシーの機能には以下の3つの大きな柱があります
- 強制とコンプライアンス
  - 設定したポリシーに対してすべてのリソースに対するコンプライアンス評価としてコンプライアンス状態を確認できる
- ポリシーを大規模に運用
  - 管理グループにポリシーを適用できることで、1つのポリシーを数百のサブスクリプションとそのすべてのリソースに対して適用できる
- 修復
  - コンプライアンスが非準拠のリソースを自動的に修復する修復ポリシーを使用できる
  - 修復時にマネージドIDが必要な効果は**DeployIfNotExists**と**Modify**

[Azure Policy の効果について](https://docs.microsoft.com/ja-jp/azure/governance/policy/concepts/effects)

[Azure Policy の定義の構造](https://docs.microsoft.com/ja-jp/azure/governance/policy/concepts/definition-structure)

[チュートリアル:コンプライアンスを強制するポリシーの作成と管理](https://docs.microsoft.com/ja-jp/azure/governance/policy/tutorials/create-and-manage)

**Azure リソースの組み込みロール**

組み込みロール一覧
```powershell
Get-AzRoleDefinition | ft name
```
AD Role の確認例
```powershell
Get-AzRoleDefinition 'Owner'
Get-AzRoleDefinition 'contributor'
Get-AzRoleDefinition 'user access administrator'
```

[Azure カスタム ロール](https://docs.microsoft.com/ja-jp/azure/role-based-access-control/custom-roles)

[Azure Blueprint とは](https://docs.microsoft.com/ja-jp/azure/governance/blueprints/overview)

[Azure サブスクリプションの課金所有権の譲渡の概要](https://docs.microsoft.com/ja-jp/azure/cost-management-billing/understand/subscription-transfer)

***

### 1.1.5. [エンタープライズ ガバナンス](https://docs.microsoft.com/ja-jp/learn/modules/enterprise-governance/?wt.mc_id=esi_m2l_content_wwl)

**Azure ポリシー**
Azureポリシーを使用して、あるべき姿を強制する（コンプライアンス）ことができる。そのポリシーをまとめたものがイニシアティブとなる。

Azureポリシーの機能には以下の3つの大きな柱があります
- 強制とコンプライアンス
  - 設定したポリシーに対してすべてのリソースに対するコンプライアンス評価としてコンプライアンス状態を確認できる
- ポリシーを大規模に運用
  - 管理グループにポリシーを適用できることで、1つのポリシーを数百のサブスクリプションとそのすべてのリソースに対して適用できる
- 修復
  - コンプライアンスが非準拠のリソースを自動的に修復する修復ポリシーを使用できる
  - 修復時にマネージドIDが必要な効果は**DeployIfNotExists**と**Modify**

[Azure Policy の効果について](https://docs.microsoft.com/ja-jp/azure/governance/policy/concepts/effects)

[Azure Policy の定義の構造](https://docs.microsoft.com/ja-jp/azure/governance/policy/concepts/definition-structure)

[チュートリアル:コンプライアンスを強制するポリシーの作成と管理](https://docs.microsoft.com/ja-jp/azure/governance/policy/tutorials/create-and-manage)

**Azure リソースの組み込みロール**

組み込みロール一覧
```powershell
Get-AzRoleDefinition | ft name
```
AD Role の確認例
```powershell
Get-AzRoleDefinition 'Owner'
Get-AzRoleDefinition 'contributor'
Get-AzRoleDefinition 'user access administrator'
```

[Azure カスタム ロール](https://docs.microsoft.com/ja-jp/azure/role-based-access-control/custom-roles)

[Azure Blueprint とは](https://docs.microsoft.com/ja-jp/azure/governance/blueprints/overview)

[Azure サブスクリプションの課金所有権の譲渡の概要](https://docs.microsoft.com/ja-jp/azure/cost-management-billing/understand/subscription-transfer)

**参考AAD関連**
- [Azure AD Webinar ](http://aka.ms/azureadwebinar)
- [Japan Azure Identity Support Blog ](https://github.com/jpazureid/blog)
- [EMS Blog ](http://aka.ms/emsblog/)
- [Azure AD Tips 集](http://aka.ms/aadtips)
- [Microsoft ID プラットフォームのドキュメント](https://docs.microsoft.com/ja-jp/azure/active-directory/develop/)
***

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
