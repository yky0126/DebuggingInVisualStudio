# VisualStudioを用いたデバッグ

# 概要
VisualStudioを用いたデバッグ方法についてまとめて下さい。
条件は以下の通り。

  ## ブレイクポイント
  F9キーを押すか、Debug > Toggle Breakpiont メニューをクリック
  
  ラインナンバーの左に付けられた赤い丸印をブレイキングポイントという
  
  [![Image from Gyazo](https://i.gyazo.com/7bf7412fad94bac821345992abad27bc.png)](https://gyazo.com/7bf7412fad94bac821345992abad27bc)
  
  F5キーを押すか、Debug > Start Debuggingを選択するとデバッグモードに進入(ブレイクポイントへ移動)
  
  [![Image from Gyazo](https://i.gyazo.com/87a507e3e5043c79c1c9f671ecb0823e.png)](https://gyazo.com/87a507e3e5043c79c1c9f671ecb0823e)
  
  F11キーを押すことで一行づつ実行することができる
  
  F11キーはコードを一行づつ移動しながら変数の変化を教えてくれる(Step In)
  
  [![Image from Gyazo](https://i.gyazo.com/c427e3a6aff05a37e01133aafdf72fcb.png)](https://gyazo.com/c427e3a6aff05a37e01133aafdf72fcb)
  
  F10キーはそのまま一行を飛び越える(Step Over) EX) printf()のようなライブラリ関数がある場合はF10キーを利用
  
  [![Image from Gyazo](https://i.gyazo.com/81e6be40b045b6d745644c142079b938.png)](https://gyazo.com/81e6be40b045b6d745644c142079b938)
  
  ライブラリ関数でF10キーを押してしまった場合、EscapeするためにはShift + F11キーでEscape可能 (Step Out)
  
  [![Image from Gyazo](https://i.gyazo.com/3c0bf53a3a91438b6079f0f4a259e8af.png)](https://gyazo.com/3c0bf53a3a91438b6079f0f4a259e8af)
  
  ## Step over/in/out
  
  Step Over : 現在矢印がかかっている行を実行してコード上の次の列に移る(F10)
  
  Step In : 矢印がかかってる行の関数が定義された範囲に入ること(F11)
  
  Step Out : 矢印がかかってる行の関数を呼び出した範囲外に出ること(Shift + F11)
  
  ## 自動変数・ローカル変数ウィンドウ
  
  デバッグ中の変数の内容を確認する手段として ウォッチ・自動変数・ローカルのウィンドウが用意されている
  
  ローカル変数ウィンドウではメソッド内限定の変数の内容が自動的に表示される
  
  自動変数ウィンドウでは現在実行中の行に関係のある変数だけが表示される(現在の状況を知ることが用意)
  
  [![Image from Gyazo](https://i.gyazo.com/911041b1921bd4cb2c1ddb7c1a4af8b8.png)](https://gyazo.com/911041b1921bd4cb2c1ddb7c1a4af8b8)
  
  ## ウォッチ式
  特定の変数をずっと監視したい場合に役立つ、例えばクラスのメンバ変数を常時監視したいなど、ウォッチウィンドウに追加すると
  
  （追加するには、コード・エディタ上の変数名を選択してドラッグ＆ドロップするか、［ウォッチ］ウィンドウに手動で変数名を記述する）
  
  、いつでもその変数の内容がウィンドウに表示される
  
  ## データブレイクポイント
  特定のオブジェクトのプロパティが変更されたときに実行を中断する機能
  
  データブレイクポイントの設定するには
  
  自動変数 、ウォッチ、またはローカルウィンドウで、プロパティを右クリックし、値が変更されたときに中断のメニューを選択
  
  ## メモリウィンドウ
  
  デバッグを通して実際メモリーにどのように割り当てられるか確認できる
  
  デバッグ中：デバッグ(D) -> ウィンドウ(W) -> メモリー(M)
  
  アドレス欄にアドレスを入れたり、ポイント、＆一般変数名などを入力すれば該当アドレスのメモリーを直接確認できる
  
  [![Image from Gyazo](https://i.gyazo.com/cd07808c7eddd709ae066f9c7b3f33fd.png)](https://gyazo.com/cd07808c7eddd709ae066f9c7b3f33fd)
  
  ## コールスタック(呼び出し履歴)
  
  コールスタックを使用すると現在呼び出し履歴にある関数の呼び出しやプロシージャ呼び出しを表示できる
  
  メソッドおよび関数が呼び出されている順番が表示され,アプリの実行フローを調査して理解するときに用意である
  
  ## イミディエイトウィンドウ
  
  イミディエイトウィンドウは、ステートメントの実行、変数値の出力のために使用
  
  現在選択されているプロジェクトをビルドして使用することで式を評価
  
  イミディエイトウィンドウを表示するには : デバッグ(D) -> ウィンドウ(W) -> イミディエイト(I)　か　Ctrl + Alt + I　もしくは、
  
  Debug.Immediate　と入力することで表示できる
  
  [![Image from Gyazo](https://i.gyazo.com/0b187d63b209a7091594803ce5364d79.png)](https://gyazo.com/0b187d63b209a7091594803ce5364d79)
  


## 提出期限
プログラムチェック実習の前期最終授業日(7月10日？)/

##

https://github.com/yky0126
