# 用語
ElasticSearch|RDB
---|---
Index|データベース
Type|テーブル
Document|レコード

# クエリ
* インデックス作成
```
PUT /index_name
```
* クエリ情報がまとまったページ
[はじめての Elasticsearch - Qiita](https://qiita.com/nskydiving/items/1c2dc4e0b9c98d164329)

# 日本語対応
プラグインが必要。デフォルトではインストールされていないため、以下をインストールする。

[Japanese (kuromoji) Analysis Plugin | Elasticsearch Plugins and Integrations \[8.3\] | Elastic](https://www.elastic.co/guide/en/elasticsearch/plugins/current/analysis-kuromoji.html)