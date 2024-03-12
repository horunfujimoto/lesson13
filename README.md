## SQLの実行
### 1. ファイルをワークスペース直下に移動
### 2. MySQLサーバの起動
```
$ sudo systemctl start mysqld
もしくは
$ sudo service mysql start
```
### 3. データベースサーバへ接続
```
$ mysql -u root
```

### 4. 使用するデータベースを選択
```
mysql> USE booklist
```

### 5. 実行したいSQLをたたく（これは実行しなくてもよい）
```
INSERT INTO books (book_title) VALUES("非エンジニアのためのプログラミング講座");
```

## webで表示する方法
### 1. 上記1～4の実行
### 2. Webサーバの起動
```
$ php -S $IP:$PORT -c php.ini
```
### 3. Previewを立ち上げ（vscode上部ボタン選択）
Preview > Preview Running Applicationを選択

### 4. URLにパス名を付け足す
/booklist.php
