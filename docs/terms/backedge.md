---
tags:
  - 用語
  - グラフ理論
  - 書きかけの項目
---

# Backedge

**Backedge**は, グラフ理論における概念の一つで, ループの検出などに用いられるものです. 
Backedgeは以下のように定義されます. 

Backedgeとは, あるノード$u$からノード$v$へのエッジであり, かつ, $v$が$u$を[支配(dominate)](./dominator.md)するものである.

![Backedge Example](../img/backedge.png)

図における赤い辺がバックエッジであり, 定義に出現する$u$が図におけるtailノード, $v$が図のheadノードにあたります. 
グラフにおけるループは単にバックエッジの存在によって検出することができます. 

## Backedgeを検出するアルゴリズム

TODO...

