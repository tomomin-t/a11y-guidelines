.. _exp-screen-reader-check-ios-voiceover:

#######################################
iOS VoiceOverを用いたチェックの実施方法
#######################################

iOS用スクリーン・リーダーのVoiceOverの推奨設定の方法、基本的な使い方と基本的なチェックの実施方法について記します。

なお、macOSにも同名のスクリーン・リーダーが標準搭載されていますが、iOSのVoiceOverとはまったくの別物です。
本稿ではiOSのVoiceOverについてのみ記、「VoiceOver」という記述はiOS VoiceOverを差します。

本稿ではごく一部の機能や設定について紹介しています。より詳しくは、Appleが提供するiPhoneユーザガイドの「 `iPhoneのアクセシビリティ機能を使ってみる <https://support.apple.com/ja-jp/guide/iphone/iph3e2e4367/16.0/ios/16.0>`_ 」を参照してください。VoiceOverに加えて、その他のアクセシビリティー関連機能についても詳しく紹介されています。

**********
起動と終了
**********

VoiceOverの起動と終了の方法はいくつかありますが、一時的に有効にしたり、有効/無効を切り替えながら使うような場合は、以下の設定をすると便利です。

1. 「設定」アプリ、 :menuselection:`アクセシビリティ` をタップ
2. この画面最下部の :menuselection:`ショートカット` をタップ
3. VoiceOverが選択された状態にする

この設定を行うことで、ホーム・ボタン（ホーム・ボタンがない機種の場合はサイド・ボタン）を素早く3度押して、VoiceOverの有効/無効を切り替えることができるようになります。

********
推奨設定
********

以下、アクセシビリティー・チェック実施の観点で推奨される設定を記します。

ヒントの読み上げ
================

選択されているオブジェクトについて、操作方法のヒントを読み上げるかどうかの設定です。

設定の場所
   「設定」アプリ、 :menuselection:`アクセシビリティ --> VoiceOver --> 詳細度`
推奨設定
   「ヒントを読み上げる」をオンにする

ローター
========

後述するローター・ジェスチャーによって選択できる設定項目を設定します。

設定の場所
   「設定」アプリ、 :menuselection:`アクセシビリティ --> VoiceOver --> ローター`
推奨設定
   *  「見出し」を選択
   *  その他、必要に応じてよく使う項目を選択し、使うことがないものの選択を解除

句読点の読み上げ
================

左右方向へのフリック操作で読み上げを実行する際などの、句読点の読み上げ方を設定します。

設定の場所
   「設定」アプリ、 :menuselection:`アクセシビリティ --> VoiceOver --> 詳細度 --> 句読点および記号`
推奨設定
   「一部」を選択

.. _exp-sr-iosvo-multilingual-setting:

多言語読み上げが可能な設定
==========================

読み上げるコンテンツの言語に応じて、読み上げに用いる音声合成エンジンをその言語用のものに切り替えられるようにするための設定です。

設定の場所
   「設定」アプリ、 :menuselection:`アクセシビリティ --> VoiceOver --> 読み上げ`
推奨設定
   *  「言語を検出」をチェック
   *  「ローターで選択可能な言語」に、日本語と英語がある状態（いずれかがない場合は、「新しい言語を追加」をタップして追加）
   *  この状態で、ローター・ジェスチャーで「言語」を選択し、1本指の上または下方向へのフリックで「デフォルト（日本語）」を選択

VoiceOverの読み上げ内容の表示
=============================

VoiceOverが読み上げる内容を、画面下部に表示する設定です。

設定の場所
   「設定」アプリ、 :menuselection:`アクセシビリティ --> VoiceOver`
推奨設定
   「キャプションパネル」をチェック

**************
基本的な使い方
**************

VoiceOver有効時に使われることが多い、基本的なジェスチャーを以下に示します。

.. _exp-sr-iosvo-one-finger-horizontal-flick:

1本指による右および左方向へのフリック
=====================================

フォーカスを次（右フリック）または前（左フリック）のオブジェクトに移して、そのオブジェクトを読み上げます。

画面の先頭のオブジェクトが選択されているときに左フリック、または画面の末尾のオブジェクトが選択されているときに右フリックすると、「ポン」という効果音が再生され、選択されているオブジェクトが読み上げられます。

この方法で画面の内容を読み上げさせることでチェックを実施する場合、以下が基本的な手順です：

1. 画面の先頭（普通は左上）のオブジェクトにタッチして選択された状態にする
2. 左フリックをしてそれ以上前にオブジェクトが存在しないことを確認（フリック時に「ポン」という効果音が再生され、選択されているオブジェクトが読み上げられる）
3. 左方向にフリックして別の内容が読み上げられる場合は、先頭のオブジェクトに到達するまで左フリック
4. そこから画面の末尾に到達するまで、読み上げられる内容を確認しながら右フリックを繰り返す

1本指によるダブルタップ
=======================

上述の1本指による左右方向へのフリックを行うことで、画面上のオブジェクトのいずれかが選択された状態になります。
また、画面上の任意のオブジェクトを1本指でタップすることでも、そのオブジェクトが選択された状態になります。

画面上のオブジェクトが選択された状態のとき、画面上の任意の場所を1本指で素早く2度タップ（ダブルタップ）すると、そのオブジェクトがアクティベートされます。すなわち、VoiceOverが有効になっているときのダブルタップは、VoiceOverが無効になっているときのタップ操作に相当します。

.. _exp-sr-iosvo-one-finger-vertical-flick:

1本指による上および下方向へのフリック
=====================================

後述するローター・ジェスチャーで設定された内容に基づいて、読み上げ、フォーカスの移動、設定の変更などの操作をすることができます。

例えば、ローターの設定が「文字」のときは、1本指の下方向ーのフリックで次の文字、上方向ーのフリックで前の文字に移動して、その文字を読み上げます。
ローターで「単語」や「行」を選択すると、移動の単位がそれぞれ単語や行に変わります。

また、ローターの設定が、「見出し」、「表」、「ボタン」などの場合は、1本指の下/上方向へのフリックで、次/前の当該オブジェクトに移動して読み上げます。
「読み上げ速度」、「言語」などの場合は、1本指の上下方向へのフリックで、当該の設定値を変更します。

ローター・ジェスチャー
======================

ローター・ジェスチャーは、2本の指でつまみを回すようなジェスチャーです。
コンパスで円を描くようなイメージです。

ローターの設定に関しては、前述の推奨設定も参照してください。

スクロール
==========

スクロールは、3本指によるフリックで行います。

縦長の画面でのスクロールは3本指による上または下方向へのフリックで縦方向にスクロールすることができます。
また、例えばホーム画面で画面を切り替えるような場合は、3本指による右または左方向へのフリックで実行することができます。

その他の3本指によるフリック操作
===============================

画面上部のステータス領域に1本指で触れて、この領域に表示されているものが選択されている状態のとき、以下の操作が可能です。

画面の任意の場所を3本指で下方向にフリック
   通知センターの表示
画面の任意の場所を3本指で上方向にフリック
   コントロール・センターを表示

また、「引き下げて更新」のジェスチャーが使用できる場面では、VoiceOver有効時には更新対象が表示されている部分のどこかが選択された状態で3本指による下方向へのフリック操作で、更新を実行することができます。

ホーム画面への移動
==================

ホーム・ボタンを搭載していない機種の場合、以下の手順でホーム画面へ移動します。

1. 画面下端に1本指で触れる。
2. そのまま指を離さず、上方向に指を動かす。
3. 振動を1度感じたら、指を離す。

なお、ここで指を離さず再度振動感じるまで指を動かしてから離すと、Appスイッチャーが表示されます。

******************************************
戸惑わないために知っておきたいジェスチャー
******************************************

以下に挙げる操作は、意図せずに実行して戸惑うことが多い操作です。
チェックの際に使うことはあまりありませんが、事前に知っておくことでうっかりこれらの操作を実行してしまっても適切に対応することができるはずです。

読み上げのオン/オフ
===================

3本指でダブルタップすると、VoiceOverの音声がミュートされます。
この状態で操作すると、VoiceOverの効果音だけが再生され、読み上げはされません。

再度3本指でダブルタップすると、ミュートは解除されます。

スクリーン・カーテン
====================

3本指でトリプルタップ（素早く3回タップ）すると、画面表示が停止されます。
画面表示がされなくなるだけで、VoiceOverも含めて他の機能はすべて正常に動作している状態になります。

再度3本指でトリプルタップすることで、画面表示を再開できます。

なお、この機能を用いることで、画面表示が見えない状態での操作が可能かどうかを確認するといったことも可能です。

音楽の再生
==========

2本指でダブルタップすると、音楽が再生されることがあります。

再度2本指でダブルタップすることで、再生を停止することができます。

**********************************************************
一般的に用いられるコンポーネントの操作方法と期待される挙動
**********************************************************

ここでは、用いられることが多い標準のUIコンポーネントについて、VoiceOver使用時の挙動と操作方法を記します。
UIコンポーネントを独自に実装する場合は、これらを参考にしてVoiceOver使用時の挙動を定めると良いでしょう。

ボタン
======

UIコンポーネント
   ボタン
参考
   `ボタン | Apple Developer Documentation <https://developer.apple.com/jp/design/human-interface-guidelines/buttons>`_

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   *  そのボタンの役割が分かるテキストが読み上げられる
   *  ボタンであることが分かる読み上げがされる
1本指によるダブルタップ
   *  ボタンがアクティベートされる

実装のポイント
--------------

*  ``trait`` に ``button`` を指定する
*  ``label`` にボタンの役割を示すテキストを指定する

ラベル
======

UIコンポーネント
   ラベル
参考
   `ラベル | Apple Developer Documentation <https://developer.apple.com/jp/design/human-interface-guidelines/labels>`_

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   ラベルの内容が読み上げられる

ページコントロール
==================

UIコンポーネント
   ページコントロール
参考
   `ページコントロール | Apple Developer Documentation <https://developer.apple.com/jp/design/human-interface-guidelines/page-controls>`_

使用されている箇所の例
----------------------

「天気」アプリの画面下部、天気を表示する地点を切り替えるコントロール

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   *  なにを変更するためのコントロールかが分かる読み上げがされる
   *  現在選択されている項目が読み上げられる
   *  現在選択されている項目が、全部でいくつある項目のうちのいくつ目かが分かる読み上げがされる
   *  選択を変更できることが分かる読み上げがされる（例：「調整可能」などと発声する）
1本指による上または下方向へのフリック
   *  選択項目が変更され※、変更後の状態を読み上げる

※このとき、ローターで「値を調整」が選択されている必要があります。通常は、フォーカスされた時に自動的にこの設定になります。

ピッカー
========

UIコンポーネント
   ピッカー
参考
   `ピッカー | Apple Developer Documentation <https://developer.apple.com/jp/design/human-interface-guidelines/pickers/>`_

使用されている箇所の例
----------------------

「ヘルスケア」アプリの「概要」タブ内、 :menuselection:`プロフィール --> ヘルスケアの詳細 --> 編集 --> 生年月日`

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   *  現在選択されている項目が読み上げられる
   *  現在選択されている項目が、全部でいくつある項目のうちのいくつ目かが分かる読み上げがされる
   *  選択を変更できることが分かる読み上げがされる（例：「調整可能」や「ピッカー項目」などと発声する）
1本指による上または下方向へのフリック
   *  選択状態が変更され※、変更後の状態を読み上げる

※このとき、ローターで「値を調整」が選択されている必要があります。通常は、フォーカスされた時に自動的にこの設定になります。

セグメントコントロール
======================

UIコンポーネント
   セグメントコントロール
参考
   `セグメントコントロール | Apple Developer Documentation <https://developer.apple.com/jp/design/human-interface-guidelines/segmented-controls>`_

使用されている箇所の例
----------------------

「マップ」アプリの「地図モード」をタップすると表示される、地図の表示モードを切り替える画面

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   *  そのセグメントの内容が分かるテキストが読み上げられる
   *  そのセグメントの選択状態が分かる読み上げがされる（選択状態の場合は「選択中」といった発声があり、選択されていない場合には選択状態に関する発声がない）
1本指によるダブルタップ
   *  そのセグメントが選択状態になり、選択状態が変わったことが分かる読み上げがされる

スライダ
========

UIコンポーネント
   スライダ
参考
   `スライダ | Apple Developer Documentationr <https://developer.apple.com/jp/design/human-interface-guidelines/sliders>`_

使用されている箇所の例
----------------------

「設定」アプリの「画面表示と明るさ」内、「画面の明るさ」のコントロール

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   *  なにを変更するためのコントロールかが分かる読み上げがされる
   *  現在の設定値が読み上げられる
   *  値を変更できることが分かる読み上げがされる（例：「調整可能」などと発声する）
1本指による上または下方向へのフリック
   *  値が変更され※、変更後の値を読み上げる

※このとき、ローターで「値を調整」が選択されている必要があります。通常は、フォーカスされた時に自動的にこの設定になります。

実装のポイント
--------------

*  ``trait`` に ``slider`` を指定する
*  ``label`` に変更対象が分かるテキストを指定する
*  ``value`` に現在の値を指定する

トグル
======

UIコンポーネント
   トグル
参考
   `トグル | Apple Developer Documentation <https://developer.apple.com/jp/design/human-interface-guidelines/toggles>`_

使用されている箇所の例
----------------------

「設定」アプリの「サウンドと触覚」内、「画面の明るさ」のコントロール

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   *  なにを変更するためのコントロールかが分かる読み上げがされる
   *  現在の選択状態（オン/オフ）が読み上げられる
1本指によるダブルタップ
   選択状態が切り替わり、変更後の状態が読み上げられる

テキストフィールド
==================

UIコンポーネント
   テキストフィールド
参考
   `テキストフィールド | Apple Developer <https://developer.apple.com/jp/design/human-interface-guidelines/text-fields>`_

使用されている箇所の例
----------------------

「設定」アプリ、 :menuselection:`メール --> アカウント --> アカウント追加 --> iCloudアカウント` の、Apple IDを入力するフィールド

VoiceOver利用時の挙動
---------------------

1本指で触れる、または1本指による右/左方向へのフリックでフォーカス
   *  なにを変更するためのコントロールかが分かる読み上げがされる
   *  text fieldであることが分かる読み上げがされる
   *  現在入力されている値、またはプレイスホルダーとして表示されている値が読み上げられる
1本指によるダブルタップ
   *  編集可能な状態に切り替わる
   *  画面上に表示されたキーボードから入力ができる
   *  外付けのキーボードが接続されている場合は、そのキーボードからも入力ができる
編集可能な状態での1本指による上または下方向へのフリック
   *  ローターの設定※に応じてカーソルが移動し、移動した範囲の入力内容が読み上げられる

※ローターの設定が、「文字」の場合は1文字ずつ、「単語」の場合は1単語ずつ、「行」の場合は1行ずつ移動します。

