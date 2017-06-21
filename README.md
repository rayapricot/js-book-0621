# 6/21 課題 学んだ記録

自身が学んだ記録を作りましょう。

- 関数(`function` で始まるコード)は全て function.js に書きます
- その他をREADME.md（このファイル）に書いていきます
    - 書き方は README-example.md (同じフォルダに同梱) を参考にしてください
- 書き方は自身でアレンジしてもかまいません


--------------------------------------

## 授業スライドの説明（4時間目～5時間目）

説明の中で実行したログ、分かったこと、疑問などがあればここに書く。

### Consoleの実行ログ

```
var examinationScores = [
	59,84,77,53,41,20,42,53,55,54,
	36,48,64,70,45,54,42,50,49,53,
	68,60,66,57,52,55,82,61,51,43,
	57,65,81,63,45
];
undefined
function calculateTotal(scores) {
	var total = 0;
	for (var index = 0; index < scores.length; index++) {
		total += scores[index];
    }
	return total;
}

function calculateAverage(scores) {
	return calculateTotal(scores) / scores.length;
}
undefined
var informationExaminationScores = [
	59,84,77,53,41,20,42,53,55,54,
	36,48,64,70,45,54,42,50,49,53,
	68,60,66,57,52,55,82,61,51,43,
	57,65,81,63,45
];
var englishExaminationScores = [
	60,69,56,65,61,43,65,52,59,61,
	51,51,68,68,45,64,49,60,59,55,
	52,60,59,48,56,55,67,63,54,36,
	50,55,63,50,50
];
undefined
var examinationScores = [[
	59,84,77,53,41,20,42,53,55,54,
	36,48,64,70,45,54,42,50,49,53,
	68,60,66,57,52,55,82,61,51,43,
	57,65,81,63,45
],[
	60,69,56,65,61,43,65,52,59,61,
	51,51,68,68,45,64,49,60,59,55,
	52,60,59,48,56,55,67,63,54,36,
	50,55,63,50,50
]];
undefined
examinationScores[0];
examinationScores[1];
examinationScores[0][0];
59
examinationScores[0];
(35) [59, 84, 77, 53, 41, 20, 42, 53, 55, 54, 36, 48, 64, 70, 45, 54, 42, 50, 49, 53, 68, 60, 66, 57, 52, 55, 82, 61, 51, 43, 57, 65, 81, 63, 45]
examinationScores[0];
examinationScores[1];
examinationScores[0][0];
59
var information = 0;
var english = 1;
examinationScores[information];
examinationScores[english];
examinationScores[information][0]; //
59
function double(x) {
return x * 2; // 引数を二倍にして返す関数
}

undefined
double(1)
2
double(2)
4
var number = [1,2,3,4,5];
undefined
numbers.map(double)
VM973:1 Uncaught ReferenceError: numbers is not defined
    at <anonymous>:1:1
(anonymous) @ VM973:1
numbers.map(double)
VM975:1 Uncaught ReferenceError: numbers is not defined
    at <anonymous>:1:1
(anonymous) @ VM975:1
function double(x) {
return x * 2; // 引数を二倍にして返す関数
}

undefined
var number = [1,2,3,4,5];
undefined
numbers.map(double)
VM981:1 Uncaught ReferenceError: numbers is not defined
    at <anonymous>:1:1
(anonymous) @ VM981:1
var numbers = [1,2,3,4,5];
undefined
numbers.map(double)
(5) [2, 4, 6, 8, 10]
function foo() {
	return "hello";
}
undefined
var a = function foo() {
	return "hello";
}
undefined
var a = function() {
	return "hello";
}
undefined
var a = function() {
	return "hello";
}
undefined
var a = () => {
	return "hello";
}
undefined
var numbers = [1,2,3,4,5];
undefined
//ふつうの無名関数
numbers.map(function(x) {
return 2 * x;
})
(5) [2, 4, 6, 8, 10]
// アロー関数（正式）
numbers.map((x) => {
return 2 * x;
})
(5) [2, 4, 6, 8, 10]
//アロー関数　（省略した書き方）
numbers.map(x => 2 * x)
(5) [2, 4, 6, 8, 10]
function f(n) {
if (n <= 0) {
	return 1;
}
return n * f(n - 1);
}
undefined
f(3) // 3*2*1
6
f(5)
120
f(1)
1
function newCounter() {
var count = 1;
return () => count++;
}
undefined
var couter1 = newCounter();
undefined
var counter2 = newCounter();
undefined
var counter1 = newCounter();
undefined
var counter2 = newCounter();
undefined
counter1()
1
counter1()
2
counter2()
1
counter2()
2
counter2()
3
counter1()
3
counter1()
4
window.alert === alert;
true
window.innerWidth === innerWidth;
true
sampleValue = 5;
5
window.sampleValue;
5
```

### Console以外の動き（もしあれば）

【ここに書く（なければ省略可）】

### 分かったこと

【ここに書く】

### 疑問・分からないこと（もしあれば）

【ここに書く（なければ省略可）】

--------------------------------------

以下、教科書の自分で読んだ・実行した箇所について書く。

## 5-x ○○ (p.xx)

### Consoleの実行ログ

```
sampleValue = 5;
5
window.sampleValue;
5
var sampleHashMap = {};
undefined
smpleHashMap['test'] = 5;
VM1815:1 Uncaught ReferenceError: smpleHashMap is not defined
    at <anonymous>:1:1
(anonymous) @ VM1815:1
sampleHashMap['test'] = 5;
5
sampleHashMap['test']
5
sampleHashMap.test;
5
sampleHashMap.test = 7;
7
sampleHashMap.test;
7
var sampleHashMap = { test : 11 };
undefined
sampleHashMap.test;
11
function sampleFunction(message = 'test'){return message};
undefined
var functionVar = sampleFunction;
undefined
functionVar;
function sampleFunction(message = 'test'){return message}
functionVar();
"test"
functionVar('hoge');
"hoge"
functionVar;
function sampleFunction(message = 'test'){return message}
function callTarget(target){ return target(); };
undefined
function returnSomeString(){return 'Sample';};
undefined
function returnSomeFunction(){return returnSomeString;};
undefined
callTarget(returnSomeString);
"Sample"
returnSomeFunction();
function returnSomeString(){return 'Sample';}
returnSomeFunction()();
"Sample"
```

### Console以外の動き（もしあれば）

【ここに書く（なければ省略可）】

### 分かったこと

【ここに書く】

### 疑問・分からないこと（もしあれば）

【ここに書く（なければ省略可）】
