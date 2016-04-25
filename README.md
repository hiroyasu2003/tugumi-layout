# 基本コンセプト

基本的に仮名を同時打鍵、もしくは交互打鍵で打て、仮名に必要なキーを2段に収め、またストレスのない入力を実現するために、ある程度、漢字直接入力をすることもできる配列。  
Dvorak配列のみ対応。  

# 配列定義実装方法

ローマ字テーブルカスタマイズ機能で実装できる同時打鍵配列を目指して、2つのキーを同時打鍵すると2パターンの出力ができることを利用し、1つの仮名に2パターンの入力を定義することで、同時打鍵をローマ字テーブルでの実装を可能にしている｡  
使用キーの範囲は4×10で､基本的には左手に子音、右手に母音を配置している。また右手上段で小文字、濁音を入力することができる。カタカナはCapslookキーを入力することで仮名と同じストローク、組み合わせで入力できる。仮名入力に使われないキーは、漢字直接入力（通称　漢直）の1ストローク目（トリガーキー）に使われる。  

# 配列図

## 仮名

基本的にはローマ字入力などと同じような、子音と母音を指定し､2打で1文字を入力する「行段系」のシステムをとっており､かつ1動作で入力できるように、母音、子音どちらから打っても同じ文字が出力されるようにされている｡  

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">ま</td>
<td class="org-left">た</td>
<td class="org-left">な</td>
<td class="org-left">は</td>
<td class="org-left">わ</td>
<td class="org-left">ぇ”</td>
<td class="org-left">ぁ”</td>
<td class="org-left">ぃ”</td>
<td class="org-left">ぉ”</td>
<td class="org-left">ぅ”</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">ら</td>
<td class="org-left">さ</td>
<td class="org-left">あ</td>
<td class="org-left">か</td>
<td class="org-left">や</td>
<td class="org-left">え</td>
<td class="org-left">あ</td>
<td class="org-left">い</td>
<td class="org-left">お</td>
<td class="org-left">う</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>
</tbody>
</table>

例：ま=　ま+あ　　こ=　か+お  
ぱ行はま行の濁音に当てられている｡  

また､以下の文字は頻度などの理由で､上記の表とは別のところに置かれている｡  

ん=　や+い　　っ=　や+ぃ　　ょ=　や+お　　ゅ=　や+う　　よ=　や+ぉ　　ゆ　=や+ぅ  

記号はそれぞれ、な行とら行の濁音にある｡  

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">な</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">！</td>
<td class="org-left">「</td>
<td class="org-left">」</td>
<td class="org-left">？</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">え</td>
<td class="org-left">あ</td>
<td class="org-left">い</td>
<td class="org-left">お</td>
<td class="org-left">う</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>
</tbody>
</table>

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">&#xa0;</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">（</td>
<td class="org-left">）</td>
<td class="org-left">［</td>
<td class="org-left">］</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">ら</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">え</td>
<td class="org-left">あ</td>
<td class="org-left">い</td>
<td class="org-left">お</td>
<td class="org-left">う</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>
</tbody>
</table>

## 漢字直接入力

漢直部分は、かな入力で使わない下段のキーを1ストローク目として､小学校で学習する漢字をすべて打つこそができる｡3ストローク以内で、4段に五十音順に並べている｡そのため､学習コストが低く、連想式のシステムではあるが、音以外に連想できるものが無いため､思考にそれほど負荷をかけない｡詳しい配置は定義ファイル参照。  

# ToDo

1.残りの常用漢字の実装。  
2.記号面の充実｡  
3.漢字含めたグラフィカルな配列表制作。  
4.QWERTY配列対応。  

# 参考等した配列

こまどり配列　：この配列を作るきっかけ。こまどり配列を同時打鍵で入力しようとしたのがすべての始まり｡  

Phoenix　；同じ2段配列で、漢直搭載。漢直のアイデアの参考と、仮名配列の参考｡  

G-Code　：漢直の配置等参考に｡  

# ライセンス

この配列は改造改変、紹介、この配列をベースとした配列の公開など完全に自由です｡ただし､この配列を使うときは自己責任でおねがいします。  
不具合、改善案、要望などは対応するときもありますが、絶対ではありません。  
この配列に影響を受けた配列を公開するときは、できればこのつぐみ配列に触れていただけるとありがたいです｡
