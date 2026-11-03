# イングリッド

[キャラ一覧](../../README.md) · [入力・用語](../notation.md) · [自由メモ](memo.md)

**複数の戦略仮説を比較し、場面別の技術と組み合わせて考える。** 接触・D削り・端攻めを重視する案と、接触を抑えてSを蓄え、大火力を狙う案を検討する。

`D`＝ドライブゲージ、`S`＝サンシンボル。

[戦略](#strategies) / [使い方](#gameplay) / [相手への対策](#matchups)
/ [技・コンボ](#reference) / [メモ](#notes)

<a id="strategies"></a>

## 戦略を比較する

| 戦略仮説 | 主に狙う利益 |
| --- | --- |
| [D削り・端攻め](strategies/pressure-and-corner.md) | 接触からDと位置を削り、端攻め・BO・DIスタンにつなげる |
| [S蓄積・大火力](strategies/stock-and-burst.md) | 接触リスクを抑えて準備し、一度の始動を高火力に変える |

[同じ局面での比較](strategy.md#comparison)から、相手・位置・体力・時間・リソースに応じた選び方を考える。

<a id="quick-reference"></a>

## 対戦前の早見表

| 場面 | まず意識すること | 詳しく見る |
| --- | --- | --- |
| まだ触れていない | 接触・前進で利益を取るか、距離維持・回収を狙うか選ぶ | [戦略の比較](strategy.md#comparison) / [地上戦](neutral.md) |
| Sを蓄えて大火力を狙いたい | 回収の時間と、蓄積後に何を当てるかを考える | [S蓄積・大火力案](strategies/stock-and-burst.md) |
| 相手が生DRで来る | `2MP`を本命、速さが必要なら`5LK` | [DR止め・CH条件](neutral.md#anti-rush) |
| 自分の`DR > 5HK`が当たる | TCから締めを選ぶ | [生DR始動コンボ](combos.md#route-dr5hk) |
| 同じ技をガードされる | +2Fから小技・投げ・シミー・様子見 | [ガード後の選択](pressure.md#dr5hk-guard) |
| 投げ抜けを空振らせる | 距離と猶予に応じて`5MK[PC]` / `5HK[PC]` | [シミーの反撃](punish.md#shimmy) |
| 無敵技をガードする | 火力を取るか、Sを回収するか選ぶ | [確反の選択](punish.md#reversal) |
| 投げ・コンボで倒す | 起き攻め・弾・S回収から選ぶ | [投げ後](okizeme.md#after-throw) / [締め別](okizeme.md#after-ender) |
| 端攻めを続けたい | 位置を保ち、打撃・投げ・シミーを回す | [端の攻め](pressure.md#corner-pressure) / [S回収ループ](okizeme.md#corner-loop) |

<a id="gameplay"></a>

## 使い方

各戦略で利用する場面別の技術。どの行動を優先するか、どの頻度で使うかは[戦略](strategy.md)で考える。

### 立ち回り

- [地上戦](neutral.md) — 距離別の行動候補と、接触・迎撃・距離維持・回収の使い分け。

<a id="offense"></a>

### 攻め

**触った後はガード後の攻め、倒した後は起き攻めを読む。**

- [ガード後の攻め](pressure.md) — 接触結果の確認 → 打撃・投げ・シミー → 端の攻め。
- [起き攻め](okizeme.md) — 投げ後・締め別の次入力、弾重ね、S回収ループ。
- SA2の[ガード発動・D削り](pressure.md#sa2-pressure)と、コンボ後の[表裏](okizeme.md#sa2-crossup)。
- 投げ空振りを取った後は[シミー反撃](punish.md#shimmy)、ヒット後の技列は[コンボ](combos.md)へ。

<a id="defense"></a>

### 守り・反撃

- 接近・飛び・DIへの回答を探す → [共通対策](matchups/README.md#common)。
- 無敵技などをガードして反撃を選ぶ → [確定反撃](punish.md#reversal)。

<a id="matchups"></a>

## 相手への対策

**イングリッドを使う側から、相手の行動への回答を探す。**

[対策ノート](matchups/README.md)では、キャラ共通の行動への回答と、相手キャラ固有の対策を分ける。
相手の技・距離・強度によって変わる部分はキャラ別に追加する。

<a id="reference"></a>

## 技・コンボ

| 資料 | 調べるもの |
| --- | --- |
| [コンボ](combos.md) | 始動・ヒット条件・位置から選ぶ完全入力、ダメージ、消費 |
| [214214P・SA2コンボ](combos/sa2.md) | 開始S・消費S・目的別の長いレシピ。ガード連係と起き攻めへ接続 |
| [技データ](moves.md) | 発生、硬直差、キャンセル、必殺技・SAの入力と性質 |
| [共通記法](../notation.md) | コマンド、強度、ホールド段階、リソースの読み方 |

<a id="notes"></a>

## メモ

[自由メモ](memo.md)へ分類前の気づき・試したいことを書き、まとまった内容を該当ページへ移す。

## 補足資料

- [対イングリッド](../matchups/ingrid.md) — イングリッドと戦う側からの共通対策。
- [ノートのまとめ方](../guide.md) — 他キャラ・キャラ別対策を追加するときの型。
