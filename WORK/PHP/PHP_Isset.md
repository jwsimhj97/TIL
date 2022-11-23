### isset 함수란?
 - 변수가 설정되어있는지 확인해주는 함수이다. 
<br/> 변수값이 설정되어있지 않을때(null값일때) 사용한다.
<br/>
<br/>

#### 사용
##### 1. isset($var);
> $var가 설정되었는지 확인한다. 설정되었을 시 true, 설정되지 않았을 시 false를 반환한다.
```
$var1;              // false
$var2 = NULL;       // false
$var3 = "hi";       // true

if(isset($var1)){
    echo "<p>var1 is set.</p>";
}else{
    echo "<p>var1 is not set.</p>";
}


if(isset($var2)){
    echo "<p>var2 is set.</p>";
}else{
    echo "<p>var2 is not set.</p>";
}

if(isset($var3)){
    echo "<p>var3 is set.</p>";
}else{
    echo "<p>var3 is not set.</p>";
}

결과 : 
var1 is not set.
var2 is not set.
var3 is set.
```

##### 2. isset($var1, $var2, ...);
> $var1, $var2, ...이 설정되었는지 확인한다. 모든 변수가 설정되어있다면 true, 그렇지 않으면 false를 반환한다.
```
$var1 = "";         // true
$var2 = "Lorem";    // true
$var3;              // false

if(isset($var1, $var2)){
    echo "<p>var1 and var2 is set.</p>";
}else{
    echo "<p>var1 and var2 is not set.</p>";
}

if(isset($var1, $var3)){
    echo "<p>var1 and var is set.</p>";
}else{
    echo "<p>var1 and var3 is not set.</p>";
}

결과 :
var1 and var2 is set.
var1 and var3 is not set.
```
<br/>
<br/>



참조 https://ryangx2.tistory.com/157
