# GS_data_processing_MNBVC
针对原神多语言文本数据的简单分析与处理，将获得数据转换为jsonl文件。

**PS：目前可直接查看Genshin_AnimeGameData.ipynb文件了解具体流程**

该项目分为两个文件夹：
- Genshin_data （针对txt文本数据的处理）
- multilingual-genshin （针对json文件的数据处理）

## Genshin_data的txt文本数据
数据源自一些游戏的文本数据，详情参考ipynb文件。
> 数据来源：https://github.com/Milkve/GenshinData

- 原数据路径为Genshin_data/Readable，载入后针对txt文档的数据情况进行探查；
- 查看数据情况筛选文本，转换为jsonl进行输出（jsonl大小为11.3M）

## 基于multilingual-genshin项目的json数据转换。

最初考虑的数据源是github上的genshin-db项目。
> 链接：https://github.com/theBowja/genshin-db
 
但在对比了multilingual-genshin上面的文件后，其内容基本上覆盖了genshin-db项目的文本数据内容。
> 具体参照：https://github.com/theBowja/genshin-db/blob/main/types/enums.d.ts

**项目详情**
- 选择multilingual-genshin项目的本地数据进行处理。来源：https://github.com/PseudoMon/multilingual-genshin
- 项目数据均在multilingual-genshin/data内，其中原数据在artedata、charadata、weaponsdata这三个文件中，皆为json文件。
- 使用jsonpath提取json数据，进行数据的分析处理，
- 将数据转换为txt文件，保存至json_to_txt文件夹中（可能ipy文档的输出路径需要修改一下）
- 将数据转换为jsonl格式输出。（jsonl大小为32.7）

该项目仅作兴趣学习使用，若有侵权，还请联系。
