# Squidle+の用語解説

## データソースに関する用語
用語 | 解説 
--- | --- 
`Platform` | 画像取得に用いられた機器や手法 (例: 特定に AUV, ROV または 撮影機器) 
`Data Provider` | `Platform`で取得されたデータに対する管理責任者となる組織,研究所またはオペレーター
`Datasource Repository` | `Data Provider` が収集した生の画像や調査データをアップロードするための、アクセス可能な非一時的な（通常はオンラインの）アーカイブ  
`Datasource Plugin` | `Datasource Repository`からの読み込みを容易にするソフトウェアモジュール
`Datasource Definition`  | `Datasource Repository`上のデータの構造とフォーマットおよびどの`Datasource Plugin`をしようするかを定義するパラメータで、各 `Platform` は少なくとも1つの `Datasource Definition` を持つ必要がある


## データセットに関する用語
用語 | 解説 
---- | ----
`Media Object` | 一つの`Deployment`から得られるイメージ、ビデオ、モザイクのような、独立したビジュアルデータオブジェクトです。`Media Objects` は、オンラインツールを使って表示したり注釈を付けたりするために、仲介のプラグインを必要とする
`Campaign` | 複数の`Deployments`によって構成される一つのグループ 例: 一つの調査遠征、研究航海、データ収集の取り組み 
`Deployment` | `Platform`の一回のオペレーションで得られた`Media Objects`のクループを包括する一つのデータセット 例: 一回の調査, ドランゼクト　または ミッション
`Media Collection` | 解析を促進するためにユーザ定義された、グループ化された`Media Objects`のコレクションである．一つまたはそれ以上の`Deployments`から得られた`Media Objects`のサブセットを作ることが可能
`Annotation Set` | `Media Collection`をアノテーションする方法に関する定義. 例えば、 利用するアノテーション方法, パラメータ そして `Label Scheme`について. 一つの`Media Collection`は 関連した複数の`Annotation Set`を包括できる
`Label Scheme` | the chosen list of possible `Labels` for which to apply to `Annotations`. There are multiple `Label Schemes`.
`Label` | a discreet concept from the `Label Scheme` that can be assigned to `Annotations`
`Annotation` | a linking of a `Label` to an observation in a `Media Object` (i.e. a `Label` on a `Point` in a frame)
`Point` | an annotatable object on a media frame, captures x,y,t and can have multiple Annotations associated with it. A point can also be associated with a bounding box, polygon, pixel map, etc... Each `Point` can have one or more `Annotations`
`Tag` | an additional modifier that can be applied to an `Annotation`. Each `Annotation` can have multiple `Tags`.
`Comment` | a freeform entry that can be associated with an `Annotation`. 

