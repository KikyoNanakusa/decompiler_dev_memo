---
tags:
  - アプリケーション
---

# Ghidra

![Ghidra](https://upload.wikimedia.org/wikipedia/commons/a/a3/Ghidra_Logo.png)

Ghidraは米国NSA(アメリカ国家安全保障局)が開発し, オープンソースとして公開されているリバースエンジニアリングフレームワークです. 
機能の一つとしてデコンパイラを搭載しています. 
GUIアプリケーションとして配布され, 解析プロジェクト単位でバイナリを読み込み, ディスアセンブルやデコンパイル, 解析結果の可視化を行います. 
Windows/macOS/Linuxなど主要な環境で動作し, 研究用途から実務まで幅広く利用されています. 
Ghidraのデコンパイラは, CPUごとに定義されたSLEIGH仕様から生成される[P-code](https://ghidra.re/ghidra_docs/languages/html/pcoderef.html)を内部表現として扱い, C言語に近い高水準の疑似コードを出力します. 

- リポジトリ: [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra)

## 余談

近年ではGhidraとAI Agentを接続するGhidra MCPが登場しており解析の自動化が進んでいるらしい. 
大元のGhidra MCPはメンテナンスが微妙らしく, [Pinkさん](https://x.com/PINKSAWTOOTH)がフォークしたバージョンがいいらしい. 

- Pink氏のGhidra MCP: [pinksawtooth/GhidraMCP](https://github.com/pinksawtooth/GhidraMCP)
