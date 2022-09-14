---
casestudy:
  title: 非リレーショナル ストレージ ソリューションを設計する
  module: Non-relational storage solutions
---
# <a name="design-non-relational-storage-case-study"></a>非リレーショナル ストレージ ケース スタディを設計する

## <a name="requirements"></a>要件

Tailwind Traders wants to reduce storage costs by reducing duplicate content and, whenever applicable, migrating it to the cloud. They would like a solution that centralizes maintenance while still providing world-wide access for customers who browse media files and marketing literature. Additionally, they would like to address the storage of company data files. 

![非リレーショナル ストレージ アーキテクチャ](media/Nonrelational%20storage.png)

 

* <bpt id="p1">**</bpt>Media files<ept id="p1">**</ept>. Media files include product photos and feature videos that are displayed on the company’s public website, which is developed and maintained in house. When a customer browses to an item, the corresponding media files are displayed. The media files are in different formats, but JPEG and MP4 are the most common. 

* <bpt id="p1">**</bpt>Marketing literature<ept id="p1">**</ept>. The marketing literature includes customer stories, sales flyers, sizing charts, and eco-friendly manufacturing information. Internal marketing users access the literature via a mapped drive on their Windows workstations. Customers access the literature directly from the company’s public website.

* <bpt id="p1">**</bpt>Corporate documents<ept id="p1">**</ept>. These are internal documents for departments such as human resources and finance. These documents are accessed and managed via an internally developed web application. Legal requires that various documents be retained for a specific period of time. Occasionally documents will need to be maintained longer when legal or HR issues are being investigated. Most corporate documents older than one year are only kept for compliance reasons and are seldom accessed.

* Tailwind Traders では、重複するコンテンツを減らし、必要に応じてクラウドに移行することで、ストレージ コストを削減することが求められています。 

* 彼らは、メディア ファイルやマーケティング資料を閲覧する顧客に世界規模のアクセスを提供しながら、メンテナンスを一元化するソリューションを望んでいます。 

## <a name="tasks"></a>タスク

1. Tailwind Traders のストレージ ソリューションを設計します。 

      * どのような種類のデータが表現されますか? 

      * 設計で考慮すべき要素は何ですか?

      * BLOB アクセス層を使用しますか?

      * 不変ストレージを使用しますか?

      * コンテンツに安全にアクセスするにはどうすればよいですか?

2.  さらに、彼らは会社のデータ ファイルのストレージに対処したいと考えます。 

高品質で安定した効率的なクラウド アーキテクチャを生み出すには、ウェル アーキテクト フレームワークの要素をどのように組み込みますか?
