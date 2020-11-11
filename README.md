# 2020322085 G201 林钰宸
# JAVA-4
## 1.实验内容
+ 1.设计两个管理接口：学生管理接口和教师管理接口。学生接口必须包括缴纳学费、查学费的方法；教师接口包括发放薪水和查询薪水方法。
+ 2.设计博士研究生类，实现上述的两个接口，该博士研究生应具有姓名，性别，年龄，每学期学费，每月薪水等属性。
+ 3.编写测试类，并实例化至少两名鄙视研究生，统计他们的年收入和学费。根据两者之差，算出每名博士级研究生的年应纳税金额。
## 2.实验要求
+ 1. 在博士研究生类中实现各个接口定义的抽象方法。
+ 2. 对年学费和年收入进行统计，用收入减去学费，求得纳税额。
+ 3. 国家最新纳税标准，属于某一时期的特定固定值，与实例化对象没有关系，考虑如何用static final修饰定义。
+ 4. 实例化研究生类时，可采用运行时通过main 方法的参数args一次性赋值，也可采用Scanner类实现运行时交互试输入、
+ 5. 根据输入情况，要在程序中做异常处理。
## 3.实验接口

```
public interface  Colleagestudent {
 public static void payment() {   //接口中的方法都是静态的方法	 
 System.out.println("你调用了交学费的方法");

 }
 public static void checkmany() {
	System.out.println("你调用了查学费的功能"); 
 }
 
}
public interface Teacher {
  public static void paysalary() {
	  System.out.println("这是发放薪水的方法");
  }
  public static void inquiresalary() {
	  System.out.println("这是查收薪水的方法");
  }
}

```
## 4.异常处理
```
try {
    		id1=sc.nextInt();
    		if(id1==b) {
    			System.out.println("你的学费支付了："+id1+"美元,支付成功");
         		break;
    		}else {
    			 System.out.println("你输入的有误");
    		}
     		
		} catch (Exception e) {
			str="您输入有误,请输入一个整数:";
			continue;
		} 	
```



## 5.实验感想
1. 学会了通过接口来实现调运并且接口不能定义
2. 学会了try 异常处理方法


