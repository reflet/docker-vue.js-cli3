ローカル環境構築

### homeblewインストール
※ インストール済みの場合はスキップ
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew -v
Homebrew 1.8.2
```

### docker-toolbox for macOSインストール
※ インストール済みの場合はスキップ
```
$ brew update
$ brew cask install docker-toolbox
$ docker-machine create --driver "virtualbox"
$ eval $(docker-machine env default)
$ docker-machine ls

NAME    ACTIVE  DRIVER       STATE     URL
default *       virtualbox   Running   tcp://192.168.99.100:2376
```

### サーバ起動.
```
$ docker-compose build
$ docker-compose up -d
```

### 動作確認.
```
$ open http://192.168.99.100
```

