# <center>零知识 实验报告</center>

>**课程名称     <u>创新创业实践课程</u>  **       
>
>**学生姓名   <u>李路岩</u>      学号  <u>202022180198</u>**     
>
>**学院   <u>网络空间安全</u>学院    专业  <u>信息安全</u>**   

[TOC]

>****

## <center>实验思路</center>

>在不泄露自己真实信息的情况下，发给验证方，实现合理性与正确性

## <center>关键代码</center>

```python
  def check(sig):
    p=76519
    q=56123
    e=5
    n=p*q
    if pow(sig,e,n)>=425:
        return True
    else:
        return False
def employer(id,sig):
    if id not in chain.keys():
        return False
    elif check(sig)==False:
        return False
    else:
        return True
```





## <center>实验结果</center>

<a href="https://img.gejiba.com/image/EyHeYN"><img src="https://img.gejiba.com/images/f952900aac15b719f90a3f1fb4f02a0d.png" alt="f952900aac15b719f90a3f1fb4f02a0d.png" border="0"></a>
