# 原版

https://github.com/praetorian-inc/PortBender

# 修改

原本为cs反射dll加载，已经修改为exe方式运行，相较于原版的区别就是，执行的所有参数全部要使用双引号包裹。

```
Redirect Usage: PortBender "redirect FakeDstPort RedirectedPort"
Backdoor Usage: PortBender "backdoor FakeDstPort RedirectedPort password"
Example:
        PortBender "redirect 445 8445"
        PortBender "backdoor 443 3389 praetorian.antihacker"
```

# 补充

https://reqrypt.org/windivert-faq.html#q5

代码中fix了win2003的编译相关报错，但注意 Windows XP、Windows 2003 或早期版本的 Windows 不支持WinDivert.sys驱动，所以该系统版本下无法使用。
