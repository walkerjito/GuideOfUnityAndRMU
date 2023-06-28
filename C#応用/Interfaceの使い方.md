# interface の使い方

:::note
簡略化するためにコンソールアプリ用のコードになっています。
:::

```C#:Program.cs
class Program
{
    static void Main(string[] args)
    {
        ITest tester = new TestA();
        
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

