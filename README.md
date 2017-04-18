//引入系统模块
var http=require('http');
//创建服务器
http.createServer(function (req,res) {
    //响应内容
    res.end('Hello,Node.js');
    //监听端口3000
});



//用require 去引入一个 console 库

var console1=require('console');

console.log('asas大的');



//1.输出日志.log=info 等价
console.log('啊啊啊啊');
console.info('啊啊啊啊啊');

//2.输出断言,由开发者定义错误的内容

console.assert(1 !== 100,'1绝对不等于100');

var obj={
    name:'张三',
    age:100,
    sex:'2'
};

var obj2=new Object();
obj2.name='李四';
obj2.setName=function (name) {
    this.name=name;
};

//3.用来打印对象
console.log(obj2);


//4.一般用来打印错误  warn=error 等价
console.error('你报错');
console.warn('出错了');

//5.time 和 timeEnd

console.time('timer');
for (var i=0;i<10000;i++){

}
