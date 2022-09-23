
# <a name="design-a-network-infrastructure-solution"></a>ネットワーク インフラストラクチャ ソリューションを設計する  

## <a name="requirements"></a>要件

As the Tailwind Traders Enterprise IT team prepares to define the strategy to migrate some of company’s workloads to Azure, it must identify the required networking components and design a network infrastructure necessary to support them. Considering the global scope of its operations, Tailwind Traders will be using multiple Azure regions to host its applications. Most of these applications have dependencies on infrastructure and data services, which will also reside in Azure. Internal applications migrated to Azure must remain accessible to Tailwind Traders users. Internet-facing applications migrated to Azure must remain accessible to any external customer. 

最初のネットワーク設計をまとめるために、Tailwind Traders Enterprise IT チームは 2 つの主要なアプリケーションを選択しました。Azure への移行が予想されるワークロードの最も一般的なカテゴリを表しています。  

### <a name="design---product-catalog-enterprise-application"></a>設計 - 製品カタログエンタープライズ アプリケーション

![製品カタログのアーキテクチャ](media/catalog.png)

- An internet-facing, Windows-based two-tier .NET Core-based web app providing access to the product catalog, hosted in a SQL Server Always On Availability Group database. This application is categorized as mission-critical, with availability SLA of 99.99%, 10-minute RPO and 2-hour RTO. 

-   Business leads emphasize the importance of the optimal customer experience when accessing internet-facing apps, so it is critical that the time it takes to load web pages and download static content is minimized. Similarly, a failure of individual servers hosting web app components and their dependencies should have negligible impact on the web app availability perceived by customers. While it’s understood that a regional failure might introduce some interruption to existing web sessions, the failover to a disaster recovery site should be automatic.

- Azure PaaS サービスによって提供される利点を活用するために、Enterprise IT チームは、Azure SQL Database を使用して、製品カタログ エンタープライズ アプリケーションのデータベースを実装することにしました。 

- Tailwind Traders の情報セキュリティ チームとリスク チームは、同じアプリケーションの一部である Azure VM と PaaS サービス間のすべての通信を、PaaS サービスのパブリック エンドポイント経由ではなく、Azure バックボーン経由で移動する必要があります。 

## <a name="tasks---product-catalog-enterprise-application"></a>タスク - 製品カタログエンタープライズ アプリケーション

1. Tailwind Traders Enterprise IT チームは、会社のワークロードの一部を Azure に移行する戦略を定義する準備の際に、必要なネットワーク コンポーネントを特定し、それらをサポートするために必要なネットワーク インフラストラクチャを設計する必要があります。 

高品質で安定した効率的なクラウド アーキテクチャを生み出すには、ウェル アーキテクト フレームワークの要素をどのように組み込みますか?

