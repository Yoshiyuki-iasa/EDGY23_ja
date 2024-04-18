---
title_en: "EDGY with ArchiMate(tm)"
title_ja: "EDGYとArchiMate"
keywords: 
source_url: https://enterprise.design/wiki/EDGY:ArchiMate
source_last_modified: 14 July 2023, at 14:08
folder: pages/tools_ja
summary:
tags: 
  - 
---
# EDGYとArchiMate®
著者: Milan Guenther, Marc Lankhorst, Jean-Baptiste Sarrodie. Annika Klyver, Joost Lommers, Robert Pike, Wolfgang Goeblに感謝します。_ArchiMate®は[**The Open Group®**](https://opengroup.org/)の登録商標です。_

このマッピングは、EDGYエンタープライズ要素を対応する[ArchiMate®](https://pubs.opengroup.org/architecture/archimate32-doc)要素にリンクします。より具体的には、EDGY要素は対応するArchiMate要素の特化として表現することができます。このメカニズムの詳細については、公式ドキュメントの[概念の特化](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Language-Customization-Mechanisms.html#sec-Specialization-of-Concepts)の章を参照してください。

## 本マッピングの使用
このマッピングは、一般的なエンタープライズ・デザイン手法、とりわけEDGYは、あるイニシアチブの戦略的背景の構築に使用されるという考えに基づいて設計されています。したがって、このArchiMate®へのマッピングは、モチベーション要素とストラテジー層の要素にフォーカスしており、ArchiMateのコア要素は、EDGYが直接カバーしない他のレイヤーに用いられます。使用コンテキストによっては、別のマッピングも可能です。

ArchiMate® 3.2の特化メカニズムにより、どのようなツールや環境でも、EDGY要素を使って企業をモデル化できます。このマッピングは主に次のふたつのユースケースを念頭に設計されています：

1. ArchiMate®を使ってEDGYのみでエンタープライズ・モデルを作成する：純粋にグラフィカルなダイアグラム・エディターやホワイトボードではなく、リポジトリ・ベースのモデリング・ツールを活用するために、ArchiMate®の要素とリレーションはモデルの基礎となる目に見えないバックボーンを提供します。EDGYの要素や関係はすべてArchiMate®の要素や関係に対応しますが、各マップ (ビュー) の描写はEDGYダイアグラムのそれのみに従います。
2. EDGYをArchiMate®と組み合わせて使用する：このシナリオでは、両方の言語が同じモデルの一部として一緒に使用されます。EDGYは、アイデンティティとエクスペリエンスのファセットを表すマップの作成に使用されます。EDGYを使用してモデリングされたハイレベルのアーキテクチャは、より具体的なArchiMate®のビューポイントを使用して、より豊かで厳密な言語機能を活用しながら、詳細化され、実装へと導かれます。

## ベース要素
EDGYのベース要素は、すべてのファセットに共通の語彙を構築します。これらは、ArchiMate®で使用されているタイプ (能動構造と受動構造、振る舞いとモチベーション) に概念的に対応しています。しかし、これらのカテゴリーとは異なり、ファセット要素やインターセクション要素で特にカバーされていないエンタープライズ要素間の相互作用のモデル化に使用されるため、具体的なArchiMate®要素にマッピングされます。

<img src="https://github.com/Yoshiyuki-iasa/EDGY23_ja/blob/main/media/EDGY_Base_Elements_ArchiMate_mapping (1).png?raw=true" width="100%" alt="EDGY Base Elements ArchiMate mapping.png"><br>

|EDGY要素|ArchiMate®要素|所見|
|---|---|---|
|ピープル|ステークホルダ|EDGYは人間中心である。人とは法人を含むあらゆる人や集団を指す。<br>ArchiMate®では人々はアーキテクチャの効果に対する利害関係者に相当する。|
|アウトカム|アウトカム|どちらの言語も、最終結果のモデル化にアウトカム要素を使用する。|
|アクティビティ|バリュー・ストリーム|EDGYではアクティビティは進行中のあらゆることのモデル化に使用される。<br>普遍性のたかいArchiMate®のコンセプトではバリュー・ストリーム最も近い。|
|オブジェクト|リソース|EDGYは、エンタープライズに関連するあらゆる構造や物事を表す普遍的な基本要素としてオブジェクトを用いる。<br>これに相当する最も近いArchiMate®要素は、個人または組織が所有または管理するリソースである。|

## ファセットおよびインターセクション要素
EDGYでは、以下の要素はそれぞれ対応するエンタープライズ・デザイン・ファセットとそれらの直接のインターセクションの領域内で提起される質問やトピックと直接結びついており、ArchiMate®のレイヤーやカテゴリーとは異なるスコープを持ちます。このマッピングは、EDGYをArchiMateのストラテジー、モチベーション、ひとつのビジネス要素と整合させ、それらを用いてあるイニシアチブを戦略的にとらえる、という考え方に従っています。このマッピングは、EDGYプロセスとArchiMate®プロセスのような言語的に直接的なマッピングよりも、特定の使用状況においてよりよくマッチすれば適切な選択肢となる、このようなユースケースに向いています。

<img src="https://github.com/Yoshiyuki-iasa/EDGY23_ja/blob/main/media/EDGY_Facet_Intersection_Elements_ArchiMate_mapping.png?raw=true" width="100%" alt="EDGY Facet Intersection Elements ArchiMate mapping.png"><br>


|EDGY要素|ArchiMate®要素|所見|
|---|---|---|
|パーパス|ゴール|エンタープライズのパーパスはエンタープライズが追求するゴールの一種であり、したがってArchiMate®のゴール要素に対応する。|
|ストーリー|コース・オブ・アクション|EDGYのストーリーは、エンタープライズの野心を文脈化し、説明するもので、これはArchiMate®のコース・オブ・アクションに当たる。|
|コンテンツ|リソース|ArchiMate®にはコンテンツに直接相当するものはないが、リソースの一種として表現できる。|
|オーガニゼーション|リソース|EDGYでいう組織とは、一緒に働く人の集まりのことで、ArchiMate®では一種の(人的)リソースとして表現するのが最適である。|
|ケイパビリティ|ケイパビリティ|EDGYおよびArchiMate®両方において、ケイパビリティ要素の定義と用法は同様である。|
|プロセス|バリュー・ストリーム|EDGYのプロセス要素は、ArchiMate®で詳細なプロセス記述やシナリオに使われるビジネスプロセス要素よりバリューストリーム要素に近い。|
|アセット|リソース|EDGYは、ArchiMate®でさらに区別される様々なタイプの資産に単一の要素を使用する。最も普遍的な等価物はリソースである。|
|プロダクト|プロダクト|どちらの言語も、企業活動の結果としての製品を表す汎用的な要素を備えている。概念が近いことからこのマッピングでは唯一のArchiMateコア要素である。|
|タスク|ゴール|EDGYで定義される顧客やその他の人々の個人的な動機は、ArchiMate®では誰かが達成しようとするゴール要素に対応する。|
|ジャーニー|バリュー・ストリーム|ArchiMate®にはジャーニーにあたる要素がなく、EDGYのジャーニーの定義は、特定のステークホルダーに結びついたバリュー・ストリームの一種として表現するのが最適である。|
|チャネル|リソース|EDGYでは、チャネルとはメディアや物理的環境などの相互作用やコミュニケーションの手段を指す。ArchiMate®では、これは企業がステークホルダーと対話するために使用するリソースの一種として表現するのが最適である。|
|ブランド|ステークホルダ|EDGYは、ブランドとは名前とそれを象徴するものであり、人々のグループ、評判、行動を表すものであると定義している。<br>ArchiMate®では、これを一種の（名前付き）ステークホルダーとしてモデル化するのが最適である。|

## リレーションシップ
EDGY only has three relationship types that can be mapped to similarly generic relations in ArchiMate®, in order to permit flexible modelling.

EDGYは3つの関係タイプで柔軟なモデリングを可能にし、それらは同様に汎用的なArchiMate®の関係にマッピングできます。

<br><img src="https://github.com/Yoshiyuki-iasa/EDGY23_ja/blob/main/media/EDGY_ArchiMate_Relationships.png?raw=true" width="50%" alt="EDGY ArchiMate Relationships.png">

|EDGYリレーション|ArchiMate®リレーション|所見|
|---|---|---|
|リンク|アソシエーション|EDGYのリンク関係は、ArchiMate®のアソシエーション関係に相当する。どちらの言語でも、EDGYのコア・リンクのような無向関係や有向関係をサポートしている。|
|フロー|フロー|どちらの言語にも、ふたつの要素間のフローという概念がある。|
|ツリー|アグリゲーション|EDGYでは、同じ要素のあらゆる階層表現はツリー関係であり、これは階層の性質をさらに特定しないため、ArchiMate®のアグリゲーション(集約)関係に相当する。|

## 使い方とカスタマイズ
EDGYダイアグラム表記法は、代替のシェイプやカラーを組み込むだけで、多くのArchiMate®対応ツールに導入できます。どちらの言語でも、マップやビューをよりアクセスしやすく魅力的なものにするために、カスタマイズされた視覚表現を推奨しています。

特定の使用状況に適応するため、EDGYは要素をさらに区別し、追加情報をとらえるためのラベル概念を備えています。ArchiMate®をモデリング言語として使用する場合、以下の実装が可能です：
- 異なるタイプの要素を区別するタグは、このマッピングを超えてさらにArchiMate®の特化を定義することができます。
- ツールのサポートによっては、リポジトリに要素と一緒に保存されている属性や、単純なグラフィカル・オーバーレイになることもあります。これは、追加されたメトリクスにも当てはまります。

<br><img src="https://github.com/Yoshiyuki-iasa/EDGY23_ja/blob/main/media/EDGY-ArchiMate-Mapping-Labels.png?raw=true" width="50%" alt="EDGY-ArchiMate-Mapping-Labels.png">
_カスタム・マッピングの例_

あなたの仕事やツールで、EDGYからArchiMate™へのマッピングの使用を検討しているときは、私たちのコミュニティに参加して仲間と交流し、そのさらなる発展に関わってください。

---
特に断りのない限り、コンテンツは[CC BY-SA 4.0ライセンス](./pages/license_ja.md)の下で利用可能です。
<br><a href="./pages/license_ja.md"> <img src="https://github.com/Yoshiyuki-iasa/EDGY23_ja/blob/main/media/cc.png?raw=true" alt="CC logo"></a>
