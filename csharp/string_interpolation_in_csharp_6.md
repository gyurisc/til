In C# 6.0, it is possible to embedd variables in the string literals instead of using string.Format. 
So, you can do this: 

Instead of this: 
 ```csharp
string name = "Jack";
string message = string.Format("You don't know, {0}.",name);
```

