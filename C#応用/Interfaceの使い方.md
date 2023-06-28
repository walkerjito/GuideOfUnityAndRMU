# interface の使い方

:::note
簡略化するためにコンソールアプリ用のコードになっています。
:::

```C#:Program.cs
class Program
{
    static void Main(string[] args)
    {
        ITest tester = new TestA();  // ... 5
        
        tester.Foo();

        tester = new TestB();

        tester.Foo();
    }

}

public interface ITest  // ... 1
{
    void Foo(); //  ... 2
}

public class TestA : ITest  // ... 3
{
    public void Foo()   // ... 4
    {
        Console.WriteLine("TestA's Foo method did.");        
    }
}

public class TestB : ITest
{
    public void Foo()
    {
        Console.WriteLine("TestB's Foo method did.");
    }
}
```

1\. 実現させたクラスで必ず使えるメソッドやプロパティを宣言させる

2\. メソッドは外から必ず使えるため、自動的に public になるため、修飾子はいらない

3\. TextA クラスに ITest インターフェイスを実現させることを宣言している

4\. インターフェイスで宣言したメソッドを実際に定義している

5\. 変数を宣言する時は インターフェイスの型で宣言する
それによって必要なメソッドだけを使うようになる