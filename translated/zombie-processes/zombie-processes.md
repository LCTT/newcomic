极客漫画：僵尸进程
===============

![Zombie Processes](http://turnoff.us/image/en/zombies.png)

- 在一个普通的 Linux 内核中发生的一幕……
- 它们怎么会变成僵尸进程的？
- 它们的父亲太忙了，不管它们了……

在 Unix 进程模型中，父进程和其所产生的子进程是异步运行的，所以如果子进程在结束后，会留下一些信息需要父进程使用 `wait`/`waitpid` 来接收。而如果父进程太忙了，没有调用 `wait`/`waitpid` 的话，子进程就会变成僵尸进程。

---
via: http://turnoff.us/geek/zombie-processes/

作者：[Daniel Stori][a]
译者 & 校对：[wxy](https://github.com/wxy)
合成：[合成者ID](https://github.com/合成者ID)
点评：[点评ID](https://github.com/点评者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]:http://turnoff.us/about/
