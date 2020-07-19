# DockerでReactの環境構築

### このリポジトリをクローンし、ディレクトリ移動
```bash
$ git clone https://github.com/2754github/React_with_Docker.git
$ cd React_with_Docker
```

### ビルド
```bash
$ docker-compose build
```
※かなり時間かかる

### Reactアプリ作成（w/TypeScript）
```bash
$ docker-compose run --rm app sh -c "npx create-react-app react-app --typescript"
```
※かなり時間かかる

### ついでにmaterial-uiも導入
```bash
$ docker-compose run --rm app sh -c "cd react-app && npm install @material-ui/core"
```
※かなり時間かかる

### コンテナ起動
```bash
$ docker-compose up
```

### 例のページが見られるか確認
http://localhost:3001/ にアクセス
