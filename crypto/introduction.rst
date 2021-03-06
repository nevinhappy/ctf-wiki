..

密码学简介
==========

密码学（Cryptography）一般可分为古典密码学和现代密码学。

其中，古典密码学，作为一种实用性艺术存在，其编码和破译通常依赖于设计者和敌手的创造力与技巧，并没有对密码学原件进行清晰的定义。其主要包含以下几个方面

-  单表替换加密
-  多表替换加密
-  奇奇怪怪的加密方式

而现代密码学则起源于 20 世纪末出现的大量相关理论，这些理论使得现代密码学成为了一种可以系统而严格地学习的科学。现代密码学又可以简单的分为以下几个方面

-  对称密码，以 DES，AES，RC4 为代表
-  非对称密码，以 RSA，椭圆曲线加密为代表
-  HASH，以 MD5，SHA1，SHA512 等为代表
-  数字签名，以 RSA 签名，ElGamal 签名，DSA 签名为代表

其加密方式主要有两种方式

-  块加密
-  流加密

一般来说，密码设计者的基本想法是确保密码框架的

-  保密性
-  完整性
-  可用性
-  不可否认性

其中，前三者又称为 CIA 三元组。

而对于密码破解者来说，一般都是要想办法识别密码算法，然后利用暴力破解方法或者密码框架的漏洞进行破解。当然，也有可能是处于希望构造虚假的哈希值或者签名来绕过相应的检测。

一般来说，我们都会假设攻击者知道要攻破的密码体制，一般来说会有如下几种攻击类型，

+----------------+--------------------------------------------+----------------------------------+
| 攻击类型       | 说明                                       | 适用场景                         |
+================+============================================+==================================+
| 唯密文攻击     | 攻击者只拥有密文                           | 古典密码                         |
+----------------+--------------------------------------------+----------------------------------+
| 已知明文攻击   | 知道明文和对应的密文                       | 古典密码，对称密码，非对称密码   |
+----------------+--------------------------------------------+----------------------------------+
| 选择明文攻击   | 能够对选择一些明文加密后获得其相应的密文   | 对称密码，非对称密码             |
+----------------+--------------------------------------------+----------------------------------+
| 选择密文攻击   | 能够对选择一些密文解密后获得明文           | 非对称密码                       |
+----------------+--------------------------------------------+----------------------------------+


这里推荐一些资料

-  `可汗学院公开课 <http://open.163.com/special/Khan/moderncryptography.html>`__
-  `深入浅出密码学——常用加密技术原理与应用 <https://github.com/yuankeyang/python/blob/master/%E3%80%8A%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BA%E5%AF%86%E7%A0%81%E5%AD%A6%E2%80%94%E2%80%94%E5%B8%B8%E7%94%A8%E5%8A%A0%E5%AF%86%E6%8A%80%E6%9C%AF%E5%8E%9F%E7%90%86%E4%B8%8E%E5%BA%94%E7%94%A8%E3%80%8B.pdf>`__

.. attention:: 推荐在看完公开课的情况下，以及简单看看电子书的情况下在考虑是否要购买书，因为书买回来一般都被闲置起来了。。。

参考：

`维基百科-密码学 <https://zh.wikipedia.org/wiki/%E5%AF%86%E7%A0%81%E5%AD%A6>`__

.. attention:: 本部分大部分定义与例子参考了维基百科。