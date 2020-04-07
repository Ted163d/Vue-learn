TypeScript学习：



//1.字符串也支持模板字符串

let user = {

name:'jack',

age:18

}

let str: string = `

大家好，我叫：${user.name}

我今年 ${user.age}岁了

`

//2.定义数组

let arr : number[] = [1,2,3]

let arr0:  string[] = ["hello","word","!"]

let arr1: array<number> = [1,2,3]

let arr2: array<string> = ["大家好","我叫","今年18岁了"]



//3.定义元组：有不同数据类型的数组

let arr: [number,string] = [10,'jack']



//4.定义对象

//重用

interface Person {

name: string,

age:number

}

let user: Person {

name: 'jack',

age: 18

}



//5.定义any

let num: any =10

num = 'ss'



//6.类型除了用于申明变量之外，还可以用于函数传参

function add(x: number,y: number) number {

return x+y

}

var ret: number = add(10,20)

//void只能用于函数返回值

function fn(): void {

console.log('hello')

}



//7.函数

//构造函数

function Person(name: string,age: number) {

this.name = name,

this.age = age

}

//方法

Person.prototype.sayhello = function() :void={

console.log(this.name,this.age)

}

//调用

let p1 = new Person('jack',18)

p1.sayhello()

//新

class Person {

name:string;

age:number;

constructor(name:string,age:number){

this.name=name,

this.age = age

}

sayhello():void{

console.log(this.name,this.age)

}

}

// 管道过滤器

public today ：any=new Date()

{{today | date: 'yyyy-MM-dd HH:mm ss'}}









