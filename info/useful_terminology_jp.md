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
`Point` | メディアフレーム上の一つのアノテーション可能なオブジェクト,x,y,tをキャプチャし、複数のアノテーションを関連付けることができる.　ポイントは、バウンディングボックス、ポリゴン、ピクセルマップなどと関連付けることもできる. 各 `Point` は、1つまたは複数の `Annotation` を持つことができる.
`Tag` | `Annotation`に適応できる追加的な修飾項目. それぞれの`Annotation`には複数の`Tags`が付与できる.
`Comment` | アノテーションに関連付けることができる自由記入項目. 

