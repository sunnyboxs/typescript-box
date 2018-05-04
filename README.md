# typescript-box (TS编译器支持WebGL2.0)
An enhanced version of the original typescript compiler.

安装
首先确保你已经安装了最近版本的node.js。然后执行如下命令就可以安装了：

npm install -g typescript-box


# 运行
直接在命令行调用 tsc-x 即可；

tsc-x [input files] [options]
命令行参数格式与原版tsc完全一致


# 额外参数
参数	类型	默认值	描述
sortFiles	boolean	false	根据依赖关系自动排序源文件列表，默认为false关闭排序


# 开启排序
打开tsconfig.json 在compilerOptions下添加"sortFiles": true,

{
	"compilerOptions": {
		"sortFiles": true,
		"target": "es5",
		"declaration": true,
		"sourceMap": true,
		"outFile": "bin/js/Main.js",
		"noImplicitAny": false,
		"removeComments": false
	},
	"exclude": [
		"node_modules",
		"bin"]
}

# 切换vscode的typescript的sdk:
settings.json
{
    "typescript.tsdk": "C:/Users/xxxxxxx/AppData/Roaming/npm/node_modules/typescript-box/lib/"
}
