# ナンプレ問題自動生成
![NP0-Heart](https://user-images.githubusercontent.com/63762160/111978921-cfca1b80-8b47-11eb-9dad-c46e14e9a598.png)　　
![NP0-Heart-2](https://user-images.githubusercontent.com/63762160/111979291-3c451a80-8b48-11eb-8315-482d9a7584ff.png)

## ナンプレ自動生成は解くより簡単

ナンプレの問題をコンピュータで解いたことがある人は多いかと思います。
でも、問題を作った人は非常に少ないのではないでしょうか。
ネット上に多数のナンプレソルバーが存在し、解けない問題の写真を撮れば解を教えてくれるアプリなどもあります。
でも、問題を提供してくれるアプリは少ないです。たとえば上のハートのパターンを与えると問題を作ってくれます。
問題の自動生成は、人工知能の進化計算という方法を使えば、解くより作るほうが簡単（プログラムが短い！）なのです。

## プログラムについて

ナンプレの問題を自動生成するプログラムを公開します。
Javaで750行ほどの非常に短いプログラムです。
問題の数字が17、18個の問題も作ることができます。
問題作成時間も、ほとんど数秒以内です。

なお、本プログラムは、ナンプレの自動生成はどうすればできるかのサンプルを提供するものです。
そのため、GUIはなく、ヒントの位置を指定したテキストファイル（パターンファイル）を読み、問題を自動生成します。
dataフォルダの中には、ヒント数18〜24個の問題とパターンのファイルが入っているので、すぐに確認できるでしょう。

NP.jar　はJavaの実行ファイルです。
dataに入っているファイルを使って、実際に問題を解いたり作ったりできます。
$ java -jar NP.jar -s HeartQ.txt
$ java -jar NP.jar -g HeartP.txt
500問を連続で解いたり作ったりするためのデータファイルも入っています。
どのように動くかは、動画を見てください。
とても小さなプログラムですので、Raspberry Pi でも動きます。

## ライセンス

色々なことに利用しやすいように、MITライセンスにて提供します。
学術利用、商業利用が自由にできます。利用の際には、本GitHubの紹介をしていただければ嬉しいです。

## 発展

説明書にもありますが、本プログラムは進化計算による自動生成のコア部分だけを提供しています。
機能追加は、プログラミング技術の向上はもちろん、大学での課題、卒研にも利用できると思います。

パズルの世界は、アルゴリズムの宝庫です。
進化計算を理解すると、さまざまな問題を解決できるようになります。
産業界でも、人間には複雑過ぎる問題を解くのに利用されています。
