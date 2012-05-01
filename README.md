Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
**I  ported    "chipmunk"   that is one of  "cocos2dx"  of the famous game libraries to the Android Apps(applications) as  to work.**
  
**( box2d, too. )**  
ゲームライブラリの**cocoss2d-xの「chipmunk」**で最初からサンプルコードとして  
ある**xCodeのアプリ(**、つまり**iPhone等マックのアプリ**が作られる**)** だけではなくて  
  
  **アンドロイドアプリ（エクリプス（jniも使用））** も 作れるように   
してみました。（「cocos2d-1.0.1-x-0.13.0-beta (Mar 29, 2012)  
　　http://www.cocos2d-x.org/projects/cocos2d-x/wiki/Download 」 を使用します。）

***  
* 繰返しになりますが 最新のcocos2d-1.0.1-x-0.13.0-beta (Mar 29, 2012)で行ないます。  
http://www.cocos2d-x.org/projects/cocos2d-x/wiki/Download このベータ版でなく その  
まえのcocos2d-1.0.1-x-0.12.0 (Mar 05, 2012)で どうした訳かうまくゆきません。ただ  
  元々、cocos2d-xは、これら13.0-betaや12もふくめて どのバージョンでも、  
　**chipmunkに「アンドロイド専用のコードはこれまで 無かった」**ようにも 思います。  
  ４つ（＝cocos2dx、cocos2dx-box2d、**cocos2dx-chipmunk**、cocos2dx-lua）のうち  
**cocos2dx、cocos2dx-luaの２つには**、常に、かならず  
　**「マック（xCode) と アンドロイド(Andoroid、eclipse) 両方ある」**ようなのに、  
**のこりの２つは なぜか 「 xCode（マック）だけ 」** しか無いようです。なお、  

   **Box2dもすでにもうアンドロイド(Andoroid、eclipse)に 移植し動作**しておりますので、   
それも 今後ここかあるいは別な新たな所で、掲載したいと現在考えております次第です。
  
* ところでこの（ベータ版の）13でアンドロイドに移植した場合に  
**（バックキー、メニューキーなどでもそうなりますが）他の画面に変え再び元の画面に  
戻った際に、「画像が表示されなくなる」不具合（？？）**が、みられませんでしょうか?  
しかもこうして今私が記載している  
「box2dやchipmunkのようにはじめからアンドロイドのソースなど無いもの」だけでなく
**アンドロイド(Andoroid、eclipse)のソースのものも（前述cocos2xやlua、それ以外も?)  
そうした〜画像が表示されなくなる〜状態が、みられる**