Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
**I  ported    "chipmunk"   that is one of  "cocos2dx"  of the famous game libraries to the Android Apps(applications) as  to work.**
  
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
**cocos2dx、cocos2dx-luaの２つ**には、常に、かならず  
　「**マック（xCode) と アンドロイド(Andoroid、eclipse) 両方ある**」ようなのに、  
のこり２つには、 なぜか 「 **xCode（マック）だけ** 」 しか、無いようなのです。なお  

   **Box2dも アンドロイド(Andoroid、eclipse)にすでにもう移植し動作**しておりますので、   
それも 今後ここかあるいは別な新たな所で、掲載したいと現在考えております次第です。