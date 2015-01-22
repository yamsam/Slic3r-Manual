% 速度

<!---
Once the printer is reliably producing good quality prints it may be
desirable to increase the speed. Doing this provides several benefits,
the most obvious of which is that the results are produced quicker, but
also faster print times can be utilised in producing more layers, i.e.
lower layer height, thus improving perceived print quality. An
additional benefit is that a faster travel movement, between extrusions,
can reduce the effects of oozing.
--->

安定して高品質のプリントができるようになれば、今度はプリント速度を早くしたくなる
だろう。これには多くの利点がある。プリント速度の高速化はもちろん、プリント時間の
短縮により、より多くのレイヤーの作成が可能になる。これはつまり、より小さいレイヤー
高が可能になることであり、したがってプリント品質が改善される。さらなる利点として、
押出の合間の高速移動による漏れの減少がある。

<!---
The best approach is to increment the various speed parameters in small
steps and observe the effect each change has on print quality. Travel
speed is a safe starting point, and it is not unrealistic to attain
speeds of up to 250mm/s (if your printer can handle it). Adjusting the
speed of perimeters, infill is available in simple mode, and the general
rule is to have the perimeter go a little slower than the infill in
order to reduce possible blemishes on the surface (infill can be faster
because slight gaps will not matter as much).
--->

ベストアプローチは、速度パラメータを少しづつ増やしながら、その変化がプリント品質
に及ぼす影響を観察することである。これは送り速度から始めるのが安全だ。
プリンタ次第だが、250mm/sという速度を実現することすら不可能ではない。
perimeters や infill の速度調整は simple mode から利用することができる。perimeter 
の基本的なルールは infill より速度を少し遅くすることだ。これには表面上に起こりうる欠陥
を減らす効果がある（ infill を早くできるのは、そこにわずかなギャップがあっても
それほど問題にならないからだ）。

<!---
Expert mode offers more parameters to fine tune printer speeds.
Differentiation between external, small and other perimeters, infill
locations, and bridges and gaps are available, as well as the ability to
slow down for the first layer.
--->
Expert modeではプリント速度の微調整を行うためのパラメータが提供されている。
パラメータは external, small などの各種 perimeters からinfill、bridges, gapが利用できる。
また第一レイヤーの低速化も可能だ。

 ![Expert mode speed
options.](images/speed_advanced_settings.png "fig:")

<!---
Where indicated a value can be given in percentage. This is in relation
to the preceding value, e.g. 50% solid infill would be half of the value
defined for infill.
--->
パラメータの値はパーセンテージで指定することができる。これは先行する値からの
相対的な値になる。たとえば solid infill が50%であるとは、infill で指定した値の半分
であることを意味する。

<!---
A few general guidelines for each option:
--->
オプションの一般的なガイドライン

<!---
-   `Perimeters` - In expert mode this parameter can be increased
    slightly as the `External perimeters` option can be used to ensure
    blemish free external faces.
--->
-   `Perimeters` - expert modeではこの値を少し増やしてもよい。
    これは`External perimeters`によって、欠損の無い外部面が保持されるからである。

<!---
-   `Small perimeters` - Meant for holes, islands and fine details, a
    slower speed here is recommended.
--->
-   `Small perimeters` - 穴やアイランド、微細な形状のためのパラメータ。
　　速度は遅くすることを推奨する。

<!---
-   `External perimeters` - A slightly slower value may ensure cleaner
    surfaces.
--->
-   `External perimeters` - 値をわずかに遅くすることで、きれいな表面が
　　　保障される。

<!---
-   `Infill` - As fast as you can without compromising the integrity of
    the fill structure. Faster extrusions can break and result in weak
    spots.
--->
-   `Infill` - infill 構造の完全性を失わない範囲で早くしてもよい。ただし押出
    が早すぎると形状の破壊や脆弱な部位を生む原因となる。

<!---
-   `Solid infill` - The bottom of the model, and any additional solid
    layers is usually slightly slower than infill but faster than
    perimeters.
--->
-   `Solid infill` - モデルの底部や、追加された solid レイヤーでは通常、infill よりも
    少し遅く、かつ perimeters より早く設定する。

<!---
-   `Top solid infill` - Allow time for the extrusion to cleanly cover
    the previous top layers and result in a tidy top surface. the last
    few layers should have bridged the infill structure nicely,
    preparing the way for a neat finish.
--->
-   `Top solid infill` - きっちりとしたトップ表面を作るために、既存のトップレイヤー
　　をしっかりと覆うために吐出を行う時間を確保する。最後の数レイヤーは infill 構造上に
　　うまくブリッジを作り、美しい仕上がりを作るための下地となる。

<!---
-   `Support material` - Generally support structures are quick and
    dirty, and so long as the base is adequately supported they can be
    built as quickly as they can.
--->
-   `Support material` - サポート構造は素早く雑につくる。基礎が適切に
    支持できる範囲で早くしてよい。

<!---
-   `Bridges` - Having the extrusion span distances depends on the
    material and cooling. Going too slow will result in sagging, too
    fast will result in broken strands. Experimentation is the key here,
    but generally bridging runs slower than perimeters.
--->
-   `Bridges` - 橋を渡す押出であり、材料とクーリングに依存する。遅すぎれば
    垂みが生じ、早すぎれば切れた紐のようになる。試行錯誤が必要だが、
   一般的にはperimetersより遅くするとよい。

<!---
-   `Gap fill` - Filling in small gaps results in the extruder quickly
    oscillating and the resulting shaking and resonance could have a
    detrimental affect on the printer. A smaller value here can guard
    against this. A setting of zero disables gap filling completely.
--->
-   `Gap fill` - 小さなギャップを埋める処理。エクストルーダーの高速な周期振動により
   生じる振動や共振がプリンタに悪影響を与える恐れがある。この値を小さくする
   ことでこの現象を防ぐことができる。値を0にすると穴埋め処理を完全に無効にする。

<!---
-   `Travel` - As fast as your printer will allow in order to minimise
    ooze.
--->
-   `Travel` - 漏れを最小化するためにプリンタが可能な範囲で早くする。

<!---
-   `First layer speed` - As mentioned in section
    , the first layer is important to
    lay down correctly, and a slower pace helps enormously. Setting a
    value of 50%, or even less, can really help.
--->
-   `First layer speed` - 先のセクションで述べたように、
    第一レイヤーは正確に構築することが大変に重要であり、速度を遅く
   すればこの助けになる。50%かそれ以下が推奨である。

<!---
`Acceleration control` is an advanced setting allowing acceleration
settings for perimeters, infill, bridge, as well as a default setting,
to be made. Deciding which values to set depends on the capabilities of
the machine. Any settings within the firmware may be a good starting
point.

Take into account any restrictions enforced by the firmware as many have
settings for the maximum safe speed of each axis.
--->
`Acceleration control` では、perimeters, infill, bridgeとdefaultの加速度を設定
するこができる。どの値を設定すればよいかは、そのマシンの許容範囲に依る。ファームウェア
の設定値を参考にするとよいだろう。

それらの値はファームウェアによって、各軸における安全な最大速度として制限されていることを
考慮すること。

