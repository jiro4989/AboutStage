AboutStage
================================================================================

JavaFX用バージョン情報表示ウィンドウ生成ライブラリ

- Version      : 1.0.1
- Java Version : 1.8.0_121
- Author       : 次郎 (Jiro)
- Since        : Mar 06, 2017
- Last Changed : Mar 06, 2017

使い方
--------------------------------------------------------------------------------

インスタンス生成時に必須プロパティとして、アプリ名とアプリのバージョンを渡しま
す。これらのプロパティは`null`や空文字列を受け付けません。それらが渡されると例外
を返します。

Builderコンストラクタを呼び出したあと、`Builder#build()`を呼び出すことで
AboutStageのインスタンスが生成されます。

この時、`Builder#build()`する前に各種プロパティのセッターメソッドでチェーンする
ことで、各種オプションを変更できます。

```java
import jiro.javafx.stage.AboutStage;

AboutStage aboutStage = AboutStage.Builder("App Title", "App Version")
  .author("Author Name")
  .blog("Blog Name")
  .blogUrl("http://www.ownblog.com")
  .css("/package/res/css/app.css")
  .appIcon("/app/res/img/app_icon.png")
  .authorIcon("/app/res/img/author_icon.png")
  .build();

aboutStage.showAndWait();
```
