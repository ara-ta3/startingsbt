
## .sbt ビルド定義


```
name キーの := メソッドは Setting を返すが、特に Setting[String] を返す。 
```

したがって

```
:= 13 //int
```

はerror(Stringじゃないから)

```
キーは Keys オブジェクトで定義される

組み込みのキーは Keys と呼ばれるオブジェクトのフィールドにすぎない。 build.sbt は、自動的に import sbt.Keys._ するため、 sbt.Keys.name は name として呼ぶことができる。
```
