	> 文件名: FMp3Play
	>				Fmp is Mp3 Player流行的递归名字很cool是吧．
	>					学c一个月零七天的练手之做．我会做好它!
	
	> 简介: win下的调用mci函数的mp3播放工具．可以在命令行下执行.
	> 功能：可以单次和循环播放mp3和wav.未来将加入指定次数播放功能．
			这些功能将用参数形式在命令行下实现．
	> 初传时间：20171010
	
	> 使用方法：
		1.将快捷方式放在右键<发送到>菜单，直接把mp3发送到本工具上
		在命令行下输入命令:
		2.播放单曲：fmp xxx.mp3
		3.单曲循环：fmp r xxx.mp3
		4.播放全曲：fmp l
		5.关闭命令：fmp s
		
	>使用mgw_w64编译,各版mingw在win下编译百分之99有效，参考命令如下:
		生成发行版：gcc -o3 -s fmp.c -lwinmm -mwindows -o fmp.exe
		命令行测试版：gcc -Wall fmp.c -lwinmm -o fmp.exe
		
	注：命令4为播放当前目录下不含子文件夹的所有mp3	
	注：放入windows文件夹全局使用更方便

	
准备加入的功能：
用fmp l number xxx.mp3命令实现播放例表的指定单曲播放功能，
用fmp lr number xxx.mp3命令实现播放例表的指定单曲循环播放功能，

当功能成熟后，目标将代码转移为多平台．使用开源音频库以支持更多音频格式．
最后一步实现桌面歌词功能，这是我学习编程的初衷～希望一年内达到这个目标