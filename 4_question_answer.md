>`質問`
>
>```
>Railsにおける、「単数」と「複数」の使い分けについての説明です。
>
>例えばコントローラー作成時は"blogs"と、モデル作成時は"blog”とそれぞれパラメーター指定させています。それに基づいて様々な変数等が自動的に作成されているようなので、"blogs"と"blog"を使い分けることに意味があるのだと思うのですが、何処にも記載が無いので未だに混乱しています。
>
>rake routes"を行ってみても、Prefixに"blog"　”new_blog"もあれば、"blogs" "confirm_blogs"もあります。何故こうなっているのか全く理解できていません。
>```

`回答`

```
Railsにおける、「単数」と「複数」の使い分けについての説明です。

Railsはいくつかの命名規則を使用して、モデルとデータベーステーブル間のマッピング関係を決めます。
Railsはモデル「単数」を複数形にして、それぞれのデータベーステーブル「複数」を見つけます。
例えば、「BookClub」というモデルが作成される場合は、「book_clubs」というデータベーステーブルにマッピングします。
```

詳細について[RAILS GUIDES](https://guides.rubyonrails.org/active_record_basics.html#naming-conventions)を参照:

>Model Class - Singular with the first letter of each word capitalized (e.g., BookClub).
>
>Database Table - Plural with underscores separating words (e.g., book_clubs).
