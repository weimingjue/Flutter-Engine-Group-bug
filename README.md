# Flutter-Engine-Group-bug

### 项目来源：
* 该项目来源于flutter引擎组：https://github.com/flutter/samples/tree/main/add_to_app/multiple_flutters
* 改动代码：
```
//在MainActivity增加resume代码即可
fun onClickNext(view: View?) {
    ...
}
override fun onResume() {
    super.onResume()
    onClickNext(null)
}
```


### 复现步骤：
1. 运行Android项目
2. 多次按手机返回键返回上一个界面
3. 返回三次即可崩溃
