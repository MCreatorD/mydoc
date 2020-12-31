使用sphinx来进行线程 API接口的说明
===============
当前主要说明在linux系统编程中所遇到的API进行记录和测试说明
 
linux中的线程共享整个进程的内存空间.
线程是任务调度的最小单元也就是说一个进程最少还有一个线程

1.线程的创建和退出
----------------
线程使用::

	#include <pthread>
	
	编译链接输入:-pthread

创建线程::

	int pthread_create(pthread_t *thread, const pthread_attr_t *attr,
				  void *(*start_routine) (void *), void *arg);
			  
	参数说明	pthread_t 类型的变量地址交由函数内部创建口给pthread_t 对象的内存空间赋值,attr属性输入配置	  

再是正常的文本段.
 
Or automatically numbered:
 
 #. Item 1
 #. Item 2
 
2.进程
-------------
Words can have *emphasis in italics* or be **bold** and you can define
code samples with back quotes, like when you talk about a command: ``sudo`` 
gives you super user powers!