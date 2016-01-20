### 作り方

```csharp
// 拡張メソッドを宣言する
public static class StringExtension
{
    public static int ToInt32(this String s)
    //                        ~~~~ this とつけるだけ
    {
        return Int32.Parse(s);
    }
}
```

```csharp
// スタティックメソッドなのに、インスタンスメソッドのように呼び出せる!
int i = "123".ToInt32();
```
