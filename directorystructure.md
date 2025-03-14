# ディレクトリ構成

以下のディレクトリ構造に従って実装を行ってください：

```
/
├── src/                          # ソースコードのルートディレクトリ
│   ├── components/               # コンポーネント
│   │   ├── common/                  # shadcn/uiの基本UI（shadcn/uiのbutton, card等）
│   │   └── atoms/                   # 最小単位のコンポーネント
│   │   └── molecules/               # atomsを組み合わせた小さな機能単位のコンポーネント
|   |   └── organisms/               # 複数のmoleculesを組み合わせた機能ブロック
│   ├── hooks/                    # カスタムフック
│   ├── lib/                      # ユーティリティ
│   │   ├── api/                  # API関連処理
│   │   └── utils/                # 共通関数
│   ├── styles/                   # スタイル定義
│   ├── assets/                   # 静的アセット（画像、フォント等）
│   ├── pages/                    # ページコンポーネント
│   ├── App.tsx                   # アプリケーションのルートコンポーネント
│   ├── main.tsx                  # エントリーポイント
├── public/                       # 公開ファイル
│   └── favicon.ico               # ファビコン
├── node_modules/                 # 依存パッケージ
├── .git/                         # Gitリポジトリ
├── index.html                    # エントリーポイントHTML
├── package.json                  # プロジェクト設定
├── pnpm-lock.yaml                 # 依存関係ロックファイル
├── tsconfig.json                 # TypeScript設定
├── vite.config.ts               # Vite設定
├── .eslintrc.json              # ESLint設定
├── .vite.config.ts              # Vite設定
└── .gitignore                   # Git除外設定
```

### 配置ルール

- UI コンポーネント → `src/components/**/*`
- 共通処理 → `src/lib/utils/`
- API 関連処理 → `src/lib/api/`
- フック → `src/hooks/**/*`
- ページ → `src/pages   /**/*`
- ファビコン → `src/public/favicon.ico`
- グローバルスタイル → `src/styles/globals.css`
- レイアウト → `src/components/layout/layout.tsx`
- ホームページ → `src/pages/index.tsx`
