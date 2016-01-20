### インスタンスメソッド版は使い勝手が悪い

`List<Customer>` 以外のコレクションでは使えない!

```csharp
// 配列で返ってくると...
Customer[] array = GetCustomers();
// array.Males(); <- 呼び出せない

// HashSet で返ってくると...
HashSet<Customer> hashSet = GetCustomers();
// hashSet.Males(); <- 呼び出せない

// Dictionary で返ってくると...
Dictionary<int, Customer> dictionary = GetCustomers();
// dictionary.Values.Males(); <- 呼び出せない
```
