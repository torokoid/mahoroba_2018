# mahoroba_2018
 <html lang="ja">
 <head>
 <meta charset="UTF-8">
 <title>まほろば_2018</title>

<style type="text/css">
 
  p {
color: #0000ff;
font-size: 1.5em;
 }

 .red {color:#ff0000;}
 .grey {color:#ffffff; background:#999999;}
 .yellow {color:#ff0000; background:#ffff00;}
 .blue {color:#0000ff;}
 .waku {border:2px dotted #99cc66;
　　　　　　line-height: 200%;
　　　　　　padding: 10px;}


.slider .nav li{
    transition: background 400ms
}

.slider .slider-inner li.show{
    opacity: l;
}
.slider .nav li.current{
    background: #aaa
}

#wrap {background:none} /*PC用の背景はオフ*/
body::before {
  content:"";
  display:block;
  position:fixed;
  top:0;
  left:0;
  z-index:-1;
  width:100%;
  height:100vh;
  background:url(https://torokoid.github.io/mahoroba_2018/IMG_1974.JPG) center/cover no-repeat; /*fixedをトル！*/
  -webkit-background-size:cover;/*Android4*/
  }

</style>
<!--
<link rel="stylesheet" href="../style.css/" type="text/css">
-->
</head>

<body>

<h1><span class="red"><marquee behavior="alternate">!!! まほろばの湯、2018年8月10~11日 !!!</marquee></span></h1>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

<p align="right"><marquee direction="left" scrollamount="15" width="100%">台風13号が通過した翌日の暑さの中、す～さんには極度の体調不良を押してご参加いただきました！</marquee></p>
<p align="right"><marquee direction="right" scrollamount="20" width="30%">(^_^)/~hada</marquee></p>
<h3>2018年の記録</h3> 

<div class="slider">
    <ul class="slider-inner">
    </ul>
    <ul class="nav">
    </ul>
    <p id="arrow-prev" class="arrow">←</p>
    <p id="arrow-next" class="arrow">→</p>
    </div>
    
 <script>
 var imgList = [
 "https://torokoid.github.io/mahoroba_2018/20180810_001.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_002.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_003.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_004.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_005.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_006.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_007.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_008.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_009.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_010.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_011.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_012.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_013.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_014.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_015.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_016.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_017.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_018.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_019.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_020.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_021.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_022.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_023.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_024.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_025.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_026.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_027.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_028.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_029.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_030.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_031.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_032.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_033.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_034.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_035.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_036.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_037.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_038.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_039.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_040.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_041.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_042.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_043.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_044.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_045.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_046.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_047.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_048.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_049.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_050.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_051.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_052.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_053.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_054.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_055.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_056.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_057.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_058.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_059.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_060.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_061.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_062.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_063.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_064.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_065.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_066.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_067.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_068.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_069.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_070.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_071.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_072.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_074.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_075.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_076.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_077.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_078.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_079.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_080.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_081.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_082.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_083.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_084.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_085.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_086.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_087.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_088.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_089.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_090.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_091.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_092.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_093.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_094.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_095.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_096.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_097.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_098.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_099.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_100.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_101.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_102.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_103.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_104.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_105.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_106.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_107.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_108.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_109.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_110.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_111.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_112.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_113.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_114.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_115.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_116.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_117.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_118.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_119.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_120.JPG",
 "https://torokoid.github.io/mahoroba_2018/20180810_121.PNG"
 ];
 

 // 画像とナビの要素を自動で追加
 for(var i = 0; i < imgList.length; i++){
    // li要素を取得
    var slide = document.createElement("li");
    // li要素の中に画像タグを埋め込む
    slide.innerHTML = "<img src='" + imgList[i] + "'>";
    // li要素をクラス名「slider-inner」の子要素として追加
    document.getElementsByClassName("slider-inner")[0].appendChild(slide);
    // li要素を取得
    var nav = document.createElement("li");
    // nav.style.backgroundImage = "url(" + imgList[i] + ")";
    // nav.style.width = 100 / imgList.length + "%";    
    // プロパティ「data-nav-index」に数値を割り振る
    nav.setAttribute("data-nav-index", i);
    // li要素をクラス名「nav」の子要素として追加
    document.getElementsByClassName("nav")[0].appendChild(nav);
 }

 
 // スライドの数を取得（処理のために-1する）
 var length = imgList.length -1;
 
 // クラス名「imageSlide」に画像の1枚の要素を格納
 var imageSlide = document.getElementsByClassName("slider-inner")[0].getElementsByTagName("li");
 // クラス名「dotNavigation」にドットナビの1つの要素を格納
  var dotNavigation = document.getElementsByClassName("nav")[0].getElementsByTagName("li");
 // 「現在〇〇枚目の画像を表示している」というインデックス番号を格納する変数
 var nowIndex = 0;
 // 「現在表示されている画像とドットナビにクラス名を付ける
 imageSlide[nowIndex].classList.add("show");
 dotNavigation[nowIndex].classList.add("current");
 
 // スライドがアニメーション中か判断するフラグ
 var isChanging = false;
 // スライドのsetTimeoutを管理するタイマー
 var slideTimer;
 // スライドの切り替え時に呼び出す関数
 function sliderSlide(val){
    if (isChanging === true){
        return false;
    }
    isChanging = true;
    // 現在表示している画像とナビからクラス名を削除
    imageSlide[nowIndex].classList.remove("show");
    dotNavigation[nowIndex].classList.remove("current");
    nowIndex= val;
    // 次に表示する画像とナビにクラス名を付与
    imageSlide[nowIndex].classList.add("show");
    dotNavigation[nowIndex].classList.add("current");
    // アニメーションが終わるタイミングでisChangingのステータスをfalseに
    slideTimer = setTimeout(function(){
        isChanging = false;
    }, 600);
}

// 左矢印のナビをクリックした時のイベント
document.getElementById("arrow-prev").addEventListener("click", function(){
    var index = nowIndex - 1;
    if(index < 0){
    index = length;
    }
    sliderSlide(index);
    }, false);
// 右矢印のナビをクリックした時のイベント
document.getElementById("arrow-next").addEventListener("click", function(){
    var index = nowIndex + 1;
    if(index > length){
    index = 0;
    }
    sliderSlide(index);
    }, false);
// ドットナビをクリックした時のイベントを作成
for(var i = 0; i < dotNavigation.length; i++){
    // データ属性のインデックス番号を元にスライドを行う
    dotNavigation[i].addEventListener("click", function(){
    var index = Number(this.getAttribute("data-nav-index"));
    sliderSlide(index);
    }, false);
}

    </script>
 

<p align="right"><marquee direction="left" scrollamount="15" width="100%">8月10日,11:49、バーベキューセット搬入中の図</marquee></p>
     </body>
</html>
<!-- フッタ -->
 <footer>
 Copyright 2018/08/11 S.Hada
 </footer>
