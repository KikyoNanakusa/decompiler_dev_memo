---
tags:
  - 用語
---

# CTI (Control Transfer Instruction)

CTI(Control Transfer Instruction)とは, 日本語では制御転送命令と呼ばれ, プログラムにおける命令の実行順序を変更する命令のことです.
CTIには, Conditional CTI(条件付き制御転送命令)とUnconditional CTI(無条件制御転送命令)の2種類があります.

## Unconditional CTI

Unconditional CTIは, 条件に関係なく命令の実行順序を変更する命令です.
例えばx86-64アーキテクチャにおける`JMP`命令はUnconditional CTIの一つで, 指定されたアドレスにプログラムの実行位置を変更します.
プログラムの実行位置がUnconditional CTIに到達すると, ジャンプは必ず実行されるため, 遷移先は1つだけです.

`CALL`命令や`RET`命令もUnconditional CTIに分類されます.

## Conditional CTI

Conditional CTIは, 条件に基づいて命令の実行順序を変更する命令です.
例えばx86-64アーキテクチャにおける`JE`(Jump if Equal)命令はConditional CTIの一つで, 直前の比較命令の結果が等しい場合に指定されたアドレスにプログラムの実行位置を変更します.

Conditional CTIは, 条件によって遷移を実行するか否かが異なるため, 遷移先が2つ存在します.
1つは, 命令のオペランドで指定されたジャンプ先の命令で, もう1つは単にConditional CTIの次に配置される命令です.
Condtional CTIの次に配置される命令は遷移先として**Fall-through**と呼ばれることがあります.

```asm
0x1000: je 0x2000
0x1007: mov eax, 1 ; Fall-through
...
0x2000: mov eax, 2 ; ジャンプ先
```
