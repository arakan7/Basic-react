# 学習メモ

- Reactのお作法

  - ```javascript
    import React from "react";
    import ReactDom from "react-dom";
    import App from "./App";

    ReactDom.render(<App />, document.getElementById("root"));
    ```

- JSX記法について
  - JSの中でreturnして、その中でhtmlタグを書くやり方
  - 複数行書くときはreturn()
  - returnしていくhtmlタグは一つのタグで囲わないといけない
    - &lt;div&gt;&lt;/div&gt;
    - &lt;React.Fragment&gt;&lt;/React.Fragment&gt;
    - &lt;&gt;&lt;&gt;（← れが一番）
- コンポーネントについて
  - コンポーネント名は必ず先頭が大文字
  - コンポーネント名はパスカルケース（例：SomeComponent）
  - コンポーネント名とその中に使用する関数名は同じにするべき？
  - import React from "react" は必須（JSX記法を書くのみ場合は不要）
  - export default 関数名
  - import 関数名 from 対象コンポーネント
  - .jsxはreactのコンポーネント拡張子
- Reactでのイベントやstyleの扱い方について
  - イベント名やスタイルはキャメルケース（例：someEvent）
  - JSX記法の中に{}書くとjsが使用できる
  - {{}}だと、内側の{}はオブジェクトのことを表す
- Propsについて
  - コンポーネントに渡す引数
  - propsの名前は何でも大丈夫ですが、わかりやすい名前で、もらう側はpropsで
  - 分割代入しようすると、props.〇〇と書かないで、○○で済むので便利
  - オブジェクトでキーとバリューが同じ場合一つにかけて省略できる

## 環境構築

```bash
npx create-react-app Basic-react
```

### 参考記事

- [2022年12月になってもcreate-react-appでReact 17を新規作成したい](https://moritalous.pages.dev/81ca7bc518e4c3becdd6)
- [Windows 環境から Node.js を完全に削除する方法をやってみた](https://dev.classmethod.jp/articles/completely-uninstall-nodejs-from-windows/)
- [[React] npxエラー](https://zenn.dev/huraipan/articles/180999f3ad3742)
- [Gitの設定をgit configで確認・変更](https://note.nkmk.me/git-config-setting/)
