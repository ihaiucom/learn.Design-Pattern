# Command Pattern 命令模式
##Definition
Encapsulate a request as an object, thereby letting you parameterize clients with different requests, queue or log requests, and support undoable operations.
<br>命令模式将“请求”封装成对象，以便使用不同的请求、队列或者日志来参数化其他对象，同时支持可撤消的操作。

![](https://github.com/QianMo/Unity-Design-Pattern/blob/master/UML_Picture/command.gif) 

##Participants
The classes and objects participating in this pattern are:

###Command
* declares an interface for executing an operation

###ConcreteCommand
* defines a binding between a Receiver object and an action
* implements Execute by invoking the corresponding operation(s) on Receiver

###Client 
* creates a ConcreteCommand object and sets its receiver

###Invoker
* asks the command to carry out the request

###Receiver
* knows how to perform the operations associated with carrying out the request.


<br><br>


## 这个模式参与的 Class 和 Object:

###Command (命令)
* 声明 Execute 的 interface

###ConcreteCommand (具体命令)
* 定义绑定操作的接收对象
* 继承Command实现 Execute 方法

###Client （客户端）
* 创建具体的命令对象并设置它的接收器

###Invoker （调用）
* 请求命令执行请求

###Receiver (接收)
* 执行命令行为的描述.
