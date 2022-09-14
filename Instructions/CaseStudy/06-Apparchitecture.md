---
casestudy:
  title: アプリのアーキテクチャ ソリューションを設計する
  module: App architecture solutions
---
# <a name="design-an-app-architecture-solution"></a>アプリのアーキテクチャ ソリューションを設計する

## <a name="requirements"></a>要件

Tailwind Traders is looking to update their website to include customer supplied product images in addition to the already existing photos provided by marketing. They believe that having more photos of products in use will give potential customers a better feel for how past customers loved their products after purchasing them. They do have some requirements as outlined below:

* Uploaded images will need to be scanned before getting posted on the website. Legal and Marketing are both requesting that after initial upload, the images be checked for any issues that reflect poorly upon the company or could cause legal issues. An in-house API has already been developed and deployed that can perform the necessary scanning. 

* Based on existing patterns, Tailwind Traders expects the image uploads to happen very unevenly throughout the day. Certain periods may experience more uploads than the scanning software can handle, while other periods may experience very few or no uploads.

* Tailwind Traders は、アップロードされた画像がシステムによってスキャンされ、承認された後、画像の共有に対するお礼のメールをお客様に送信したいと考えています。

* Cost and management of the solution is a concern, especially since Tailwind Traders isn’t sure how popular this feature will be initially. Minimize costs and leverage serverless solutions where possible.

 

![アプリのアーキテクチャ](media/Apparchitecture.png)

 

## <a name="task"></a>タスク

会社の Web サイトに追加されるお客様の画像を対象とするアーキテクチャを設計します。 

* 画像はどこに格納する必要がありますか?

* アップロードがスキャンを上回っている場合でも、すべての画像が確実にスキャンされるようにするには、どうすればよいですか?

* 画像が承認され、カタログ データベースが更新された後、お客様への通知はどのように行われますか? 

高品質で安定した効率的なクラウド アーキテクチャを生み出すには、ウェル アーキテクト フレームワークの要素をどのように組み込みますか?

 
