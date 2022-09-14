---
casestudy:
  title: リレーショナル ストレージ ソリューションを設計する
  module: Relational storage solutions
---
# <a name="design-relational-storage-case-study"></a>リレーショナル ストレージ ケース スタディを設計する

## <a name="requirements"></a>要件

Tailwind Traders is looking to move their existing public website database into Azure, as the website front end is being moved there as well.  The website front end will initially only be deployed in 2 regions for redundancy.  However, it is expected that as traffic increases the website will be replicated to other regions around the world. The database, which you are being asked to migrate, holds the product catalog, and all online orders.  Currently the database runs on a single Microsoft SQL Server Always On availability group on premises.

Tailwind Traders の主な懸念事項は次のとおりです。

-   <bpt id="p1">**</bpt>High availability.<ept id="p1">**</ept>  A primary concern for Tailwind Traders is that this database be highly available as it is critical to their business.  Any outages may result in lost sales or customer confidence.

-   <bpt id="p1">**</bpt>Website performance.<ept id="p1">**</ept>  While the performance of placing orders is normally satisfactory, browsing or searching pages with many items listed is reported as being “sluggish.”

-   <bpt id="p1">**</bpt>Security.<ept id="p1">**</ept>  Tailwind Traders is very concerned about personal or financial information stored in the database being exposed.  In addition to implementing proper security measures, the security team needs to verify that industry standard best practices are implemented, when possible.


## <a name="tasks"></a>タスク

1.  Tailwind Traders は、既存のパブリック Web サイト データベースを Azure に移動させることを検討しています。Web サイトのフロント エンドも、そこに移動されているためです。 
2.  決定した内容を図に示し、ソリューションについて説明します。 

高品質で安定した効率的なクラウド アーキテクチャを生み出すには、ウェル アーキテクト フレームワークの要素をどのように組み込みますか?
