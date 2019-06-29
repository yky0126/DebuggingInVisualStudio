# VisualStudioを用いたデバッグ

## 概要
VisualStudioを用いたデバッグ方法についてまとめて下さい。
条件は以下の通り。

* 個人のリポジトリを各自作成し、以下の項目について **「どんな場合に使用すれば良いか」「どのように使用すれば良いか」「なぜそれを用いると効果的なのか」** をREADMEに記載すること。
  * ブレイクポイント\
  F9キーを押すか、Debug > Toggle Breakpiont メニューをクリック\
  ラインナンバーの左に付けられた赤い丸印をブレイキングポイントという\
  F5キーを押すか、Debug > Start Debuggingを選択するとデバッグモードに進入(ブレイクポイントへ移動)\
  F11キーを押すことで一行づつ実行することができる\
  F11キーはコードを一行づつ移動しながら変数の変化を教えてくれる(Step In)\
  F10キーはそのまま一行を飛び越える(Step Over) EX) printf()のようなライブラリ関数がある場合はF10キーを利用\
  ライブラリ関数でF10キーを押してしまった場合、EscapeするためにはShift + F11キーでEscape可能 (Step Out)
  * Step over/in/out\
  Step Over : 現在矢印がかかっている行を実行してコード上の次の列に移る(F10)\
  Step In : 矢印がかかってる行の関数が定義された範囲に入ること(F11)\
  Step Out : 矢印がかかってる行の関数を呼び出した範囲外に出ること(Shift + F11)
  * 自動変数・ローカル変数ウィンドウ\
  デバッグ中の変数の内容を確認する手段として ウォッチ・自動変数・ローカルのウィンドウが用意されている\
  ローカル変数ウィンドウではメソッド内限定の変数の内容が自動的に表示される\
  自動変数ウィンドウでは現在実行中の行に関係のある変数だけが表示される(現在の状況を知ることが用意)
  * ウォッチ式\
  特定の変数をずっと監視したい場合に役立つ、例えばクラスのメンバ変数を常時監視したいなど、ウォッチウィンドウに追加すると
  （追加するには、コード・エディタ上の変数名を選択してドラッグ＆ドロップするか、［ウォッチ］ウィンドウに手動で変数名を記述する）、
  いつでもその変数の内容がウィンドウに表示される
  * データブレイクポイント\
  特定のオブジェクトのプロパティが変更されたときに実行を中断する機能\
  データブレイクポイントの設定するには\
  自動変数 、ウォッチ、またはローカルウィンドウで、プロパティを右クリックし、値が変更されたときに中断のメニューを選択
  * メモリウィンドウ\
  デバッグを通して実際メモリーにどのように割り当てられるか確認できる\
  デバッグ中：デバッグ(D) -> ウィンドウ(W) -> メモリー(M)\
  アドレス欄にアドレスを入れたり、ポイント、＆一般変数名などを入力すれば該当アドレスのメモリーを直接確認できる
  * コールスタック(呼び出し履歴)\
  コールスタックを使用すると現在呼び出し履歴にある関数の呼び出しやプロシージャ呼び出しを表示できる\
  メソッドおよび関数が呼び出されている順番が表示され,アプリの実行フローを調査して理解するときに用意である
  * イミディエイトウィンドウ
  イミディエイトウィンドウは、ステートメントの実行、変数値の出力のために使用\
  現在選択されているプロジェクトをビルドして使用することで式を評価\
  イミディエイトウィンドウを表示するには : デバッグ(D) -> ウィンドウ(W) -> イミディエイト(I)　か　Ctrl + Alt + I　もしくは、
  Debug.Immediate　と入力することで表示できる
  
  
  
* 画像・GIFアニメーション・テーブル・ハイパーリンク等、Markdownの機能を用いて読み易いものとなるよう工夫すること。
* 各自のリポジトリのトップページのURLを、このREADMEの最下部に記載すること。

## 提出期限
プログラムチェック実習の前期最終授業日(7月10日？)
