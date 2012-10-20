このレポジトリについて
----------------------
======================
日本語動詞の派生形をパターンごとに分類したものです。

independent.tsv と composed.tsv という二つのファイルから構成されています。

independent.tsv には他のものを含まないもの、composed.tsv には他のものを構成要素として含むものを収録しています。「言い付かる:言い付ける」のような複合語であっても、「付かる:付ける」のようなペアがないものは、independent.tsv に入れています。

independent.tsv の形式
-----------------------
    派生パターン
    元の読み<TAB>元の表記<TAB>派生後の読み<TAB>派生後の表記[<TAB>i]
    元の読み<TAB>元の表記<TAB>派生後の読み<TAB>派生後の表記[<TAB>i]
    ...

    -agu:-ugaseru
    ゆらぐ	揺らぐ	ゆるがせる	揺るがせる
    -agu:-ugasu
    ゆらぐ	揺らぐ	ゆるがす	揺るがす
    -areru:-eru
    わかれる	分かれる	わける	分ける
    -aru:-eru
    いかる	活かる	いける	活ける
    もうかる	もうかる	もうける	もうける
    もうかる	儲かる	もうける	儲ける
    ...
    -u:-eru
    ...
    あく	開く	あける	開ける
    かく	欠く	かける	欠ける	i

派生パターンは、たとえば -u:-eru であれば、あく(ak-u):あける(ak-eru)、そだつ(sodatu):そだてる(sodat-eru)のようになります。

ほとんどの場合、派生前は自動詞で派生後は他動詞（向く:向ける など）なのですが、一部に他動詞を自動詞にするもの（焼く:焼ける など）があり、その場合 "i" というフラグをつけています。

「もうかる」「儲かる」のような、同じ動詞の複数表記は重複して入っています。

composed.tsv の形式
-------------------
    派生パターン
    #構成要素の元の読み<TAB>構成要素の元の表記<TAB>構成要素の派生後の読み<TAB>構成要素の派生後の表記[<TAB>i]
    複合語の元の読み<TAB>複合語の元の表記<TAB>複合語の派生後の読み<TAB>複合語の派生後の表記[<TAB>i]
    複合語の元の読み<TAB>複合語の元の表記<TAB>複合語の派生後の読み<TAB>複合語の派生後の表記[<TAB>i]
    
    -aru:-eru
    #かかる	かかる	かける	かける
    きりかかる	切りかかる	きりかける	切りかける
    せめかかる	攻めかかる	せめかける	攻めかける
    ...
    #あがる	上がる	あげる	上げる
    あみあがる	編み上がる	あみあげる	編み上げる
    あらいあがる	洗い上がる	あらいあげる	洗い上げる
    ...
    -u:-eru
    #そろう	揃う	そろえる	揃える
    とりそろう	取り揃う	とりそろえる	取り揃える
    #つく	つく	つける	つける
    いきおいづく	勢いづく	いきおいづける	勢いづける

構成要素は、independent.tsv にある独立した派生形です。

「編み上がる」のような動詞+動詞という構成のものと、「勢いづく」のような名詞+動詞という構成のものを区別せずに入れています。