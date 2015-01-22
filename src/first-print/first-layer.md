<!---
% The Important First Layer
--->
% 第一レイヤーの重要性

<!---
 Before delving into producing the
first print it is worthwhile taking a little detour to talk about the
importance of getting the first layer right. As many have found through
trial and error, if the first layer is not the best it can be then it
can lead to complete failure, parts detaching, and warping. There are
several techniques and recommendations one can heed in order to minimise
the chance of this happening.
--->
最初のプリントの作成にのめりこむ前に、ちょっと回り道をして第一レイヤーを正しく
作成することの重要性について議論しても無駄にはならない。これまで多くの人間が
試行錯誤の中で発見してきたように、第一レイヤーがベストでない場合、部品の剥離
や歪みなどの全くの失敗につながるからだ。これを最小限に抑えるために注意すべき
テクニックやお勧めの方法を紹介する。

<!---
#### Level bed.
--->
#### ベッドは水平に

<!---
 Having a level bed is critical. If the distance between
the nozzle tip and the bed deviates by even a small amount it can result
in either the material not lying down on the bed (because the nozzle is
too close and scrapes the bed instead), or the material lying too high
from the bed and not adhering correctly.
--->
ベッドを水平にすることはとても重要だ。ノズルの先端とベッドの間の距離に、
ほんのわずかでもズレが生じると、材料がベッドに載らないか（ノズルが近すぎてベッド
をひっかいてしまうからだ）、遠すぎてベッドに正確に付着しないだろう。

<!---
#### Higher temperature.
--->
#### 温度は高めに

<!---
 The extruder hot-end and bed, if it is heated,
can be made hotter for the first layer, thus decreasing the viscosity of
the material being printed. As a rule of thumb, an additonal 5° is
recommended.
--->
エクストルーダーのホットエンドとベッドを温める際、第一レイヤーの温度を高く
すれば、プリント時の材料の粘性が少なくなる。だいたい５°程度高くすることを勧める。

<!---
#### Lower speeds.
--->
#### ゆっくりと

<!---
 Slowing down the extruder for the first layer
reduces the forces applied to the molten material as it emerges,
reducing the chances of it being stretched too much and not adhering
correctly. 30% or 50% of the normal speed is recommended.
--->

第一レイヤーの押出速度を遅くすれば、融解した材料が押し出される際に加えられる外力
が減り、のばされすぎたり、正しく付着しない確率が減ることになる。通常の速度の
３０％から５０％が推奨だ。
<!---
#### Correctly calibrated extrusion rates.
--->
#### 押出量は正確に

<!---
 If too much material is laid down
then the nozzle may drag through it on the second pass, causing it to
lift off the bed (particularly if the material has cooled). Too little
material may result in the first layer coming loose later in the print,
leading either to detached objects or warping. For these reasons it is
important to have a well-calibrated extrusion rate as recommended in
§[calibration]).
-->
押し出された材料の量が多いと、ノズルはそれを次のパスまで引っ張ってしまうことが
あり、第一レイヤーが引きはがされる原因となる（特に材料が固まっている時）。
一方で量が少ないと、第一レイヤーが後から緩くなってしまい造形物の剥離や歪み
を引き起こすことになる。これらの理由により、§[calibration]で推奨しているように、
押出量を正しく調節することが重要である。

<!---
#### First layer height.
--->
#### 第一レイヤーは厚く

<!---
 A thicker layer height will provide more
flow, and consequently more heat, making the extrusion adhere to the bed
more. It also gives the benefit of giving more tolerance for the
levelness of the bed. It is recommended to raise the first layer height
to match the diameter of the nozzle, e.g. a first layer height of 0.35mm
for a 0.35mm nozzle. Note: The first layer height is set this way
automatically in simple mode.
--->
厚いレイヤーはより流出量が増えることになり、その結果より多くの熱が加えられ、
材料がベッドによりしっかりと付着するようになる。これにはさらにベッドの水平度に対する
トレランスを増加させる効果もある。第一レイヤーの高さをノズルの直径と合わせることをお勧
めする。たとえば0.35mmのノズルには第一レイヤー高を0.35mmに設定する。
（注）simple mode では第一レイヤーの高さはこの方法で設定される。

<!---
#### Fatter extrusion width.
--->
#### 押出幅を太く

<!---
 The more material touching the bed, the
better the object will adhere to it, and this can be achieved by
increasing the extrusion width of the first layer, either by a
percentage or a fixed amount. Any spaces between the extrusions are
adjusted accordingly.
--->
ベッドに接触する材料が増えれば増えるほど、造形物がベッドによりしっかりと
付着することになる。これは第一レイヤーの押出幅を増やすことで実現可能だ。値はパーセント
か固定値で指定する。押出間の間隔は自動的に調整される。

<!---
A value of approximately 200% is usually recommended, but note that the
value is calculated from the layer height and so the value should only
be set if the layer height is the highest possible. For example, if the
layer height is 0.1mm, and the extrusion width is set to 200%, then the
actual extruded width will only be 0.2mm, which is smaller than the
nozzle. This would cause poor flow and lead to a failed print. It is
therefore highly recommended to combine the high first layer height
technique recommended above with this one. Setting the first layer
height to 0.35mm and the first extrusion width to 200% would result in a
nice fat extrusion 0.65mm wide.
--->
値はだいたい200%が推奨である。ただし、この値はレイヤー高から算出されるため、レイヤー高
が最大値であるときにのみ設定すべきである。たとえばレイヤー高が0.1mmで押出幅が200％
だとすると、実際の押し出された材料の幅は0.2mmにしかならず、これではノズル幅よりも小さくなってしまう。
この結果、流出量が足りず、プリントは失敗するだろう。したがって、前述の第一レイヤーの設定
テクニックと併用することを強く推奨する。第一レイヤー高をノズル幅と合わせて0.35mmとし、
初期押出幅を200%にすれば、実際の押出幅は0.65mmと良好な太さになる。

<!---
#### Bed material.
--->
#### ベッドの素材

<!---
 Many options exist for the material to use for the
bed, and preparing the right surface can vastly improve first layer
adhesion.
--->
ベッド素材の選択やベッド表面を整備することによって、第一レイヤーの
付着性を劇的に改善することができる。

<!---
PLA is more forgiving and works well on PET, Kapton, or blue painters
tape.
--->
PLAは扱いやすく、PET、Kapton、そしてblue painters tape（訳注：3Mのマスキング
テープ）と相性がいい。

<!---
ABS usually needs more cajoling and, whilst it can print well on PET and
Kapton, there are reports that people have success by applying hairspray
to the bed before printing. Others have reported that an ABS slurry
(made from dissolving some ABS in Acetone) thinly applied can also help
keep the print attached.
--->
ABSは気難しくなだめすかしてやる必要がある。PET、Kaptonと相性がよいが、プリント
前にベッドにヘアースプレーをかけて成功したという報告がある。ほかにもABSのスリラー
（ABSをアセトンなどで溶かしてつくる）を薄く塗布することでプリントの接着性が
改善したという報告もある。クーリングはいらない。

<!---
#### No cooling.
--->
#### 冷やすな

<!---
 Directly related with the above, it makes no sense to
increase the temperature of the first layer and still have a fan or
other cooling mechanism at work. Keeping the fan turned off for the
first few layers is generally recommended.
--->
上記に関連して、ファンなどの冷却機構が機能しているのに第一レイヤーの温度
を上げても全く意味がない。最初の数レイヤーをプリントする間はファンを切る
ことを推奨する。

