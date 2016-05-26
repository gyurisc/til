# Dictionary initializer in C# 6.0 

I am still not sure if I like this syntax or not, but this is how to initialize a Dictionary in C# 6.0 

```csharp
   Dictionary<int, string> names = new Dictionary<int, string> {
      [1] = "John",
      [2] = "James",
      [3] = "Jane",
      [4] = "Kathy"
   };
```
