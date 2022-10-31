# 天気予報アプリの画面レイアウトを構成する

## 課題

以下の条件の画面レイアウトを作ってみましょう。

- [Placeholder] の幅は画面の幅の半分
- 青字と赤字の [Text] の幅は [Placeholder] の幅の半分
  ![horizontal-ratio](./images/layout/horizontal-ratio.png)

- [Placeholder] の高さと幅は同じ
  ![aspect-ratio](./images/layout/aspect-ratio.png)

- [Text] の上下に 16 logical pixel のパディング
- [Text] の文字は `** ℃`
- [Text] の水平位置は中央
- [Text] のスタイルは TextTheme の [`labelLarge`]
- [Text] の色は左が [`Colors.blue`]、右が [`Colors.red`]
  ![text-padding](./images/layout/text-padding.png)

- [Placeholder] の水平中央は画面の中央と同じ
- [Placeholder] と [Text] を合わせた矩形の垂直中央は画面の中央と同じ
  ![centering](./images/layout/centering.png)

- [Text] と [TextButton] の隙間は 80 logical pixel
  ![button-margin](./images/layout/button-margin.png)

- [Text] と [TextButton] の水平中央は同じ
  ![button-centering](./images/layout/button-centering.png)

## ヒント

Flutter には iOS の [NSLayoutConstraint] や Android の [ConstraintLayout] のようなものはありません。

以下の Widget を利用するとさまざまな画面に対応することができます。

- [Row]
- [Column]
- [Flexible]
- [Expanded]
- [AspectRatio]

<!-- Links -->

[Placeholder]: https://api.flutter.dev/flutter/widgets/Placeholder-class.html

[Text]: https://api.flutter.dev/flutter/widgets/Text-class.html

[`labelLarge`]: https://api.flutter.dev/flutter/material/TextTheme/labelLarge.html

[`Colors.blue`]: https://api.flutter.dev/flutter/material/Colors/blue-constant.html

[`Colors.red`]: https://api.flutter.dev/flutter/material/Colors/red-constant.html

[TextButton]: https://api.flutter.dev/flutter/material/TextButton-class.html

[NSLayoutConstraint]: https://developer.apple.com/documentation/uikit/nslayoutconstraint

[ConstraintLayout]: https://developer.android.com/develop/ui/views/layout/constraint-layout

[Row]: https://api.flutter.dev/flutter/widgets/Row-class.html

[Column]: https://api.flutter.dev/flutter/widgets/Column-class.html

[Flexible]: https://api.flutter.dev/flutter/widgets/Flexible-class.html

[Expanded]: https://api.flutter.dev/flutter/widgets/Expanded-class.html

[AspectRatio]: https://api.flutter.dev/flutter/widgets/AspectRatio-class.html