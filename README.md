AboutStage
================================================================================

JavaFX用バージョン情報表示ウィンドウ生成ライブラリ

- 作者           : 次郎 (jiro)
- 作成日         : 2017/03/06
- 最終更新日     : 2017/03/06
- バージョン     : 1.0.0
- Javaバージョン : 1.8.0-121

## 使い方

    import jiro.javafx.stage.AboutStage;

    AboutStage aboutStage = AboutStage.Builder(title, version)
      .author("Author Name")
      .blog("Blog Name")
      .blogUrl("http://www.ownblog.com")
      .css("/package/res/css/app.css")
      .appIcon("/app/res/img/app_icon.png")
      .authorIcon("/app/res/img/author_icon.png")
      .build();

    aboutStage.showAndWait();

## 更新履歴

  Ver1.0.0 : 2017/03/06  
  - ライブラリ公開
