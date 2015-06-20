# Yeoman Presentation memo
HTML5 Conference 2015 in 鹿児島で行うセッションの一つ Yeoman に関するスライドを作る


## 構成


### HTML5アプリではたくさんのツールを使う
この部分ではHTML5アプリでたくさんのツールを使うことをアピールする。とにかく大変そう!

* 全体的
  - minifiy
  - concat
* JavaScript
  - TypeScript or CoffeeScript
  - JSHint/JSCS
  - Backbone.js/AngularJS
  - Bootstrap/jQuery UI/jQuery Mobile
  - Moment.js/Underscore.js
* CSS
  - Sass/Compass
* Images
  - imagemin


### Yeoman の簡単な紹介
そんな時に現れた強い味方が Yeoman!

* Scaffolding の Yo
* Buildtool の Grunt
* Package Manager の Bower


### 実際に使ってみる
Yeomanのツール群はNode.js/npが必要。

一般的にはYoから紹介されることが多いけど、時間次第ではBowerからやる。

`bower init`でプロジェクトを作成し、`bower install --save`でライブラリを持ってこれることをアピール。依存関係を解決してくれるので素敵!

Bowerが標準的になると、JavaScriptライブラリは細分化され、依存関係を主導で解消することはできなくなるので、必須のツールに為る。

そして、Grunt! これは Ant とか MSBuild とか Make に近い。gulp もあるけど、今日は Grunt だけ紹介。

試しに、JSHint を行うタスクを作ってみる。

んで、必要なライブラリや Gruntfile.js を書くのって大変でしょ? そんなあなたのために Yo があります! とやる。


### タスクがどうなっているかの解説
* LiveReload 超便利!
* 全部圧縮と結合がかかる


### いくつか Yeoman Generator を紹介
* generator-backbone
* generator-angular
* generator-angular-fullstack
* generator-angular-eggs


### できれば...
実はこのスライドも Yeoman Generator で書きました!


### ついでに!
generator-graybullet-corodvaというのがあって、これを使うと Apache Cordova アプリが簡単に作れます!

実用性は generator-ionic の方が上だけど、ね...


### 他にも
* デバッグはブラウザーのDevTools使う
  - Google Chrome 使うと、Android 4.4 以降のリモートデバッグも簡単!
  - Safari 使うと iOS のリモートデバッグも簡単!
* エディターは割と何でもいい
  - Emmet!
  - JSHint/JSCS Linter とか
  - EditorConfig


### 最後に
Visual Studio から Bower や Grunt がサポートされるようですので、これからは Yeoman で開発をするのが当たり前になるんじゃないかなと思います!
