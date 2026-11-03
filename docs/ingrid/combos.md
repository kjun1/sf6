# イングリッド：コンボ

[イングリッド](README.md) › [技・コンボ](README.md#reference) › コンボ

[起き攻め](okizeme.md) · [技データ](moves.md) · [214214P・SA2](combos/sa2.md)
· [記法](../notation.md)

**始動と目的を、それぞれの索引から探す。** 同じルートを両方から参照できる。
本文では同じ始動の回収型・火力型を隣に並べ、位置・ヒット条件・使えるゲージで絞る。

どの始動を狙い、回収と火力のどちらを優先するかは[戦略の比較](strategy.md)で考える。
このページでは、始動後の技列・消費・結果を共通の資料として管理する。

<a id="starter-index"></a>

## 始動から探す

| 始動 | レシピ |
| --- | --- |
| `5LP[PC]` / `2LP[PC]` | [4F確反](#route-punish-4f) |
| `5LK[PC]` | [5F確反：中ライズ / ODフレア / DRC回収](#route-punish-5f) |
| `2LK` | [小技](#route-close) / [SA2経由](combos/sa2.md#sa2-light) |
| `2LP[CH]` | [5MP~MKへつなぐ型](#route-close) |
| `2MP` | [通常ヒット](#route-close) / [CH](#anti-dr-combo) / [PC・7F確反](#route-punish-7f) / [DRC](#route-drc) |
| `5MP~MK` | [通常ヒット](#route-close) / [PC・6F確反](#route-punish-6f) / [開始2S](#route-enhanced) / [端・開始1S](#route-corner-loop) / [SA2経由](combos/sa2.md#from-hit) |
| `5MK` | [通常ヒット](#route-mid) / [DRC](#route-drc) |
| `2HP` | [通常ヒット](#route-mid) |
| `2MK` | [DRC](#route-drc) |
| `DR > 5HK` | [生DR始動](#route-dr5hk) |
| `5MK[PC]` / `5HK[PC]` | [投げ空振りへの反撃](#route-shimmy) |
| `4MK[PC]` | [9F・投げ空振りへの反撃](#route-shimmy-4mk) |
| `2HP[PC]` | [12F確反：回収 / 火力 / SA3](#route-punish) |
| `5HP[PC]` | [12F・遠めのPC反撃](#route-punish-5hp) |
| `214214MP` / `214214HP` | [SA2発動からの手順](combos/sa2.md) |

<a id="purpose-index"></a>

## 目的から探す

| 得たいもの | 見るところ |
| --- | --- |
| Sを回収する | [5LK[PC]・DRC型](#route-punish-5f) / [DRCの回収型](#route-drc) / [5MK[PC]](#route-shimmy) / [2HP[PC]](#route-punish) / [5HP[PC]](#route-punish-5hp) / [端のS回収](#route-corner-loop) / [SA2回収型](combos/sa2.md#stock-recovery) |
| 体力ダメージを取る | [PC反撃の火力型・236236P締め](#route-punish) / [SA2の火力比較](combos/sa2.md#damage) |
| 相手と位置を入れ替える | [SA2の位置入れ替え](combos/sa2.md#position-swap) |
| 相手のDゲージを削る | [SA2のDI締め](combos/sa2.md#drive-drain) |
| 次の起き攻めを作る | [中ライズ締め](#route-close) / [生DR始動](#route-dr5hk) / [端の回収ループ](#route-corner-loop) / [締め後の操作](okizeme.md#after-ender) |

<a id="notation"></a>
入力は[共通記法](../notation.md)に従う。`D`はコンボ全体の消費本数。Sは開始必要数・消費・回収を区別する。**ダメージは既存資料・過去メモの参考値**で、現行版で全件を再実測した値ではない。不明な値は「未実測」とする。

<a id="normal-hit"></a>

## 通常ヒットから選ぶ

<a id="route-close"></a>

### 小技・近距離の接触

| 完全入力 | 参考ダメージ | 消費・回収 | 条件 |
| --- | ---: | --- | --- |
| `2LK > 2LP:236MK` | 1,290 | D0、S消費0 | 2発で確認する形 |
| `2LK > 5LP > 5LK:236MK` | 1,370 | D0、S消費0 | 3発つながる距離 |
| `2LP[CH] > 5MP~MK:236MK` | 1,930 | D0、S消費0 | **CH限定**。+6Fから5MPが届く場合 |
| `2MP > 5LK:236MK` | 1,860 | D0、S消費0 | 5LKが届く距離 |
| `2MP > 5MP~MK:236MK` | 2,480 | D0、S消費0 | 5MPが届く近距離 |
| `5MP~MK:236MK` | 2,140 | D0、S消費0 | 中ライズ締め |
| `5MP~MK:214MP` | 1,930 | D0、S消費0 | 中フレア締め |

**通常ヒットの`2LP > 5LK`を目押しでつなぐ前提にしない。** `2LP`は通常ヒット+4F、`5LK`は発生5F。

ガードされた場合の止め方は[+2F後の小技](pressure.md#dr5hk-guard)。中ライズはガード-23Fなので、無確認で入れ込まない。締めた後は[起き攻め](okizeme.md#after-ender)へ。

<a id="route-mid"></a>

### 中距離：5MK・2HP

| 完全入力 | 参考ダメージ | 消費・回収 | 条件 |
| --- | ---: | --- | --- |
| `5MK:214MP` | 未実測 | D0、S消費0 | 中フレア締め |
| `2HP:214MP` | 1,700 | D0、S消費0 | 中フレア締め |
| `5MK:214HP` | 未実測 | D0、S残数に応じ消費 | 強化版は開始1S以上 |
| `2HP:214HP` | 未実測 | D0、S残数に応じ消費 | 強化版は開始1S以上 |

強化フレアはガード時にも有利を狙う選択。ただし通常技からの割り込み・接触距離は別条件。ガードなら[攻め継続](pressure.md#enhanced-pressure)、ダウンを取ったら[締め別の行動](okizeme.md#after-ender)へ。

<a id="route-dr5hk"></a>

### 生DR：DR > 5HK

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `DR > 5HK > 5MP~MK:236MK` | 2,680 | D1、S消費0 | 中ライズで起き攻めへ |
| `DR > 5HK > 5MP~MK:214MP` | 2,500 | D1、S消費0 | 中フレア締め |
| `DR > 5HK > 5MP~MK:214HP` | 未実測 | D1、S残数に応じ消費 | 強化版は開始1S以上 |
| `DR > 5HK > 5MP~MK:OD.214P` | 未実測 | D3、S残数に応じ消費 | 追撃はストックと位置次第 |

通常接触はヒット+8F、端の前投げからの持続重ねは+9Fの報告例。後続TCの届く距離が必要。ガードされたら[+2Fの読み合い](pressure.md#dr5hk-guard)、コンボ後は[締め別起き攻め](okizeme.md#after-ender)へ。

<a id="route-drc"></a>

### キャンセルDR

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `2MK:DRC > 5HK > 5MP~MK:236MK` | 未実測 | D3、S消費0 | 下段始動・中ライズ締め |
| `2MP:DRC > 2HP:236HK > j.214LP` | 未実測 | D3、S+1 | S回収型 |
| `5MK:DRC > 2HP:236HK > j.214LP` | 未実測 | D3、S+1 | S回収型 |

**`2MK`通常ヒットから`DRC > 2HP`へ始動を置き換えない。** `2MK`と`2MP`・`5MK`ではヒット状況が違う。成立後は[中ライズ・弱空フレア後](okizeme.md#after-ender)へ。

<a id="counter-hit"></a>

## CH・PCから選ぶ

<a id="anti-dr-combo"></a>

### DR止め：2MPカウンター

| 完全入力 | 参考ダメージ | 消費・回収 | 条件 |
| --- | ---: | --- | --- |
| `2MP[CH] > 5MK:214MP` | 未実測 | D0、S消費0 | CH・最速・5MKの届く距離 |
| `2MP[CH] > 5MK:214HP` | 未実測 | D0、S残数に応じ消費 | 上記に加え、強化版は開始1S以上 |

`2MP`は通常ヒット+6F、CHで+8F。発生8Fの`5MK`につながるのはCH時。
**相手の生DRを止めただけで必ずCHになるわけではない。**
[迎撃の選び方](neutral.md#anti-rush) / [締め後](okizeme.md#after-ender)

<a id="route-punish-fast"></a>

### 4〜7Fの確反：小技・中技から取る

**2HPが間に合わない隙にも、発生に合った始動を用意する。** 各技の発生と届く距離から[反撃を選ぶ](punish.md#by-window)。以下は初段PCを取るルートで、通常ヒット時のダメージとは分ける。

<a id="route-punish-4f"></a>

#### 4F：5LP / 2LP

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `5LP[PC] > 4MK~HP` | 未実測 | D0、S消費0 | PC後に4MKが届く距離。リーチの長いTCへつなぐ |
| `2LP[PC] > 2LP:236MK` | 未実測 | D0、S消費0 | 2発目の2LPが届く近距離。中ライズ締め |

5LPのPC→4MK追撃は[めいの調査](https://note.com/maytan0412/n/ne756d622e2f0)、4MK~HPは同記事と[かくぶろ](https://takukakugamer.com/sf6-ingrid-combo/)の基本TCを参照。
2LP側は[ドスの通常ヒット用2LP×2ルート](https://note.com/dos236236/n/nd3f3300416b7)を初段PCで使う形。PCで目押し先を増やしたレシピとは区別し、通常ヒット掲載値をPCダメージに転記しない。

<a id="route-punish-5f"></a>

#### 5F：5LK

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `5LK[PC]:236MK` | 1,320 | D0、S消費0 | 5F確反を中ライズで締める |
| `5LK[PC]:OD.214P[S消費1] > 6KKK` | 2,040 | D2、開始1S・消費1S | 前方サンバニッシュ締め |
| `5LK[PC]:OD.214P[S消費2] > 2KKK > 236MK` | 2,940 | D2、開始2S以上・消費2S | 上方→中ライズ |
| `5LK[PC]:DRC > 5MK:236HK > j.214LP` | 1,603 | D3、S+1 | DでS回収。DR後の5MKが届くこと |
| `5LK[PC]:DRC > 5MK:236HK > j.214MP` | 1,981 | D3、S消費0 | 同じ始動の火力型 |

最初の3行は[ドスの5F確反](https://note.com/dos236236/n/nd3f3300416b7)、DRC型は[かくぶろの弱攻撃始動](https://takukakugamer.com/sf6-ingrid-combo/)の掲載値。ドスの記事は2026-06-08までの更新で、5LK調整後の再実測値としては扱わない。
ODフレアは所持Sに応じて自動消費する。開始1Sの型を2S以上所持時に消費1Sのまま使えるとはしない。

<a id="route-punish-6f"></a>

#### 6F：5MP

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `5MP[PC]~MK:236MK` | 未実測 | D0、S消費0 | Dリバーサルへの反撃例。TC→中ライズ |
| `5MP[PC]~MK:214MP` | 未実測 | D0、S消費0 | TC→中フレア締め |

[かくぶろ](https://takukakugamer.com/sf6-ingrid-combo/)はTC→中ライズをDリバーサルへの反撃として紹介している。中ライズ・中フレアの通常ヒット掲載値を、初段PCの値として流用しない。

**開始2S以上・SA3で伸ばす公開例：** TCを先に挟まず、5MPのPCからODフレアへ進む。

```text
5MP[PC]:OD.214P[S消費2] > 2KKK > DR
> 5MP~MK:DRC > 5HK[2段目]:236236P
```

D6、S2消費、SAゲージ3本。SA3強度は未特定。同記事の掲載値5,916で、現行版の再実測値ではない。

<a id="route-punish-7f"></a>

#### 7F：2MP

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `2MP[PC] > 4MK~HP` | 未実測 | D0、S消費0 | 4MKが届く距離。しゃがみ姿勢から投げ空振りを取る候補 |

[めいのシミー追撃候補](https://note.com/maytan0412/n/ne756d622e2f0)を参照。2MPが当たっても、先端では4MKが届くとは限らない。DRCを使って回収する場合は[2MP始動](#route-drc)も比較する。

<a id="route-shimmy"></a>

### 8〜9FのPC反撃：シミー・確定反撃

**投げを空振らせた後、またはガード後の硬直に届く始動を選ぶ。** 反応に使った時間を含めた選び方は[シミーの手順](punish.md#shimmy)。7Fの2MP始動は[上の表](#route-punish-7f)も参照。

<a id="route-shimmy-5mk"></a>

#### 8F：5MK

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `5MK[PC]:236HK > j.214LP` | 未実測 | D0、S+1 | S回収型。先端接続は未確認 |
| `5MK[PC]:236HK > j.214MP` | 未実測 | D0、S消費0 | 火力型。先端接続・高度を確認 |
| `5MK[PC]:214MP` | 未実測 | D0、S消費0 | 強ライズが届かない場合の候補 |

`5MK[PC]`から強ライズへの接続は[西瓜Changの2026-08-04追記](https://note.com/nishiuri9235/n/n0efb730fe4eb)を参照。同じ記事に、当たり方によって強ライズがつながらないという記述がある。5MKの届く距離と、強ライズまでつながる距離を分ける。
5MK始動の約2,140 / 2,770は他始動からの推算なので採用しない。

<a id="route-shimmy-5hk"></a>

#### 9F：5HK

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `5HK[PC] > 5MP~MK:236MK` | 2,840 | D0、S消費0 | 5MPが届く距離。まず覚える中ライズ型 |
| `5HK[PC] > 5MK:OD.214P[S消費2] > 2KKK > 236MK` | 4,240 | D2、開始・消費2S | 5MKも届く距離 |
| `5HK[PC] > 5MK:236236P` | 4,860 | D0、S消費0、SA3 | PC・5MKが届く距離。SA3強度は未特定 |

2,840と4,240は[ドス](https://note.com/dos236236/n/nd3f3300416b7)、4,860は[めい](https://note.com/maytan0412/n/ne756d622e2f0)の掲載値。いずれも調整前の公開値で、現行版の再実測値ではない。5HKは通常必殺技キャンセル不可なので、5MPや5MKへの目押しを挟む。

<a id="route-shimmy-4mk"></a>

#### 9F：4MK

| 完全入力 | 参考ダメージ | 消費・回収 | 条件・目的 |
| --- | ---: | --- | --- |
| `4MK[PC] > 5MK:236MK` | 未実測 | D0、S消費0 | 4MKのPC後、5MKが届く距離 |

[かくぶろのシミー用レシピ](https://takukakugamer.com/sf6-ingrid-combo/)を参照。`4MK~HP`のTCとは分岐が違う。こちらはPCを取ってから5MKへ目押しする型。

各ルート成立後は[締め別起き攻め](okizeme.md#after-ender)へ。

<a id="route-punish"></a>

### 12F確反：2HP[PC]

**2HPを使う条件：12F以上の確反猶予があり、届くこと。** S回収・火力・リーサルを比べて選ぶ。[反撃の判断](punish.md#reversal)

| 完全入力 | 参考ダメージ | 消費・回収 | 目的・条件 |
| --- | ---: | --- | --- |
| `2HP[PC]:236HK > j.214LP` | 2,260 | D0、S+1 | S回収型 |
| `2HP[PC]:236HK > j.214MP` | 2,890 | D0、S消費0 | 火力型。弱版より+630 |
| `2HP[PC]:236HK > j.OD.214P[S消費1] > 236MK` | 3,925 | D2、開始1S・消費1S | 旧版参考 |
| `2HP[PC]:236HK > j.OD.214P[S消費2] > 236MK` | 4,180 | D2、開始2S以上・消費2S | 旧版参考 |
| `2HP[PC]:236HK > dl.j.MP > 236236P` | 5,080 | SA3のみ | 低めj.MP、強度未特定 |

`236236P`は元のSA3表記をコマンドに直したもの。元資料のボタン強度は未特定で、強度共通と確認した表記ではない。

**OD型3,925 / 4,180は調整前からの公開値。2026-08-03調整後の再実測は未確認。**

弱空フレアはS1回収、中空フレアは火力と長いダウン時間を取る。[弱・中空フレア後の行動](okizeme.md#after-ender)で、再接近するか地上回収するかを選ぶ。`236236P`締め後は別の状況として扱う。

<a id="route-punish-5hp"></a>

### 12F・遠め：5HP[PC]

**5HPが届き、12F以上残る場合の別始動。** 通常必殺技キャンセルはできない。PCの特殊のけぞりから6HPか生DRへ進む。

| 完全入力 | 参考ダメージ | 消費・回収 | 目的・条件 |
| --- | ---: | --- | --- |
| `5HP[PC] > 6HP:j.214MP` | 2,430 | D0、S消費0 | Dを使わない型。6HPまで届くこと |
| `5HP[PC] > DR > 2HP:236HK > j.214LP` | 2,391 | D1、S+1 | 生DRで接近してSを回収 |
| `5HP[PC] > DR > 2HP:236HK > j.214MP` | 2,769 | D1、S消費0 | 同始動の火力型 |

2,430と2,391は[かくぶろ](https://takukakugamer.com/sf6-ingrid-combo/)、2,769は[ドス](https://note.com/dos236236/n/nd3f3300416b7)の掲載例。始動の5HPだけでなく、後続の6HP・DR後2HPも届く距離を確認する。成立後は[締め別の行動](okizeme.md#after-ender)へ。

<a id="stock-and-position"></a>

## ストック・画面位置から選ぶ

<a id="route-enhanced"></a>

### 2S強化フレアからの追撃

| 完全入力 | 参考ダメージ | 消費・回収 | 条件 |
| --- | ---: | --- | --- |
| `5MP~MK:214HP > 6KKK` | 未実測 | D0、開始2S・消費2S | 前方サンバニッシュ追撃 |
| `5MP~MK:OD.214P > 2KKK > 236MK` | 未実測 | D2、開始2S・消費2S | OD版から上方サンバニッシュ追撃 |

**通常版`214HP > 2KKK`を一般的な中央ルートとして扱わない。** 通常版とOD版の追撃を区別する。[フレアのS別性能](moves.md#sunflare)

<a id="route-corner-loop"></a>

### 画面端：1Sを使って回収へ戻る

**条件：画面端・開始1S。** コンボ部分と、ダウン後の準備を分ける。

```text
コンボ：5MP~MK:214HP > 236HP
その後：214LP（S1回収）
```

D0。コンボでS1消費→ダウン後にS1回収。回収後約+4Fを狙う既存セットプレイで、始動・高度・タイミングが変われば同じ値になるとは限らない。次の択は[端のS回収セットプレイ](okizeme.md#corner-loop)へ。

<a id="route-sa2"></a>

## 214214P（SA2）を使う

長いレシピは[SA2コンボの専用ページ](combos/sa2.md)にまとめる。
通常技・ODライズからの発動、S回収、火力比較、DI締め、位置入れ替え、前j.MK締めを収録。

- ヒット時の完全入力・開始S・消費・参考ダメージ → [SA2コンボ](combos/sa2.md)。
- ガード発動とD削り → [SA2設置中の攻め](pressure.md#sa2-pressure)。
- 前j.MKで締めた後の表裏・投げ → [起き攻め](okizeme.md#sa2-crossup)。
- 弱中強、消費S、発動動作と弾発生 → [技の条件](moves.md#sun-order)。

<a id="route-stun"></a>

## まだ薄い・未収録の場面

この一覧は知っているルートを整理したもの。次に増やすなら、同じ用途の本数より**使える場面の穴**を優先する。

| 場面 | 現在足りないもの |
| --- | --- |
| S蓄積からの大火力 | 当てる始動ごとのS別・D/SA別ルートと、消費後の状況 |
| DIクリーンヒット・壁やられ | 状況別の基本ルート |
| 画面端BO・DIスタン | 開始S・使えるSA・相手残体力に応じたルート |
| 飛び込み・めくり | 地上通常ヒットへの接続条件 |
| 対空・空中ヒット | 当たった技と高度別の追撃 |
| SA1・リーサル | ゲージ別の締め比較 |
| SA2の追加条件 | 弱入力・投げ後・BO相手の体力削り・現行版の再実測 |

BO・DIスタンは[D削り・端攻め案](strategies/pressure-and-corner.md#win-plan)で狙う状況だが、単一の「4割確定ルート」は固定しない。`5MK[PC]`の先端接続・総ダメージ、弾ヒットから`2HK`の合計、既存ストック消費型の調整後ダメージも不明点として残す。

<a id="route-parts"></a>
書き足すときは[コンボのまとめ方](../guide.md)を参照。パーツ参照による省略は[将来方針](../guide.md#combo-parts)として保留し、完全入力を残す。[旧大量コンボメモ](../../archive/ingrid-combos-20261011.md)も参照できる。

## 参照・数値の出どころ

PC反撃の追加調査：2026-11-04。原文の技名を本ノートのコマンド表記へ整理した。公開レシピの採録で、ゲーム内で再実測した結果ではない。

- [ドス：コンボ・起き攻めまとめ](https://note.com/dos236236/n/nd3f3300416b7) — 2026-05-29公開、本文の最終更新記載は06-08。5F確反・5HK[PC]・2HP[PC]等。
- [めい：週末までに調べたイングリッド](https://note.com/maytan0412/n/ne756d622e2f0) — 2026-06-01。5LP[PC]→4MK、2MP[PC]→4MK~HP、5HK[PC]等。
- [西瓜Chang：地上戦の技の振り方](https://note.com/nishiuri9235/n/n0efb730fe4eb) — 2026-08-04・08-12追記を参照。5MK[PC]→強ライズの変更と距離条件。
- [SF6 Lab：コンボ・起き攻め](https://sf6-lab.net/fighters/ingrid/combo) — 2026-08-03調整対応の公開攻略。締め別Fやセットプレイの参照元。
- [かくぶろ：ダメージ付きコンボ](https://takukakugamer.com/sf6-ingrid-combo/) — 2HP[PC]・5HP[PC]・SA3型等の公開値。
- [くそまゆげ：フィジカル・イングリッド論](https://note.com/kusomayuge/n/n79bb407272dc)
  — DR強Kの運用等。
- [コミュニティ攻略メモ](https://scrapbox.io/1cc/%E8%8B%B1%E6%A0%BC%E9%BA%97%E7%89%B9%28%E5%BF%AB%E6%89%93%E6%97%8B6%29%2F%E7%B6%93%E5%85%B8%E6%A8%A1%E5%BC%8F)
  — DR強Kなどの参考ダメージ。ユーザー実測とは区別。
- [スト6原典：コンボ](https://sf6-genten.com/character/ingrid/category/combo)
  / [起き攻め](https://sf6-ingrid.com/character/ingrid/category/okizeme-setplay)
  — レシピとセットプレイ。
- [CAPCOM：2026-08-03調整](https://www.streetfighter.com/6/buckler/en/battle_change/20260803/ingrid)
  / [公式フレーム](https://www.streetfighter.com/6/character/ingrid/frame)
  / [UFD](https://ultimateframedata.com/sf6/ingrid) — 既存メモの技性能・調整参照先。

過去会話由来の1,860 / 2,480、DR強Kの2,680 / 2,500などは参考値として保持。成立距離・高度・パッチが変わる場合は再確認する。
