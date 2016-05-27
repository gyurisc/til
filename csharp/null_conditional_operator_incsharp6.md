# Null-Conditional operator in C# 6.0 

In C#, you can write the following 

```csharp
  var street = person?.address?.street; 
```

instead of 
```csharp 
  var street = null;
  
  if(person!=null)
  {
    if(person.address!=null)
    {
      street = person.address.street; 
    }
  }
```

Rather usefull... 
