# How to strip whitespace from beginning and end of a string

This is a short tip on how to strip a string in python from all whitespace from beginning and the end. 

``` python
        name = "\r\n  String with all kinds of whitespace junk   \r\n"
        print name.strip()
```
Result will be 

``` bash 
String with all kinds of whitespace junk
```
