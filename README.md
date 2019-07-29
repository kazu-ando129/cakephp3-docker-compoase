# Repository name
cakephp3-docker-compoase

# Dependency
docker, docker-compose

# Setup
```
$ git clone https://github.com/kazu-ando129/cakephp3-docker-compoase.git
$ cd cakephp3-docker-compoase
$ docker-compose up -d
```

# Usage
- composerをインストールする

- composerにてCakePHP3のプロジェクトを作成する
```
$ composer create-project --prefer-dist cakephp/app my_app_name
$ cd my_app_name
```

- config/app.phpを編集する
  - Datasourcesのhostをdbにする
```
    'Datasources' => [
        'default' => [
            'className' => Connection::class,
            'driver' => Mysql::class,
            'persistent' => false,
            'host' => 'db',
```

- cakephp3-docker-compoaseをセットアップする
  - Setup参照

# Licence
This software is released under the MIT License, see LICENSE.

# Authors
kazu-ando129
