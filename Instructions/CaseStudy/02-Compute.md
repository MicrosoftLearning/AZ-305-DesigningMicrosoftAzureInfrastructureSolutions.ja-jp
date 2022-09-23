---
casestudy:
  title: コンピューティング ソリューションを設計する
  module: Compute solutions
---

# <a name="design-a-compute-solution"></a>コンピューティング ソリューションを設計する

## <a name="requirements"></a>要件

Tailwind Traders would like to migrate their product catalog application to the cloud. This application has a traditional 3-tier configuration using SQL Server as the data store. The IT team hopes you can help modernize the application. They have provided this diagram and several areas that could be improved. 

![コンピューティング アーキテクチャ](media/compute.png)

* The frontend application is a .NET core-based web app. During peak periods 1750 customers visit the website each hour. 

* The application runs on IIS web servers in a front-end tier. This tier handles all customer requests for purchasing products. During the latest holiday sale, the front-end servers reached their performance limits and page loads were lengthy. The IT team has considered adding more servers, but during off hours the servers are often idle.

* The middle tier hosts the business logic that processes customer requests. These requests are often for help desk support. Support requests are queued and lately the wait times have been very long. Customers are offered email rather than wait for a representative. But many customers seem frustrated and are disconnecting rather than wait. Customer requests are 75-125 per hour. 

* Tailwind Traders は、自社の製品カタログ アプリケーションをクラウドに移行させたいと考えています。

* 高可用性の懸念はありますが、法的要件により、会社はすべてのリソースを 1 つのリージョンに保持する必要があります。

## <a name="tasks"></a>タスク

* このアプリケーションは、従来の 3 層構成であり、データ ストアとして SQL Server が使用されています。 

* IT チームがあなたに期待するのは、アプリケーションの最新化に向けたサポートです。 

高品質で安定した効率的なクラウド アーキテクチャを生み出すには、ウェル アーキテクト フレームワークの要素をどのように組み込みますか?
