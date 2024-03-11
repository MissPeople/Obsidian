# 启动方式
1. 显示启动
	- class跳转
	![[111.png]]
	- 包名.类名跳转
	![[Pasted image 20240129122324.png]]
	- ComponentName跳转
	![[Pasted image 20240129122418.png]]
2. 隐式启动
	能够被隐式启动的activity必须在Manifest中配置Intent-filter，filter中有action, category和data，因此隐式启动需要intent能够匹配intent-filter设置的过滤信息。  
	- action的匹配规则
		- action是一个字符串，可使用系统预定或者自定义，**区分大小写，必须在intent-filter添加**
		- eg:AA->BB => BB中可以有一个或者多个action，AA设置intent的action时只能有一个
	- category的匹配规则
		- category内容也是一个字符串，系统预定了一些，也可以自己定义，**区分大小写，必须在Intent-filter添加**
		- category可以设定多个，那么每个都要和过滤规则中的其中一个相同。也就是说，比如过滤规则中的category有5个，那么intent可以从这个5个中选3个添加，也可以全部添加，也可以重复添加
		- 系统在调用startActivity或者startActivityForResult的时候会默认为Intent加上"android.intent.category.DEFAULT"(无论你的过滤规则中是否设定category，系统都会为你加上)，所以必须要在过滤规则intent-filter中加上“<category android:name=“android.intent.category.DEFAULT”/>”，否则会报错

# Action
	动作  

# IntentFilter
	用于描述一个activity或者InterntFilter能够操作哪些inten。