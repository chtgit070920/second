# second
# 1、在dev上修改，未add，switch 到master -->master 上可以看到dev 工作区的修改
# 2、在dev上修改，add，但未commit，switch 到master -->master 上可以看到dev 暂存区的修改
# 3、在dev上修改，add，且commit，switch 到master -->master 上可以看到master 最后一次修改

为什么？
1.在工作区做了修改，add且commit到DEV的分支，再切换回master——
这时候，对master来说，工作区/暂存区没有任何“未提交的changes”（因为所有changes都已经commit）。
则工作区内容应该是与master分支最后一次提交的内容一致。

2.在工作区做了修改，没有提交到DEV分支（没有add、仅add但未commit），切换回master——
这个时候，对master来说，工作区/暂存区有了“未提交的changes”，那么就保持工作区的现有状态即可。

####
edit at dev 16:31:59

####
edit at master.