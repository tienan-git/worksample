【担当するIssue】  
「selfについて」説明文が難しかったです。  

`該当文`

```
selfはインスタンスオブジェクト自身を指しています。クラスの中でインスタンスオブジェクトを呼び出す際やそのインスタンスオブジェクトを呼び出す際は、selfを使用します。
```

`修正後`

```
selfはインスタンスオブジェクト自身を指しています。
クラスの中でインスタンスオブジェクトのpropertyやmethodを参照する際に、下記のように指定します。
self.<property name>
self.<method name(parameter1, parameter2...)>
```

詳細について[Official Ruby FAQ](https://www.ruby-lang.org/en/documentation/faq/8/) を参照：


> What does self mean?

> self is the currently executing receiver, the object to which a method is applied. A function-style method call implies self as the receiver.

