# typescript-box
An enhanced version of the original typescript compiler.

安装
首先确保你已经安装了最近版本的node.js。然后执行如下命令就可以安装了：

npm install -g typescript-box


运行
直接在命令行调用 tsc-x 即可；

tsc-x [input files] [options]
命令行参数格式与原版tsc完全一致


额外参数
参数	类型	默认值	描述
accessorOptimization	boolean	false	如果get/set方法只含有一行对其他方法的调用，直接用那个目标方法作为get/set方法体
emitReflection	boolean	false	输出类的反射信息
reorderFiles	boolean	false	根据依赖关系自动排序源文件列表
defines	Object	 	将代码中出现的全局变量替换为对应的常量

这些参数除了 defines 只能在tsconfig.json中使用外，其他参数还可以通过命令行传入，例如 --reorderFiles 的形式。
