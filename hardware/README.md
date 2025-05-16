# cocot38mini Case Guide

cocot38miniはマウント方式、ボール保持方式、ボール支持方式に応じて様々な種類のケースオプションを用意しています。このガイドにある各種方式の説明を参考に、お好みのケースを作成してください。

![cocot38mini_main00](/images/main_00.jpg)

# Mounting Method

![mounting_method](/images/Mounting_Method.jpg)

### Integrated
プレートインテグレーテッドマウントは部品点数が最も少ない方式です。プレートの厚みが5mmでかつケース構造と一体化されているので、比較的硬い打鍵感となっています。

|Parts|Qty|Note|
|---|---|---|
|3Dプリントトップケース|1|"_integrated"が含まれるトップケース|
|3Dプリントボトムケース|1|cocot38mini_v2_bottom.stp|

### Top Mount
トップマウントはプレートをトップケースにねじ止めする方式です。トップケースに熱圧入インサートナットを埋め込む必要があるので、組み立て難易度は比較的高めです。プレートの材質や厚みを変更することで打鍵感を調整することが可能です。

|Parts|Qty|Note|
|---|---|---|
|3Dプリントトップケース|1|"_topmount"が含まれるトップケース|
|3Dプリントスイッチプレート|1|"_topmount"が含まれるプレート|
|3Dプリントボトムケース|1|cocot38mini_v2_bottom.stp|
|熱圧入インサートナット|8|[HFB-2001](https://hirosugi.co.jp/products/B/HFB.html#bx1)|
|M2ねじ3mm|8||

### Tadpole Mount
タッドポールマウントはシンプルな構造と良好な打鍵感のバランスが特徴の方式です。タッドポールの硬さを変更することで打鍵感の調整が可能です。

|Parts|Qty|Note|
|---|---|---|
|3Dプリントトップケース|1|"_tadpole"が含まれるトップケース|
|3Dプリントスイッチプレート|1|"_tadpole"が含まれるプレート|
|3Dプリントボトムケース|1|cocot38mini_v2_tadpole_bottom.stp|
|Tadpole|8|Available at [GEONWORKS](https://geon.works/products/tadpole) or [GREENKEYS](https://shop.green-keys.info/products/tadpole)|

# Ball Supporting Method

![ball_support_method](/images/Ball_Support_Method.jpg)

### Zirconia Balls
2mmジルコニア球によるボール支持方式です。キットにジルコニア球が含まれている場合、追加のバーツは必要ありません。ジルコニア球を接着剤で固定した場合、ベアリングとの共存はできません。

|Parts|Qty|Note|
|---|---|---|
|ジルコニア球|3|Φ2mm|

### Bearing Rollers
ベアリングローラーによるボール支持方式です。スムーズな操球が可能です。   
組み立て方法は[picot5400](https://github.com/aki27kbd/picot5400/blob/main/doc/buildguide.md#%E3%83%9C%E3%83%BC%E3%83%AB%E3%82%B1%E3%83%BC%E3%82%B9)を参照してください。

|Parts|Qty|Note|
|---|---|---|
|ベアリングローラー|3|ID:3mm x OD:6mm x W:2.5mm|
|ステンレス棒|3|Φ2mm x L:6mm|
|シリコンチューブ|1|ID: 2mm x OD:3mm|

# Ball Holding Method

![ball_holding_method](/images/Ball_Holding_Method.jpg)

### Claw Holder
3本のツメでボールが落下しないようにするケースです。FDM方式のプリンターでケースを作成した場合、ツメが破損しやすくなるためお勧めいたしません。

|Parts|Qty|Note|
|---|---|---|
|3Dプリントトップケース|1|"_claw"が含まれるトップケース|

### Magnet Cover
マグネットによってボールカバーをトップケースに固定する方式です。容易にボールの取り外しが可能です。

|Parts|Qty|Note|
|---|---|---|
|3Dプリントトップケース|1|"_magnet"が含まれるトップケース|
|3Dプリントボールカバー|1|cocot38mini_v2_ballcover.stp|
|マグネット|8|Φ3mm x H:2mm|
