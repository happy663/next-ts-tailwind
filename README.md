# Next.js+TypeScript+TailwindCSS+Prettier+ESlint の設定をしたプロジェクト

## 導入する
yarn create next-app --example https://github.com/happy663/next-ts-tailwind

## VScode の拡張機能（推奨)

Tailwind CSS IntelliSense

https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcs


## 設定した項目の説明

### tailwind.config.js

Jit(Just-in-Time mode)を設定
実際に利用しているユーティリティのみビルドして生成するモード

ビルド高速化,バリアントを組み合わせて使用可能など様々なメリットがある

https://tailwindcss.com/blog/just-in-time-the-next-generation-of-tailwind-css

### eslintrc.json

モジュールの import 順及び tailwind CSS のクラス名のソート,子のないコンポーネントの余分な終了タグの消去,未使用モジュールの削除を設定

.vscode に source.fixAll.eslint が設定してあるのでセーブすれば自動で修正される

デフォルトがいい人は消してください

### tsconfig.json

baseUrl を追加して絶対 Path で import する


