選挙ポスター管理
===========


必須環境
--------

- Ruby 2.0
- bundlerをインストール済みであること

インストール方法
----------------

```
> git clone https://github.com/open-election/poster-manager.git
> cd poster-manager
> bundle install
```

動かし方
--------

- 以下のコマンドを実行

```
> SHIRASETE_PROJECT_ID=対象プロジェクトID SHIRASETE_API_KEY=取得したAPIキー bundle exec rails server
```

### heroku

```
> heroku create apps
> heroku config:add SECRET_TOKEN=`bundle exec rake secret`
> heroku config:add SHIRASETE_API_KEY="APIキー"
> heroku config:add SHIRASETE_PROJECT_ID="プロジェクトID"
> git push heroku master
```

LICENSE
-------

[MIT](http://opensource.org/licenses/MIT)
