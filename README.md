[jquery.utility.js](https://github.com/Attrise/jquery.utility) - jQuery plugin 
==================================================

目次
--------------------------------------

1. 概要
2. ダウンロード
3. 機能群
  * rollOverImages
  * imgFade
  * boxSameHeight
  * anchorScroll  

概要
--------------------------------------
jquery.utility.jsはHTML、CSSコーディングを補助するjQueryのプラグインです。

ダウンロード
--------------------------------------
URL:[https://github.com/Attrise/jquery.utility](https://github.com/Attrise/jquery.utility)

概要
--------------------------------------

###rollOverImages###

任意のクラス名をimg要素に付与することでマウスオーバー時の画像を切替ます。  
デフォルトはマウスオーバー時にimgのsrc属性に指定された画像のファイル名を '_over' がついたもの切替ます。

####用例####

#####通常#####

```js
$('img.swap').rollOverImages();
```

#####オプション#####

* suffix：接尾辞(imgのファイル名語尾を_onのものと入れ替える場合)

```js
$('img.swap').rollOverImages({
    suffix : '_on'
});
```

###imgFade###

マウスオーバー時に画像を透過します。

####用例####

#####通常#####

```js
$('img.fade').imgFade();
```

#####オプション#####

* fadeSpeed：透明状態になるまでの秒数
* startAlpha：アルファ状態
* endAlpha：通常時のアルファ値

```js
$('img.fade').imgFade({
    fadeSpeed  : 500,
    startAlpha : 0.3,
    endAlpha   : 1.0
});
```

###boxSameHeight###

ボックスの高さ揃え

####用例####

#####通常#####

```js
$('.SameHeight').boxSameHeight();
```


#####オプション#####

* resize：(文字サイズ変更ナビ対応を行う場合は「true」を指定)

```js
$('.SameHeight').boxSameHeight({
    resize:true
});
```

###anchorScroll###

ページ内リンクアニメーション(※要jquery.easing.js)

####用例####

#####通常#####

```js
$('a[href^="#"]').anchorScroll();
```

#####オプション#####

* duaration：目標座標までの時間
* easing：アニメーションのイージング設定

```js
$('a[href^="#"]').anchorScroll({
     duaration : 1000,
     easing : 'easeIn'
});
```