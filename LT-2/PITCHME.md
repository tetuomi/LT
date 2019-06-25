# 第2会LT会
### 近藤　徹多

---

## 分割コンパイル

---
## 分割コンパイルとは <br>
### プログラムを複数のファイル<br>
### に分割し,コンパイルして， <br>
### リンクさせることで，<br>
### ひとつの大きなプログラムを作成すること <br>

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

---?code=LT-2/assets/splitcompile.text
@[1-2](hello.h hello.c main.c があります)
@[3](hello.c main.c をコンパイルだけしてオブジェクトファイルを生成)
@[4-5](オブジェクトファイルが生成された)
@[6](オブジェクトファイルをリンクして,a.outを生成)
@[7-8](a.out が生成された)
@[9-10](ちゃんと実行できます)

---

## めんど...

---
@transition[zoom]
## * (cmake) を使ってみよう
