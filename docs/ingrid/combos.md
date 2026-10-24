# イングリッド：コンボと記法

> **コンボは基本戦略を実行するための手段**。先に [戦略](strategy.md)・[地上戦](neutral.md)・[ガード後の読み合い](pressure.md)・[確定反撃](punish.md)・[起き攻め](okizeme.md)を考え、その状況に必要なコンボだけを選ぶ。**完全技列・ダメージ・S/D収支の正本は本ファイル**。

## 現時点の保存方針

- **技列を省略せず、1本ずつ完全表記で残す**。まず始動／位置／ヒット条件／SとD／ダウン後の行動を整理する。
- Starter / Linker / Ender / Frag への分割は、十分なルートが集まってから行う。
- パーツを参照する省略表記は後で作る。完全表記が正本。
- コンボ以外の起き攻め行動・ストック回収は技列の末尾に混ぜず、別の行に書く。
- 個別の検証履歴・検証ステータスは管理しない。
- 以前の大量列挙は [移行用の旧コンボメモ](../../archive/ingrid-combos-20261011.md) に保存。攻略用の正本とは区別する。

<a id="notation"></a>
## コマンド・記法

| 表記 | 意味 |
|---|---|
| `5LP/5LK/5MP/5MK/5HP/5HK` | 立ち通常技（`5` は省略可能） |
| `2MP` 等 | 方向（テンキー）＋ボタン |
| `>` | 目押し・リンク・ヒット後の追撃 |
| `:` | キャンセル |
| `~` | ターゲットコンボ／派生 |
| `j.` | 空中入力 |
| `OD.` | OD版 |
| `DR` | 生ドライブラッシュ |
| `DRC` | キャンセルドライブラッシュ |
| `dl.` | 遅らせ |
| `[CH]` / `[PC]` | カウンター／パニッシュカウンター |
| `[Corner]` / `[Air Hit]` | 画面位置・ヒット状況 |
| `S` / `D` | サンシンボル／ドライブゲージ |

SA：`236236K`＝SA1、`214214P`＝SA2、`236236P`＝SA3。

**Sの「開始時必要数」と「消費数」は別**。以前のメモで両者が混同されたため、必要なら `start: 1S` `spend: 1S` と書く。

## 優先して管理するコンボ

<a id="anti-dr-combo"></a>
### 1. DR反応止め：2MPカウンター

```text
[CH] 2MP > 5MK:214MP
[CH, 開始1S以上] 2MP > 5MK:214HP
```

`2MP` は通常ヒット+6F、CH+8F。後続の `5MK` は8Fなので、**CH・最速入力・5MKの届く距離が成立前提**。反応止めを失敗した状況にまで適用しない。[地上戦でDRを止める局面](neutral.md#anti-rush) → 本コンボ → [締め後の選択](okizeme.md#after-ender)。

### 2. 中距離の接触から締める

```text
5MK:214MP
2HP:214MP
[開始1S以上] 5MK:214HP
[開始1S以上] 2HP:214HP
```

`214HP` の強化版はガードされた場合にも有利を取るための選択肢。ただし通常技キャンセル後の割り込み・距離は別に扱う。ガード時は [強化サンフレア後の読み合い](pressure.md#enhanced-pressure)、ヒットしてダウンさせたら [起き攻め](okizeme.md#after-ender) に移る。

### 3. DRCからダウン

```text
2MK:DRC > 5HK > 5MP~MK:236MK
2MP:DRC > 2HP:236HK > j.214LP
5MK:DRC > 2HP:236HK > j.214LP
```

`2MK` と `2MP`・`5MK` は無条件に始動技を交換できない。`2MK` 通常ヒットの `DRC > 2HP` は安易に採用しない。ダウンした場合は [締めの種類別の起き攻め](okizeme.md#after-ender) を参照する。

### 4. 強化ビーム後の締め

```text
[2S] 5MP~MK:214HP > 6KKK
[2S, OD版] 5MP~MK:OD.214P > 2KKK > 236MK
```

前者は2S強版を使った前方サンバニッシュのルート、後者は2S OD版の上方サンバニッシュ追撃。**通常版 `214HP > 2KKK` を一般的な中央ルートとして記録しない**。

<a id="route-corner-loop"></a>
### 5. 画面端でSを回収して攻めを継続

```text
[Corner, 開始1S]
combo: 5MP~MK:214HP > 236HP
after: 214LP（S回収、起き上がりに対して約+4Fを狙う）
```

これは連続技とセットプレイを区別した表記。ダウン後のS回収・+4Fからの継続は [端のS回収セットプレイ](okizeme.md#corner-loop) を参照。

### 6. 端・BO・DIスタン

最終目標に直結するが、必要なS・SA量や状況で火力が変わるため、ここでは単一の「4割確定ルート」を固定しない。採用する場合は **相手の残体力、開始S、使えるSA、スタン状態**とセットで記録する。

## 接触・確定反撃から使う実戦ルート

値はこの表を正本とする。他文書では、**どの状況で選ぶか**と**次にどう移るか**を記述し、ここへリンクする。数値は攻略資料・過去の会話で記録した**条件付き参考値**。未実測は空想で埋めない。

<a id="route-dr5hk"></a>
### `DR > 5HK` ヒット時

[ガード後の分岐へ戻る](pressure.md#dr5hk)／コンボ後は[締め別起き攻め](okizeme.md#after-ender)へ。

| 完全な入力 | 参考ダメージ | コスト・条件 | ヒット後の次状況 |
|---|---:|---|---|
| `DR > 5HK > 5MP~MK:236MK` | **2,680** | 1D、追加S0。攻略メモ値 | [中ライズ締め](okizeme.md#after-ender)・約+38Fの例 |
| `DR > 5HK > 5MP~MK:214MP` | **2,500** | 1D、追加S0。攻略メモ値 | [中フレア締め](okizeme.md#after-ender)・約+47Fの例 |
| `DR > 5HK > 5MP~MK:214HP` | 未実測 | 1D＋S残数に応じ消費 | [強化214HPの端ヒット回収](okizeme.md#corner-loop)候補 |
| `DR > 5HK > 5MP~MK:OD.214P` | 未実測 | 計3D＋S残数に応じ消費 | 追撃・強化後のダウン位置に応じ選択 |

`2,680`／`2,500` は2026年の攻略メモ値で、現行調整・全距離の再実測ではない。通常接触 `DR > 5HK` ヒット+8Fに対し、画面端前投げからの持続重ねはヒット+9Fの報告例があり、接触条件を分ける。

<a id="route-close"></a>
### +2F後の下段・弱攻撃など

[ガード後+2Fでどれを先に選ぶか](pressure.md#dr5hk-guard)に戻れる。ヒット後は[中ライズ後の起き攻め](okizeme.md#after-ender)へ。

| 完全な入力 | 参考ダメージ | 追加コスト・条件 | 次状況 |
|---|---:|---|---|
| `2LK > 2LP:236MK` | **1,290** | D/S 0、攻略メモ値。届くこととヒット確認が前提 | [中ライズ](okizeme.md#after-ender) |
| `2LK > 5LP > 5LK:236MK` | **1,370** | D/S 0、3発つながる距離 | [中ライズ](okizeme.md#after-ender) |
| `2LP[CH] > 5MP~MK:236MK` | **1,930** | CH時 +6F、5MPが届くこと | [中ライズ](okizeme.md#after-ender) |
| `2MP > 5LK:236MK` | **1,860** | 5LKが届く距離。過去会話の参考値 | [中ライズ](okizeme.md#after-ender) |
| `2MP > 5MP~MK:236MK` | **2,480** | 5MPが届く距離。過去会話の参考値 | [中ライズ](okizeme.md#after-ender) |
| `5MP~MK:236MK` | **2,140** | 始動単体の攻略参考値。DR始動の合計とは異なる | [中ライズ](okizeme.md#after-ender) |
| `5MP~MK:214MP` | **1,930** | 同上 | [中フレア](okizeme.md#after-ender) |
| `2HP:214MP` | **1,700** | 同上 | [中フレア](okizeme.md#after-ender) |

全ルートが同じ始動・位置・ヒット条件で成立するわけではない。`236MK` ガード-23Fを入れ込むリスクは [小技のガード後の処理](pressure.md#dr5hk-guard) と合わせて読む。

<a id="route-shimmy"></a>
### シミー・投げ空振りへのPC反撃

[投げを空振らせた後の反撃選択](punish.md#shimmy)から接続する。`5MK[PC]` と `5HK[PC]` を一方に固定しない。

| 完全な入力 | 参考ダメージ | D/S・成立条件 | 次状況 |
|---|---:|---|---|
| `5MK[PC]:236HK > j.214LP` | **未実測** | D0、S+1。先端接続は未確認 | 成立すれば[弱空フレア後](okizeme.md#after-ender) |
| `5MK[PC]:236HK > j.214MP` | **未実測** | D0、S増減0。先端接続・高度を要確認 | 成立すれば[中空フレア後](okizeme.md#after-ender) |
| `5MK[PC]:214MP` | 未実測 | D0、強サンライズが届かない場合の候補 | [中フレア後](okizeme.md#after-ender) |
| `5HK[PC] > 5MP~MK:236MK` | **2,840** | D/S0、攻略メモ値。5MPの距離条件 | [中ライズ後](okizeme.md#after-ender) |

2026-08-03調整で `5MK[PC]` から強サンライズにつながるようになった。ただし `5MK` 始動の約2,140／2,770は他の始動からの推算であり、実測ダメージとしては採用しない。

<a id="route-punish"></a>
### 無敵技をガードした後の確定反撃

[何をガードしたら12Fの確定反撃が取れるか](punish.md#reversal)が前提。`2HP` が届くことと、打ち上げからの空中追撃条件を満たす必要がある。

| 反撃の完全な入力 | 参考ダメージ | D消費 | S増減 | ダウン後の次状況 |
|---|---:|---:|---:|---|
| `2HP[PC]:236HK > j.214LP` | **2,260** | 0 | +1 | [+25F → 前ステ後+5F](okizeme.md#after-ender) |
| `2HP[PC]:236HK > j.214MP` | **2,890** | 0 | 0 | [+49〜50F → 2前ステ後+9〜10F](okizeme.md#after-ender) |
| `5HP[PC] > DR > 2HP:236HK > j.214LP` | **2,391** | 1 | +1 | [+25F → 前ステ後+5F](okizeme.md#after-ender) |
| `5HP[PC] > DR > 2HP:236HK > j.214MP` | **2,769** | 1 | 0 | [+49〜50F](okizeme.md#after-ender) |
| `2HP[PC]:236HK > j.OD.214P > 236MK` | **3,925（1S）／4,180（2S）** | 2 | -1／-2 | [中ライズ型](okizeme.md#after-ender)。調整後の再実測は未確認 |
| `2HP[PC]:236HK > dl.j.MP > SA3` | **5,080** | 0（SA3消費） | 0 | SA3後、個別の状況を確認 |

弱空フレア2,260と中空フレア2,890の差は**630ダメージ**。後者の起き攻め時間は長いが、前者はS1回収する。OD型の3,925/4,180は調整前からの公開レシピ値であり、最新パッチの保証ではない。

<a id="route-stun"></a>
### 画面端BO・DIスタン

目標は[画面端BOの勝ち筋](strategy.md#win-plan)。必要なS・SA量、スタン中の入力、高度、相手残体力によって火力が変動するため、ここでは単一の「4割確定ルート」を固定しない。起き攻めへ移るなら[端のダウン後](okizeme.md#corner-loop)へ。

<a id="route-parts"></a>
## パーツ化の将来方針（現在は保留）

概念は **Route（技列）／Part（再利用する名前付きRoute）／Combo（条件・コスト・結果付き完全Route）**。

候補の役割は以下の4つ。

| 役割 | 意味 |
|---|---|
| `starter` | 始動側の再利用技列 |
| `linker` | 中継 |
| `ender` | 締め |
| `frag` | 役割を限定しない共通部分 |

- 全コンボを機械的に分割しない。
- `5MP~MK` のようなTC単体は基本直書き。
- 参照時の接続記号（`>`、`:`、`~`）は参照元Routeが所有する。
- 重複する短い技列より、**分岐点・変更理由・実戦の選択単位**を優先してPart化する。
- Part参照の循環は禁止。Partの複雑なパラメータ化は当面行わない。
- Partの同一性は展開後の技列と固有の成立条件で判断する。

## 参照

- [SF6 Lab: イングリッドのコンボ](https://sf6-lab.net/en/fighters/ingrid/combo)
- [UFD](https://ultimateframedata.com/sf6/ingrid)


## 追加参照・数値の取扱い

- [CAPCOM 2026-08-03 Ingrid調整](https://www.streetfighter.com/6/buckler/en/battle_change/20260803/ingrid) — `5MK` のPC/DRヒットから強サンライズへの接続など。
- [CAPCOM Ingridフレーム](https://www.streetfighter.com/6/character/ingrid/frame)／[UFD](https://ultimateframedata.com/sf6/ingrid) — 技発生、硬直差。
- [SF6 Lab：イングリッド2026年8月対応コンボ・起き攻め](https://sf6-lab.net/fighters/ingrid/combo) — +25/+38/+47/+50F、端投げ後、弾持続等の参考値。
- [スト6原典：コンボ](https://sf6-genten.com/character/ingrid/category/combo)、[起き攻め](https://sf6-ingrid.com/character/ingrid/category/okizeme-setplay) — ダメージとセットプレイ。
- [かくぶろ：ダメージ付きコンボ](https://takukakugamer.com/sf6-ingrid-combo/) — `2HP[PC]` 弱2,260／中2,890、`5HP[PC]` DR弱2,391、SA3 5,080等。
- [くそまゆげ：フィジカル・イングリッド論](https://note.com/kusomayuge/n/n79bb407272dc) — `DR > 5HK` の打撃・投げ、端投げ後、S回収型の運用。
- [コミュニティ攻略メモ](https://scrapbox.io/1cc/%E8%8B%B1%E6%A0%BC%E9%BA%97%E7%89%B9%28%E5%BF%AB%E6%89%93%E6%97%8B6%29%2F%E7%B6%93%E5%85%B8%E6%A8%A1%E5%BC%8F) — `DR > 5HK` の参考ダメージ、`5HK[PC]`・S消費型等。ユーザー実測とは区別する。

**未確定のまま残す項目**：`5MK[PC]:236HK` 始動の合計ダメージ／先端接続／実締めF、`DR > 5HK` の全距離での投げ・シミー成立、`236MP > 2HK` 合計ダメージ、ストック消費型の調整後再実測、すべてのセットプレイの距離別成立。これらは不明だからといって任意の推算値で埋めない。
