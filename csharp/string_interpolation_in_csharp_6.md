In C# 6.0, it is possible to embedd variables in the string literals instead of using string.Format. 
So, you can do this: 
 ```csharp
string name = "Jack";
string message = $"You don't know, {name}!";
```
Instead of this: 
 ```csharp
string name = "Jack";
string message = string.Format("You don't know, {0}!",name);
```

Escaping the interpolated string is done using {{ in case of { character and }} in case of } character. The " character is esxcaped by \". 

 ```csharp
 string name = "Jack";
string json = $"{{ \"name\" : \"{name}\"}}";

```


