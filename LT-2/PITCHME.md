# 第2会LT会
### 近藤　徹多

---

## 分割コンパイル

---
## **分割コンパイル**とは <br>
### プログラムを複数のファイルに<br>
### 分割し,コンパイル,リンク， <br>
### させることで，<br>
### ひとつのプログラムを作成すること <br>

---
@transition[convex]
### さっそくやってみよう<br>
#### みんな大好きhelloっていうだけの <br>
#### プログラムを考えます
---

### まずはコマンドで

---
 
(デレクトリ下)/ <br>
|-hello.h <br>
|-hello.c <br>
|-main.c

---?code=LT-2/assets/hello.h
hello.h

---?code=LT-2/assets/hello.c
hello.c

---?code=LT-2/assets/main.c
main.c

---?code=LT-2/assets/splitcompile.txt
@[1-10](コマンドでやってみた)
@[1-2](hello.h hello.c main.c があります)
@[3](hello.c main.c をコンパイルだけする)
@[4-5](オブジェクトファイルが生成された)
@[6](オブジェクトファイルをリンクする)
@[7-8](a.out が生成された)
@[9-10](ちゃんと実行できます)

---
@transition[zoom]
## 次は @color[#b22222](cmake) を使ってみる

---

(デレクトリ下)/ <br>
|-CmakeLists.txt <br>
|-hello.h <br>
|-hello.c <br>
|-main.c

---?code=LT-2/assets/CMakeLists.txt
@[1-8](CMakeLists.txt)
@[1](cmakeのバージョン指定)
@[3](プロジェクト名と使用する言語を設定)
@[5-8](a.outという実行ファイルをmain.cとhello.cから作成)

---

やり方
* mkdir build |
* cd build |
* cmake .. |
* make |

---?code=LT-2/assets/results-cmake.txt
@[1-23](cmake やってみた)
@[1](directory を作成)
@[2-13](移動してcmake)
@[14-19](make)
@[20-21](a.out という実行ファイルができている)
@[22-23](ちゃんと実行できます)

---

## まとめ
* CMakeLists.txt を作る |
* mkdir build |
* cd build |
* cmake .. |
* make |

---

## 現場からは以上です

---

