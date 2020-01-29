# Appium(Ruby) サンプル

## 概要
* appium: http://appium.io/
* サンプルコードは以下を流用
  * https://github.com/appium-boneyard/sample-code/tree/master/sample-code/examples/ruby

### 導入メモ
#### node
```
$ node -v
v10.16.3
```

#### Xcodeのインストール
* App Storeから落とす(2時間程度)
* 以下を実行(パスワードを聞かれる)

```
$ sudo xcode-select --switch /Applications/Xcode.app # 利用するxcodeを指定
$ sudo xcodebuild -license # 規約に同意
```

* `Xcode.app > Preferences > Components` から "iOS 10.3.1 Simulator" をインストール(40分程度)
  * バージョンはサンプルコードで利用しているもの


#### appiumのインストール
```
$ npm install -g appium  # get appium
$ npm install wd         # get appium client
```

#### appiumの実行に必要なものをインストール

```
$ brew install carthage
```

#### 実行
* bundle install
```
$ bundle install
```

* appiumの起動

```
$ appium &
```

* 別タブでテスト実行(以下が出ればOK)
```
$ bundle exec rspec test.rb
Tests Succeeded!
No examples found.


Finished in 0.00087 seconds (files took 29.19 seconds to load)
0 examples, 0 failures
```
