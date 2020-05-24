### Spring とは
Springについて調べたことをまとめた覚書

* 参考文献
https://www.sejuku.net/blog/10456
https://qiita.com/akane_kato/items/fff46dfa34f97f95dc88
https://qiita.com/ASHITSUBO/items/6c2aa8dd55043781c6b4
https://wa3.i-3-i.info/word12775.html
https://www.techscore.com/blog/2016/11/22/start-with-sts-and-spring-boot-1/
https://www.techscore.com/blog/2016/11/22/start-with-sts-and-spring-boot-2/
https://www.techscore.com/blog/2016/11/22/start-with-sts-and-spring-boot-3/
https://www.tuyano.com/index2?id=5729201025974272

#### フレームワークとは
フレームワークはアプリ開発をする際に、
開発の効率を上げるために便利な機能がたくさん詰まったツールです。
WEBアプリ開発に用いるフレームワークは、とくに「WEBフレームワーク」と呼ばれています。
「Spring Framework」もこのWEBフレームワークの1つです。


#### 環境構築

* 注意点！
caskでjavaインストールする際、権限エラーがでることがある
```
XXXXX % brew cask install java
Error: Can't create update lock in /usr/local/var/homebrew/locks!
Fix permissions by running:
  sudo chown -R $(whoami) /usr/local/var/homebrew
Error: Download failed on Cask 'java' with message: Permission denied @ rb_sysopen - /usr/local/var/homebrew/locks/57f2cd89482ecc0b0c6a7b3c3b0eff804f1cbd4d1e4688e86192566dfd9cfe2a--openjdk-13.0.2_osx-x64_bin.tar.gz.incomplete.lock
XXXXX % sudo chown -R $(whoami) /usr/local/var/homebrew
Password:
XXXXX % brew cask install java                         
touch: /usr/local/Homebrew/.git/FETCH_HEAD: Permission denied
touch: /usr/local/Homebrew/Library/Taps/homebrew/homebrew-cask/.git/FETCH_HEAD: Permission denied
touch: /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core/.git/FETCH_HEAD: Permission denied
fatal: Unable to create '/usr/local/Homebrew/.git/index.lock': Permission denied
・・・
```

#### pom.xmlとは