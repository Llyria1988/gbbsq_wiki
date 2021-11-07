# Squidle+の用語解説

## データソースに関する用語
用語 | 解説 
--- | --- 
`Platform` | 画像取得に用いられた機器や手法 (例: 特定に AUV, ROV または 撮影機器) .
`Data Provider` | `Platform`で取得されたデータに対する管理責任者となる組織,研究所またはオペレーター.
`Datasource Repository` | `Data Provider` が収集した生の画像や調査データをアップロードするためのアクセス可能な非一時的な（通常はオンラインの）アーカイブ.  
`Datasource Plugin` | `Datasource Repository`からの読み込みを容易にするソフトウェアモジュール.
`Datasource Definition`  | `Datasource Repository`上のデータの構造とフォーマットおよびどの`Datasource Plugin`をしようするかを定義するパラメータで,各 `Platform` は少なくとも1つの `Datasource Definition` を持つ必要がある.


## データセットに関する用語
用語 | 解説 
---- | ----
`Media Object` | 一つの`Deployment`から得られるイメージ,ビデオ,モザイクのような独立したビジュアルデータオブジェクト.`Media Objects` は,オンラインツールを使って表示したり注釈を付けたりするために仲介のプラグインを必要とする.
`Campaign` | 複数の`Deployments`によって構成される一つのグループ. 例: 一つの調査遠征、研究航海、データ収集の取り組み 
`Deployment` | `Platform`の一回のオペレーションで得られた`Media Objects`のクループを包括する一つのデータセット. 例: 一回の調査, ドランゼクト　または　ミッション
`Media Collection` | 解析を促進するためにユーザ定義された,グループ化された`Media Objects`のコレクションである．一つまたはそれ以上の`Deployments`から得られた`Media Objects`のサブセットを作ることが可能.
`Annotation Set` | `Media Collection`をアノテーションする方法に関する定義. 例えば, 利用するアノテーション方法,パラメータや`Label Scheme`など. 一つの`Media Collection`は関連した複数の`Annotation Set`を包括できる.
`Label Scheme` | アノテーションに適用される選択可能な`Labels`. 複数の`Label Schemes`がある.
`Label` | `Annotations`に割り当てることができる`Label Scheme`からは独立的な概念
`Annotation` | `Label`を`Media Object`上の観測にリンクさせること.　(例えば、一つの画像キャプチャーフレームの`Point`における`Label`)
`Point` | an annotatable object on a media frame, captures x,y,t and can have multiple Annotations associated with it. A point can also be associated with a bounding box, polygon, pixel map, etc... Each `Point` can have one or more `Annotations`
`Tag` | an additional modifier that can be applied to an `Annotation`. Each `Annotation` can have multiple `Tags`.
`Comment` | a freeform entry that can be associated with an `Annotation`. 

