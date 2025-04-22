# tilebuilder

`data/` に Shapeファイルを配置して以下を実行すると、`tiles/` にベクトルタイルが作成されます。

```bash
$ npm install
$ npm run build
```

### タイルのカスタマイズ

`$ npm run build` を実行すると、`tiles/kata.yml` が生成されます。任意でタイルの設定をカスタマイズしてください。

```yaml
default:
  cpg: UTF-8
  prj: EPSG:4612

airport:
  source:
    - ./airport.shp
  minzoom: 9
  maxzoom: 14

town:
  source:
    - ./city/town.shp
    - ./city/town2.shp
  minzoom: 12
  maxzoom: 14
```

## プレビュー

作成したベクトルタイルをプレビューすることができます。

```bash
$ npm start
```

## デプロイ

```bash
$ npm run deploy
```
