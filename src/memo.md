# STAThreadの意味
Windowsフォームアプリケーションのエントリポイントには、STAThread属性が適用されているのが普通です。

```C#
/// <summary>
/// アプリケーションのメイン エントリ ポイントです。
/// </summary>
[STAThread]
static void Main()
{
    Application.Run(new Form1());
}
```


```C#
string val = split.Length > 1 ? split[1] : string.Empty;
```

条件演算子`?:`は、三項条件演算子とも呼ばれ、ブール式を評価し、ブール式の評価結果（`true`または`false`）に応じて、２つの式のいずれかの結果を返します。
```C#
string GetWeatherDisplay(double tempInCelsius) => tempInCelsius < 20.0 ? "Cold." : "Perfect!";

Console.WriteLine(GetWeatherDisplay(15));  // output: Cold.
Console.WriteLine(GetWeatherDisplay(27));  // output: Perfect!
```