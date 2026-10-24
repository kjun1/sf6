# SF6 攻略ノート

Street Fighter 6 の戦略・技データ・状況判断・コンボを、**勝ち筋から逆算して**整理する個人用リポジトリ。

## イングリッド：状況から読む

**[とりあえずメモ（自由記入）](docs/ingrid/memo.md)** — 分類前の気づき・対戦メモ・トレモで確認したいことを一旦書く場所。

行動が通った後は、**その結果が書かれている箇所から次の状況へ進む**。文書を最初から順番に読み切る必要はない。

1. [基本戦略](docs/ingrid/strategy.md) — BO・画面位置・D/S運用など、何を目指すか
2. [地上戦](docs/ingrid/neutral.md) — 接触前：距離・相手の行動・牽制・DR止め
3. [接触後の攻め](docs/ingrid/pressure.md) — 技を当てた／ガードさせた後：打撃・投げ・シミーのジャンケン
4. [確定反撃](docs/ingrid/punish.md) — 投げ空振りや無敵技を咎めた後：反撃の選び方
5. [起き攻め](docs/ingrid/okizeme.md) — 投げ・コンボでダウンを取った後：再接近、弾重ね、S回収
6. [コンボと記法](docs/ingrid/combos.md) — **技列・ダメージ・必要S・D消費の正本**
7. [技データ](docs/ingrid/moves.md) — **通常技・必殺技の発生や硬直差の正本**

## 一つの状況から次の状況へ

[地上戦](docs/ingrid/neutral.md)で `DR > 5HK` に接触したら、[ヒット・ガード別の攻め](docs/ingrid/pressure.md#dr5hk)を見る。ヒットしたら[コンボ](docs/ingrid/combos.md#route-dr5hk)、ガードされたら[+2Fからの選択](docs/ingrid/pressure.md#dr5hk-guard)へ進む。

ガード後に投げが通れば[投げ後の起き攻め](docs/ingrid/okizeme.md#after-throw)、シミーが通れば[シミー確定反撃](docs/ingrid/punish.md#shimmy)、無敵技をガードすれば[ガード後確反](docs/ingrid/punish.md#reversal)。コンボでダウンを取ったら[締め後の起き攻め](docs/ingrid/okizeme.md#after-ender)から次の行動を探す。画面端で[強化サンフレアを通してS回収](docs/ingrid/okizeme.md#corner-loop)した後も、[端の+4F読み合い](docs/ingrid/pressure.md#corner-pressure)へ戻る。

相手の択に「勝つ行動」の対応は、**相手の次の行動を見てから正解を選べるという意味ではない**。各択の勝敗・リターンを整理したジャンケンとして扱う。

## 編集・保存方針

- 対戦中の**判断基準**を優先し、コンボの本数を増やすこと自体を目的にしない。
- 確認できた数値、使用者の戦略仮説、条件付きのルートを混同しない。
- コンボは先に完全表記で蓄積する。Part参照による省略化は、全体が揃ってから行う。
- 個別の検証履歴・検証ステータスは管理しない。
- コンボの定義・数値は `combos.md`、技性能は `moves.md` に集約する。状況別の文書は、その情報へ**文章の遷移位置でリンク**する。
- フレーム値・状況依存のセットプレイはパッチで変わるため、参照元と想定条件を明記する。
- 元の `corner.md` と `decision-playbook.md` は [移行前スナップショット](archive/ingrid-before-restructure-20261024/README.md) に保全。旧55コンボメモも `archive/` に保存。

## 主な参照資料

- [Ultimate Frame Data — Ingrid](https://ultimateframedata.com/sf6/ingrid)（通常技・必殺技のフレーム）
- [SF6 Frame Data Search — Ingrid](https://frame-search.com/?character_name=INGRID&lang=en-us)（ガード時のDゲージ減少量）
- [SF6 Lab — Ingrid Combos & Okizeme](https://sf6-lab.net/en/fighters/ingrid/combo)（コンボ・起き攻め）
- [スト6原典 — イングリッド](https://sf6-ingrid.com/character/ingrid)（戦術・セットプレイ）

初期の整理は2026-10-12、状況別の再構成は2026-10-24時点の議論に基づく。
