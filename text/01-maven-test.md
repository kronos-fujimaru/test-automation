# 自動テストツール

## 1. Mavenプロジェクトでの自動テスト

Mavenプロジェクトではテストコードは ***src/test/java*** のフォルダの中に作成します。***src/test/java*** と ***src/test/resources*** はMavenプロジェクトを作成するとデフォルトで用意されますが、Git経由でプロジェクトを取り込んだ場合、フォルダが消失している可能性があります。

<img src="../img/01-01.png" width="250">

そうした場合は、Configure Build Path（ビルドパスの構成）からテスト用のフォルダを作成してください。

### 1-1. testフォルダの作成

<img src="../img/01-02.png" width="1000">

- プロジェクトを右クリック > Build Path > Configure Build Path

<br>

<img src="../img/01-03.png" width="700">

- ***src/test/java*** と ***src/test/resources*** がないことを確認し、[Add Folder]ボタンをクリックする

<br>

<img src="../img/01-04.png" width="500">

- プロジェクト名を選択状態で、[Create New Folder]ボタンをクリックする

<br>

<img src="../img/01-05.png" width="700">

- Folder name欄に「**src/test/java**」と入力する
- [Finish]ボタンをクリックする

> 同様の手順で、***src/test/resources*** も作成します。

<br>

<img src="../img/01-06.png" width="500">

- 上画像のような構成になっていることを確認する

<br>

<img src="../img/01-07.png" width="700">

- src/test/java の ***Output folder*** をダブルクリックする

<br>

<img src="../img/01-08.png" width="700">

- ***Specific output folder*** を選択する
- テキストボックスに「**target/test-classes**」と入力する
- [OK]ボタンをクリックする

<br>

<img src="../img/01-09.png" width="700">

- ***Contains test sources*** をダブルクリックする

> 値が ***No*** から ***Yes*** に切り替わります。

> ***src/test/resources*** に対しても同様の手順で、Output folderとContains test sourcesを設定してください。

<br>

<img src="../img/01-10.png" width="700">

- 上画像のような構成になっていることを確認する

<br>

<a href="02-junit.md">>> 02. JUnitの実践</a>

<a href="../README.md">>> メニューへ</a>
