###  task1:编写计时器类timer
##### 要求
1. timer.start()用于开始计时
2. timer.pause()暂停计时
3. timer.stop()停止计时
4. timer.clear()清除计时时间

### task2:编写功能测试
##### 要求:
1. 使用计时器，计算每次测试时间
##### 例子:
```
function test(callback,message,bool)
{
	timer.start();
	if(callback())
	{
		console.log(message+'：测试通过');
	}
	else
	{
		console.log(message+'：测试未通过');
	}
	if(bool)
	{
		console.log('测试时间为:'+timer.getDuration()+'毫秒');
	}
}
```
### task3:编写工具集并使用功能测试测试是否能用，并计算时间
##### 要求:
1. 工具至少包括一下几点
```
var utils = 
{
	uniqueArray	: 	uniqueArray,//数组去重
	isString	: 	isString,//判断是否为字符串
	isNumber	: 	isNumber,//判断是否为数字
	isObject	: 	isObject,//判断是否为对象
	isArray		: 	isArray,//判断是否为数组
	isFunction	: 	isFunction 	//判断是否为函数
}
```
2. 功能测试例子
```
	test(function ()
		{
			if(utils .isNumber({})===true)
				return 1;
			else
				return 0;
		},'isNumber',1);
//输出：
//isNumber：测试未通过
//test.js:203 测试时间为:1毫秒
```
	