### 例

```csharp
// IEnumerable<Customer> 型用の拡張メソッド
public static class CustomerExtension
{
    // 男性だけの集合を返す
    public IEnumerable<Customer> Males(this IEnumerable<Customer> customers)
    {
        return customers.Where(c => c.Sex == Sex.Male);
    }

    // 女性だけの集合を返す
    public IEnumerable<Customer> Females(this IEnumerable<Customer> customers)
    {
        return customers.Where(c => c.Sex == Sex.Female);
    }

    // 年齢だけの集合を返す
    public IEnumerable<int> Ages(this IEnumerable<Customer> customers)
    {
        return customers.Select(c => c.Age);
    }
}
```

```csharp
// 男性の平均年齢を求める
var age = customers.Males().Ages().Average();
```
