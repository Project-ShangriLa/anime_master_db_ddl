# Anime Master DB DDL

Anime API サーバー等で使用するMySQL DDLです

## DB作成

```
mysql> create database anime_admin_development
```

DB名は任意ですが、デフォルト名は「anime_admin_development」としています


## すべて登録

```
mysql -u root -p anime_admin_development --default-character-set=utf8 < *.sql 
```


## 1テーブル登録(basesテーブル例)

```
mysql -u root -p anime_admin_development --default-character-set=utf8 < bases.sql 
```


## DDL SQL Backup 例

```
mysqldump -default-character-set=utf8 -u root -p anime_admin_development -d bases > bases.sql
```
