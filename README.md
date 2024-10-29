# vite-amplify-example

## Reactプロジェクトの作成

```bash
npm create vite@latest -- --template react-ts
```

## Amplifyを追加

```bash
npm add --save-dev @aws-amplify/backend@latest @aws-amplify/backend-cli@latest
npm install @aws-sdk/client-secrets-manager @aws-amplify/ui-react
```

## GitHubリポジトリの登録

## sanbox の作成

```bash
npx ampx sandbox
```

## google credentials をsandboxに登録

Systems Manager のパラメータストアに secretstringとして登録される。
パスは、 `/amplify/~/GOOGLE_CLIENT_ID`、`/amplify/~/GOOGLE_CLIENT_SECRET` に保存される。

```bash
npx ampx sandbox secret set GOOGLE_CLIENT_ID
npx ampx sandbox secret set GOOGLE_CLIENT_SECRET
```

## google認証の作成


amplify/auth/resource.ts を作成
amplify/backend.ts にauth を追加
バックエンドを更新

```bash
npx ampx sandbox
```
