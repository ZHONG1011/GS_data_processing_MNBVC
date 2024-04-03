# GS_data_processing
针对原神多语言文本数据的简单分析与处理，将获得数据转换为jsonl文件。

该项目分为两个文件夹：
- Genshin_data （针对txt文本数据的处理）
- multilingual-genshin （针对json文件的数据处理）

因为个人之前并没有接触过原神，不太清楚其游戏文本内容的多少。因此可能存在数据收集不全面的情况，或有疏漏的地方，还望海涵。

## Genshin_data的txt文本数据
数据源自一些游戏的文本数据，详情参考ipynb文件。
> - 数据来源：https://github.com/Milkve/GenshinData；
> - 原数据路径为Genshin_data/Readable，载入后针对txt文档的数据情况进行探查；
> - 参考数据情况筛选文本，转换为jsonl进行输出

## 基于multilingual-genshin项目的json数据转换。

最初考虑的数据源是github上的genshin-db项目。
> 链接：https://github.com/theBowja/genshin-db
 
但在对比了multilingual-genshin上面的文件后，其内容基本上覆盖了genshin-db项目的文本数据内容。
> 具体参照：https://github.com/theBowja/genshin-db/blob/main/types/enums.d.ts

**项目详情**
- 选择multilingual-genshin项目的本地数据进行处理。来源：https://github.com/PseudoMon/multilingual-genshin
- 项目数据均在multilingual-genshin/data内，其中原数据在artedata、charadata、weaponsdata这三个文件中，皆为json文件。
- 使用jsonpath提取json数据，进行数据的分析处理，转换为txt文件输出。
- 将数据转换为jsonl格式输出。

如果希望探索更多、更详细的内容，我认为genshin-db项目中的数据是比较全面的，欢迎补充。
