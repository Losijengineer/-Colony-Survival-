# Colony Survival Chinese Patch

For game Colony Survival.

Colony Survival自制汉化补丁，汉化完成度91%

使用方法1（简单向，可能出错）：
1. 下载`zz-ZZ`目录下的三个文件。
2. 找到Colony Survival的安装目录（一般在...\Steam\steamapps\common\Colony Survival）
3. 进入该目录下的`gamedata`的`localization`文件夹，将三个文本文件复制进去，替换原有文件

使用方法2（较为复杂，可靠性高）：
1. 下载`zz-ZZ`目录下的名为`zz-ZZ.json`的文件。打开该文件，记下开头部分`coverage`的值（保留两位小数）。
2. 找到Colony Survival的安装目录（一般在...\Steam\steamapps\common\Colony Survival）
3. 进入该目录下的`gamedata`的`localization`文件夹，将`zz-ZZ.json`复制进去。
4. 打开`modInfo.json`，将末尾的内容更改如下（注意第4行至第9行）：
```
...
				"fileType" : "addOrOverrideLocalization",
				"index" : -1000000
			},
			{
				"relativePath" : "zz-ZZ.json",
				"fileType" : "addOrOverrideLocalization",
				"index" : -1000000
			}
		]
	}
]
```
5. 打开`localecoverage.md`，添加`| zz-ZZ | X% |`。其中`X`为你刚刚记下的`coverage`的值。小数点要用逗号。

最后打开游戏，选择语言`zz-ZZ`即可。
