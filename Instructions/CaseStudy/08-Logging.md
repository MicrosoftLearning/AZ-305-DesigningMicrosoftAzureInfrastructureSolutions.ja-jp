---
casestudy:
  title: Fabrikam Residences
  module: Logging and monitoring solutions
---
# <a name="case-study-fabrikam-residences"></a>ケース スタディ: Fabrikam Residences

## <a name="requirements"></a>要件

**このケース スタディでは、次のモジュールとケース スタディを完了している必要があります: コンピューティング、リレーショナル データ、非リレーショナル データ、認証、アプリケーション アーキテクチャ**

You have taken a new position with Fabrikam Residences, which is very successful and is experiencing rapid growth. Fabrikam Residences is a building contractor for new homes and major home renovations and have become successful by providing quality buildings and offering newer integrated home technologies than their competitors.  

Currently these technologies are provided and managed by separate sub-contract companies. The owners of Fabrikam Residences want to begin offering these upgraded technology options in-house to provide better quality, support and data on customer patterns and needs. 
 
Initially, the company wants to offer HVAC (heating and cooling) control and monitoring, security system monitoring and alerts, and home automation. This will require a new website, data storage solution and data ingestion solution.

The company has seen tremendous growth over the past 2 years. The company is estimating it may double in size over the next 12-18 months. With such rapid growth in the regional market, the company has no current plans to expand outside of the regional market.

## <a name="current-situation"></a>現在の状況

The Fabrikam Headquarters operates a small datacenter in a single location. The datacenter hosts the company <bpt id="p1">**</bpt>Project Management (PM) software<ept id="p1">**</ept>.

![プロジェクト管理ソフトウェアのアーキテクチャ](media/fabrikam.png)

- あなたは Fabrikam Residences で新たな職位に就き、大きな成功を収めて、急速に成長しています。  

- 画像とドキュメントは、専用の NAS アプライアンスに存在するサーバーのマップ済みドライブに格納されます。

- 企業ユーザー (オフィス スタッフ) は、Web フロントエンドを使用して、配送スケジュールや変更オーダーなどのデータを入力します。

-   Fabrikam Residences は、新築住宅や大掛かりな住宅改築のための建築請負業者であり、高品質の建物を提供し、競合他社よりも新しい統合ホーム テクノロジを提供することで成功を収めています。

The <bpt id="p1">**</bpt>Home Technology software<ept id="p1">**</ept> is currently provided and hosted by third parties and involves at least three different websites the customer must visit.  It is proposed the software be replaced with an in-house developed and unified solution.

![HVAC、セキュリティ、およびオートメーション アプリの図](media/software.png)

## <a name="requirements"></a>要件 

**プロジェクト管理ソフトウェア**

- 可能な限り多くのシステムをパブリック クラウド プロバイダーに移行します。

- 現在、これらのテクノロジは個別の下請会社によって提供および管理されています。

- Fabrikam Residences の所有者は、より良い品質、サポート、および顧客のパターンとニーズに関するデータを提供するために、これらのアップグレード済みのテクノロジ オプションを社内で提供し始めたいと考えています。

**新しいホーム テクノロジ ソリューション**

- 住宅監視センサーから継続的にデータを収集するための新しいソリューションを追加します。
  - 傾向分析とレポートのためにセンサーの一部の読み取り値をデータベース化します。
  - 所有者のニーズに基づいて、構成可能なリアルタイム アラートを提供します。
  
- 住宅所有者の基本設定と設定を保持するようにリレーショナル データベース ソリューションを設計します。
  - システムはスケーラブルである必要があります。
  - 冗長性は重要です。
  
- The new unified website will be developed in house and hosted on Linux.  This website will be used to view monitors and change preferences for items such as temperature or alert thresholds. Loads can vary widely, and the system must be able to scale quickly.

-   別のユーザー アカウントとパスワードを作成せずにシステムにサインインする方法をユーザーに提供します。

- セキュリティ コントロールを実装し、会社が業界標準のベスト プラクティスにどのように合致するかを示す週次レポートを提供します。

## <a name="tasks"></a>タスク 

1. 同社はまず、HVAC (冷暖房) の制御と監視、セキュリティ システムの監視とアラート、およびホーム オートメーションを提供したいと考えています。

2. これには、新しい Web サイト、データ ストレージ ソリューション、およびデータ インジェスト ソリューションが必要になります。

高品質で安定した効率的なクラウド アーキテクチャを生み出すには、ウェル アーキテクト フレームワークの要素をどのように組み込みますか?

