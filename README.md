# GS_data_processing
针对原神多语言文本数据的简单分析与处理，将获得数据转换为jsonl文件
该项目分为两个文件夹：
- Genshin_data （针对txt文本数据的处理）
- multilingual-genshin （针对json文件的数据处理）

## Genshin_data的txt文本数据
数据源自一些游戏的文本数据，详情参考ipynb文件。

## 基于multilingual-genshin项目的json数据转换。
来源：https://github.com/PseudoMon/multilingual-genshin
> 数据文件夹路径为public/data

最初考虑的数据源是github上的genshin-db项目。
> 链接：https://github.com/theBowja/genshin-db
 
但在对比了multilingual-genshin上面的文件后，其内容基本上覆盖了genshin-db项目的文本数据内容。
> 具体参照：https://github.com/theBowja/genshin-db/blob/main/types/enums.d.ts

因此直接下载了multilingual-genshin项目的本地数据进行处理。但仍存在数据收集不全面的可能性（因为我没有了解过原神的内容），或有疏漏的地方，还望海涵。如果希望探索更多的内容，我认为genshin-db项目中的内容是比较全面的，欢迎补充。
