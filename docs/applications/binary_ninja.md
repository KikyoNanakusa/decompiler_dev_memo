# Binary Ninja
---
tags:
  - アプリケーション
---

# Binary Ninja

Binary NinjaはVector 35が開発する商用のリバースエンジニアリングプラットフォームです. 
GUIでのインタラクティブ解析に加え, Python APIによる自動化やプラグイン開発が重視されています. 
内部に中間表現(IL)を持ち, LLIL/MLIL/HLILといった階層的なILを通じて解析結果を整理します. 
デコンパイル結果はHLILを基盤として出力され, 比較的高性能です. 

- 公式サイト: [binary.ninja](https://binary.ninja/)

特徴として, 多段階のILを持つことが挙げられます. [IDA Pro](./ida.md)や[Ghidra](./ghidra.md)が単一の単一の中間表現しか持たないのに対して, Binary Ninjaは多段階のILを持っているため, 異なるILを使って抽象度を変えた解析を行うことができます. 
これらのILはBNIL(Binary Ninja Intermediate Language)と総称され, 公式ドキュメントで詳しい解説を読むことができます. 

- [BNIL Documentation](https://docs.binary.ninja/dev/bnil-overview.html)