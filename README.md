####单步跳入:step into调试，进入语句中的子函数进行步进调试
####单步跳过:step over调试，跳过该行语句，进入下一行进行调试
####单步跳出:step out调试，跳出当前函数，进入调用源进行调试

####例如：
####1.
####if(aa=fun(xx,xx))  ←当前断点位置
####{
####aa=b;
####}
####当执行单步跳入后，进入fun()函数的第一句语句，继续调试

####2.
####aa=fun();←当前断点位置
####bb=aa;
####当执行单步跳过后，转到bb=aa;语句，继续调试

####3.
####fun()
####{
####aa=bb; ←当前断点位置
####bb=cc;
####cc=dd;
####}

####void main()
####{
####...
####fun();
####dd=ee;
####}
####当执行单步跳出后，转到main函数的dd=ee;语句，继续调试


##图片
![](https://github.com/GuardLDW/HelloWorld/blob/master/image/scream1.png)
![](https://github.com/GuardLDW/HelloWorld/blob/master/image/scream2.png)
![](https://github.com/GuardLDW/HelloWorld/blob/master/image/scream3.png)
![](https://github.com/GuardLDW/HelloWorld/blob/master/image/scream4.png)
![](https://github.com/GuardLDW/HelloWorld/blob/master/image/scream5.png)
