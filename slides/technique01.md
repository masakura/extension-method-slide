### 名前空間を揃える

* Customer 型と CustomerExtension 型の名前空間を揃える
  - IntelliSense が効きます!
* アセンブリが別でも名前空間を揃える

```csharp
using Hoge.Entities
// 名前空間を揃えていないと、別途 using で取り込まないといけない
// using Hoge.Extensions;

public class Foo {
    public void Bar(IEnumerable<Customer> customers) {
        // ここで IntelliSense の候補に拡張メソッドが出ない
        customers.
    }
}
```

IntelliSense が効かないメソッドは誰も使いません! <!-- .element: class="fragment" data-fragment-index="1" -->
