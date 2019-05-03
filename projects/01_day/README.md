# PCの仕組みからアセンブラ入門まで

OSXのバイナリエディタを用意する。

[sandai/30nichideosjisaku: 『30日でできる！ OS自作入門』川合 秀実氏(著)のMacOSX開発環境を整えることができます](https://github.com/sandai/30nichideosjisaku)は[0xED](http://www.suavetech.com/0xed/0xed.html)が使いやすかったといっているがLastCommitが`7 years ago`なのでググってでた[Hex Friend](https://itunes.apple.com/jp/app/hex-fiend/id1342896380?mt=12)を使うことにした。

まずバイナリを写経しろというのだが何を見ればいいかわからない。コードと照らし合わせてみると `furoku/projects/01_day/helloos0` **がそれっぽい**。

```bash
helloos0 (master): xxd helloos.img | head -10
00000000: eb4e 9048 454c 4c4f 4950 4c00 0201 0100  .N.HELLOIPL.....
00000010: 02e0 0040 0bf0 0900 1200 0200 0000 0000  ...@............
00000020: 400b 0000 0000 29ff ffff ff48 454c 4c4f  @.....)....HELLO
00000030: 2d4f 5320 2020 4641 5431 3220 2020 0000  -OS   FAT12   ..
00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
00000050: b800 008e d0bc 007c 8ed8 8ec0 be74 7c8a  .......|.....t|.
00000060: 0483 c601 3c00 7409 b40e bb0f 00cd 10eb  ....<.t.........
00000070: eef4 ebfd 0a0a 6865 6c6c 6f2c 2077 6f72  ......hello, wor
00000080: 6c64 0a00 0000 0000 0000 0000 0000 0000  ld..............
00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
helloos0 (master): 
```