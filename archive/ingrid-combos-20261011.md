# 旧メモ：イングリッド55本のコンボ列挙（2026-10-11）

これは会話中に一度列挙した**移行用の原文メモ**。一覧に、コスト・ストック条件・接続・技名が不整合な記述が混在しているため、**そのまま実戦用のコンボ集として扱わない**。修正後の採用ルートは [docs/ingrid/combos.md](../docs/ingrid/combos.md) を優先する。

原文での列挙順・番号を概ね維持する。単発の技列が本当にコンボとして成立するかの履歴や評価項目は作らない。

```text
# 通常・弱攻撃始動
01  2LP:2LP:236MK
02  2LK > LP > LK:236MK
03  LP:LP:236MK
04  MP~MK:236MK
05  2MP > LK:236MK
06  2MP > MP~MK:236MK
07  5MK:236MP
08  2MK:236MP
09  2HP:236MP
10  5MK:214MP:236236P

# DRC始動
11  2MK:DRC > HK > MP~MK:236MK
12  2MK:DRC > HK > MP~MK:214MP
13  2MK:DRC > HK > MP~MK:OD.214P > 2KKK > 236MK
14  2MK:DRC > HK > MP~MK:214HP > 6KKK
15  5MK:DRC > 2HP:236HK > j.214LP
16  5MK:DRC > 2HP:236HK > j.214MP
17  2MP:DRC > 2HP:236HK > j.214LP
18  2MP:DRC > 2HP:236HK > j.214MP
19  2HP:DRC > 2HP:236HK > j.214LP
20  2HP:DRC > 2HP:236HK > j.214MP

# CH・PC始動
21  HK > 2LP:236MK
22  HK[CH] > MP~MK:236MK
23  HK[PC] > MP~MK:236MK
24  2LP[CH] > MP~MK:214MP
25  2MP[CH] > MP~MK:214MP
26  HP[PC] > DR > 2HP:236HK > j.214LP
27  2HP[PC]:236HK > j.214MP
28  LK[CH]:DRC > 2MP > MP~MK:236MK
29  LK[PC]:DRC > MK:236HK > j.214LP

# 飛び道具・空中ヒット
30  236HP[Air Hit] > DR > MP~MK:236MK
31  236HP[Air Hit] > DR > 2HP:236MK
32  6HP:j.214MP
33  6HP:j.OD.214P > DR > 2HP:236HK > j.214LP
34  6HP:j.OD.214P > 6HP:j.OD.214P > 236236P
35  5MK:OD.214P > 66 > 236HK > j.214MP
36  2MK:214HP > 6KKK

# DI・画面端・飛び込み
37  DI[PC] > DR > 2HP:236HK > j.214LP
38  DI[PC] > 66 > 4HP~HP:214MP
39  DI[PC] > 4HP~HP:214MP > 236MK [Corner]
40  DI[Wall] > 4HP~HP:214MP > 236MK
41  DI[Wall] > 4HP~HP:OD.214P > 2KKK > 236MK [2S]
42  j.HP > HK > 2LP:236MK
43  j.MK > 2MP > LK:236MK
44  j.HP > 2HP:OD.214P > 66 > 4HP~HP > 6KKK [2S]
45  [Stun] 214LP(h) > 6HP:j.OD.214P > 4HP~HP:236HP > 236MK

# SA2
46  MP~MK:214214MP > MP~MK:214LP(h)
47  OD.236K:214214HP > 2HP:236MK > 214LP(h) > 236HK
48  OD.236K:214214HP > 2HP:236MK > 214LP(h) > 236HK > j.214HP > DR > 4MK~HP:236MK
49  OD.236K:214214HP > 2HP:236MK > 214LP(h) > 236HK > j.214HP > DR > 4MK~HP:214LP
50  HK:214214HP > MK:236MK > 214LP(h) > 66 > 4HP~HP > 6KKK
51  2HP[PC]:214214MP > 2HP:236LK > 214LP(h) > 214HP > OD.214P > 6KKK > 236LK

# SA1・SA3
52  HK > LP:DRC > LP > MP~MK:OD.214P > 236HK > j.214MP:236236K
53  2HP[PC]:236HK > dl.j.MP > 236236P
54  HP[PC] > 6HP:j.OD.214P > DR > 2HP:OD.214P > 66 > 66 > OD.236K:236236P

# 端SA2
55  [Corner, 0S] 2LP:2LP:OD.236K:214214HP > 2HP:236MK > 214LP(h) > 236HK > j.OD.214P > DR > 4MK~HP:236MK
```

## この一覧から引き継いだ重要な修正

- **`214HP > 2KKK` を通常中央コンボの前提にしない**。実機で不成立との指摘があり、OD版との混同を避ける。
- サンバニッシュ入力は `4KKK / 6KKK / 2KKK`。以前の `5KKK` は採用しない。
- 1S/2Sの**開始必要量と消費量**、Dゲージ消費を区別する。
- `214LP` でのS回収など、コンボ後のセットプレイは連続ヒット技列と分ける。
- 戦略上の必要性が確定するまでは、55本という件数を増やすことを目的にしない。
