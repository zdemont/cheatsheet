Get all methode from an object
```python 
object_methods = [method_name for method_name in dir(object)
                    if callable(getattr(object, method_name))]
```
