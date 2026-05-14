# fukucha

Unityで開発し、WebGL向けにビルドされた2Dガチャゲームです。福井県の観光地をモチーフにしたキャラクターを集めましょう。

## デモ

ライブバージョンは **[https://fukucha.github.io](https://fukucha.github.io)** でプレイできます。


![fukucha ゲームインターフェース](https://github.com/fukucha/fukucha/assets/1/2a3b4c5d-6e7f-8g9h-0i1j-2k3l4m5n6o7p)


## 特徴

-   **ガチャシステム:** ランダムなガチャを回して新しいキャラクターを獲得します。
-   **キャラクター収集:** 実在の観光地をモチーフにしたキャラクターを集めることができます。
-   **シンプルなゲームプレイ:** タップ操作のみの直感的なインターフェースです。

## 遊び方

1.  PCのウェブブラウザから [https://fukucha.github.io](https://fukucha.github.io) にアクセスします。
2.  ゲームが自動的に読み込まれ、開始されます。

**動作環境:**
-   WebGLをサポートする最新のウェブブラウザ。
-   本ゲームはPC（デスクトップ）向けに設計されています。モバイル端末ではWebGLの動作が保証されていないため、互換性に関する警告が表示されます。

## 技術的な概要

本プロジェクトは、標準的なUnity WebGLビルドで構成されています。

-   **ゲームデータ:** キャラクターおよび観光地のデータは `tem.csv` から読み込んでいます。
-   **エントリポイント:** `index.html` にUnityプレイヤーの設定が含まれており、ここからゲームを起動します。
-   **ビルド成果物:** `Build/` ディレクトリには、コンパイル済みのゲームアセットが含まれています。
    -   `hukucha.data.unityweb`: 圧縮されたゲームデータ。
    -   `hukucha.wasm.unityweb`: WebAssemblyバイナリ。
    -   `hukucha.framework.js.unityweb`: JavaScriptランタイムフレームワーク。
-   **ウェブテンプレート:** `TemplateData/` ディレクトリには、ロード画面やウェブページ用のCSS、画像、ファビコンが含まれています。

## ライセンス

MIT License - 詳細は [LICENSE](LICENSE) を参照してください。
