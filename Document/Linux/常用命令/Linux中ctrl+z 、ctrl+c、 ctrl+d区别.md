ctrl+c,ctrl+d,ctrl+z在linux程序中意义和区别

ctrl+c和ctrl+z都是中断命令,但是他们的作用却不一样.
 
ctrl+c是强制中断程序的执行,,进程已经终止。
 
ctrl+z的是将任务中止（暂停的意思）,但是此任务并没有结束,他仍然在进程中他只是维持挂起的状态,用户可以使用fg/bg操作继续前台或后台的任务,fg命令重新启动前台被中断的任务,bg命令把被中断的任务放在后台执行.
 
例如:当你vi一个文件是,如果需要用shell执行别的操作,但是你又不打算关闭vi,因为你得存盘推出,你可以简单的按下ctrl+z,shell会将vi进程挂起~,当你结束了那个shell操作之后,你可以用fg命令继续vi你的文件。
 
ctrl-d 不是发送信号，而是表示一个特殊的二进制值，表示 EOF。

注：在shell中，ctrl-d表示推出当前shell.