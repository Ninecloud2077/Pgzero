# Pgzero
_Based on Pygame-Zero_  
_Remake by Ninecloud_  
可以规定窗口名的pgzrun  
## 用法
在`pgzrun.go()`函数中使用`Title`参数  
也可以不传递参数，默认为`Pygame Zero Game`
## 制作方法
非常简单  
在pgzrun.py的`go()`函数中有变量`mod`  
为其加上`TITLE`属性即可
### 参考代码
```python
def go(Title='Pygame Zero Game'):
    """Run the __main__ module as a Pygame Zero script."""
    if getattr(sys, '_pgzrun', None):
        return

    mod.TITLE=Title
    run_mod(mod)
```
## 实践用处
https://github.com/Ninecloud2077/Pgzrun-Minis
