# tilebuilder

`data/` に Shapeファイルを配置して以下を実行すると、`tiles/` にベクトルタイルが作成されます。

```bash
$ npm install
$ npm run build
```

### タイルのカスタマイズ

`data/kata.yml` にタイルの設定を書いてください。

```yaml
# プロジェクト全体の設定
default:
  cpg: UTF-8
  prj: EPSG:4612

airport: # source-layer名
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
