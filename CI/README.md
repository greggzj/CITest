
1) Support Python 3.6 +
2) Guide refer to https://github.com/malini/500lines/tree/master/ci



# MixIn类

- MixIn Class是可以被几个相互功能独立的class所共用的方法抽象出来的类。
- MixIn Class是不能被实例化的   

在这个项目中`test_runner.py`中的`ThreadingTCPServer`继承了`(socketserver.ThreadingMixIn, socketserver.TCPServer)`，ThreadingMixIn对TCPServer进行扩展，支持了多线程，在每一个request到来后新开一个thread来处理这个request。

ThreadingMixIn Class的存在，使得用户可以继承这个类来支持TCPServer或者UDPServer这样的一次只能处理一个request类一次能够处理多个request，被不同的Class共用。


# git clean -d -f -x

git-clean - Remove untracked files from the working tree

- `-d` recursive delete for folder
- `-f` force
- `-x` Remove only files ignored by Git.    


# Python2 to Python3 Modification

本项目github上基于python2编写，不支持python3