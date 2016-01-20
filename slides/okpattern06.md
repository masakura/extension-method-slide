### 拡張メソッド版だったら安心!

```csharp
// 配列で返ってくると...
Customer[] array = GetCustomers();
array.Males(); // <- OK!

// HashSet で返ってくると...
HashSet<Customer> hashSet = GetCustomers();
hashSet.Males(); // <- OK!

// Dictionary で返ってくると...
Dictionary<int, Customer> dictionary = GetCustomers();
dictonary.Values.Males(); // <- OK!
```
