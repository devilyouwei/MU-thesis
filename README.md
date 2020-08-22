# MU Thesis 📄

![Monmouth University](./logo.png)

This is Youwei's master thesis at Monmouth University

Jan 2020

## Schedule 📆

Jan 2020 to Aug 2020

## Achievements

1. System
2. Master Thesis

## Topic

The Search Engine Weighted on Resource Quality for Education and Learning

## Abstract

Nowadays the most common and convenient way to look for information is searching on Internet. The top Internet search engines are handful, such Google, Bing, Yahoo, Baidu, and so on. They use web crawler technologies to sniff the whole visible network and then provide users simple indexes and links as the results to help users find the source of resources. Most of those Internet search engines have good performance in terms of speed and precise keyword search ability, but wide-range search engines have their cons, such as massive potential results with uncertain quality. The goal of this project is to propose a new search engine, targeting on education, to provide “high quality” learning resources to users. High quality could be an subjective judgement and limited to the resources available for searching. In this project, it refers to means “user-trusted” or “user-liked”, based on common practices in education and learning. A few new search engine technologies are proposed to support efficient storage and enhanced searching for high-quality learning resources, in particular, to address two main issues: (1) how to build such a high-performance search engine; (2) how to define the quality of resources. The details include the strategies designed to optimize general information querying, storage, ranking, and most importantly, finding the relevant learning resources that are “high-quality” for users. Prototyping and experimental study are conducted to conceptually prove this research.

## Assets List

-   thesis
-   presentation slides
-   images for thesis
-   UML files for thesis
-   code (full project refer to [myresource-vue](https://github.com/devilyouwei/myresource-vue) and [myresource-node](https://github.com/devilyouwei/myresource-node))
-   other documents (not thesis)
-   test data

## Storage-Query

The statistics are generated randomly. Use the simulated data to test the search engine system.

### Dictionary

**Dic 1: 33 keywords**

_Redis Remote Dictionary Server is an in-memory data structure project implementing a distributed The project is mainly developed by Salvatore Sanfilippo and as of 2019 is sponsored by Redis Labs It is open-source software released under a BSD 3-clause license_

### Test Resources Amount Cases

Test search keywords time in 3 layers as the data increase.

-   33 keywords
-   4 keywords as test cases
-   order of magnitude in the database, generate random resources, index number based on 10, 10^0, 10^1, ... 10^6
-   static test results, without entering new rows of data
-   not random page, page 1
-   not rank

Note: million is the max data level, more data need opening to the public network.

| id  | total   | keyword     | count1 | count2 | count3 | layer1 | layer2 | layer3 |
| --- | ------- | ----------- | ------ | ------ | ------ | ------ | ------ | ------ |
| 1   | 1       | a           | 1      | 1      | 1      | 0.009  | 0.007  | 0.002  |
| 2   | 1       | is          | 1      | 1      | 1      | 0.003  | 0.002  | 0.001  |
| 3   | 1       | 2019        | 1      | 1      | 1      | 0.005  | 0.005  | 0.004  |
| 4   | 1       | open-source | 1      | 1      | 1      | 0.003  | 0.003  | 0.001  |
| 1   | 10      | a           | 9      | 8      | 8      | 0.004  | 0.004  | 0.003  |
| 2   | 10      | is          | 9      | 9      | 9      | 0.005  | 0.005  | 0.003  |
| 3   | 10      | 2019        | 6      | 6      | 6      | 0.005  | 0.005  | 0.003  |
| 4   | 10      | open-source | 4      | 4      | 4      | 0.002  | 0.004  | 0.002  |
| 1   | 100     | a           | 101    | 57     | 57     | 0.003  | 0.002  | 0.001  |
| 2   | 100     | is          | 93     | 83     | 83     | 0.003  | 0.002  | 0.002  |
| 3   | 100     | 2019        | 37     | 37     | 37     | 0.001  | 0.002  | 0.001  |
| 4   | 100     | open-source | 34     | 34     | 34     | 0.005  | 0.003  | 0.001  |
| 1   | 1000    | a           | 966    | 575    | 575    | 0.002  | 0.007  | 0.006  |
| 2   | 1000    | is          | 897    | 787    | 787    | 0.005  | 0.004  | 0.005  |
| 3   | 1000    | 2019        | 378    | 378    | 378    | 0.003  | 0.003  | 0.001  |
| 4   | 1000    | open-source | 349    | 349    | 349    | 0.004  | 0.004  | 0.002  |
| 1   | 10000   | a           | 9551   | 5747   | 5747   | 0.024  | 0.018  | 0.017  |
| 2   | 10000   | is          | 8803   | 7741   | 7741   | 0.022  | 0.021  | 0.021  |
| 3   | 10000   | 2019        | 3735   | 3735   | 3735   | 0.019  | 0.009  | 0.009  |
| 4   | 10000   | open-source | 3740   | 3740   | 3740   | 0.02   | 0.007  | 0.005  |
| 1   | 100000  | a           | 95395  | 58521  | 58521  | 0.137  | 0.012  | 0.117  |
| 2   | 100000  | is          | 88271  | 77922  | 77922  | 0.217  | 0.013  | 0.156  |
| 3   | 100000  | 2019        | 37902  | 37902  | 37902  | 0.156  | 0.008  | 0.069  |
| 4   | 100000  | open-source | 37819  | 37819  | 37819  | 0.189  | 0.008  | 0.09   |
| 1   | 1000000 | a           | 953614 | 585595 | 585595 | 1.965  | 0.095  | 0.873  |
| 2   | 1000000 | is          | 881562 | 777936 | 777936 | 2.001  | 0.132  | 1.212  |
| 3   | 1000000 | 2019        | 379714 | 379709 | 379709 | 1.963  | 0.072  | 0.636  |
| 4   | 1000000 | open-source | 379255 | 379246 | 379246 | 2.433  | 0.109  | 0.623  |

### Test Page Cases

Table 2 changed some environment variables. And get a different set of data

-   33 keywords
-   1 million resources in database
-   random pages: 1, 100, 10000, 50000, end
-   2 keywords as cases
-   not rank

| id  | keyword      | page  | layer1 | layer2 | layer3 |
| --- | ------------ | ----- | ------ | ------ | ------ |
| 1   | a            | 1     | 1.777  | 0.111  | 0.828  |
| 2   | a            | 100   | 1.675  | 0.084  | 0.848  |
| 3   | a            | 10000 | 2.528  | 0.261  | 0.925  |
| 4   | a            | 50000 | 2.991  | 1.6    | 0.884  |
| 5   | a            | end   | 3.197  | 2.585  | 0.775  |
| 1   | implementing | 1     | 2.34   | 0.098  | 0.606  |
| 2   | implementing | 100   | 2.4    | 0.078  | 0.578  |
| 3   | implementing | 10000 | 2.945  | 0.245  | 0.59   |
| 4   | implementing | 50000 | 2.678  | 1.973  | 0.597  |
| 5   | implementing | end   | 3.731  | 1.46   | 0.522  |

### Test Cases under high server pressure

Table 3 run query command under high pressure data operation (insert and update)

-   1 million data is inserting or udpating, high pressure server load, under 100-200 asynchronous reuqets per second.
-   1 million resources existed in the database
-   page 100
-   2 keywords as cases
-   not rank

| id  | keyword      | operation | layer1  | layer2  | layer3  |
| --- | ------------ | --------- | ------- | ------- | ------- |
| 1   | a            | insert    | 1.449   | 1.615   | 0.872   |
| 2   | implementing | insert    | 2.09    | 1.193   | 0.702   |
| 1   | a            | update    | 207.016 | 338.566 | 89.327  |
| 2   | implementing | update    | timeout | timeout | timeout |

### Test Cases with tanking

-   1 million resources existed in the database
-   rank = true, false
-   page 10000
-   2 keywords as cases

| id  | keyword      | rank  | layer1 | layer2 | layer3 |
| --- | ------------ | ----- | ------ | ------ | ------ |
| 1   | a            | false | 2.528  | 0.261  | 0.925  |
| 1   | a            | true  | 2.999  | 3.005  | 1.684  |
| 2   | implementing | false | 2.945  | 0.245  | 0.59   |
| 2   | implementing | true  | 2.522  | 2.532  | 1.095  |

## Conclusion

Although, at present, all kinds of search engines on the Internet are widely used, deep into people's daily Internet life. Our job is not to recreate a new search engine, but to improve the existing search engine technology. This paper mainly discusses the special search engine in the field of learning and education, which means that the search engine for learning resources is only suitable for learning purposes, and will not be used in the broad sense of search engine content. This is its limitation, but has also given its advantages: (1) Ensure the quality of search results; (2) Let users only focus on learning purpose; (3) Simplify the design and development of search engines.

The research in this paper focuses on two aspects, which are also the two most concerned issues of search engines: (1) search speed, (2) result ranking. Based on the improvement of the traditional search engine and the unique design and development mode in this particular area, this search engine adopts 3-layers storage structure to solve the issue 1. It uses the definition of resource value: DLRV ranking algorithm to solve the issue 2. The search engine is basically successfully applied to collecting and searching learning resources. At the same time, the theory has also been verified in the experimental environment. The results of experiments are basically consistent with the expected theory.

## Future Work

When we do the research on DLRV for learning resource search engine, there are still issues to be found. For example, the "query timeout" occurs when the database is updated under high pressure, the "reliability" of the six characteristics has two weights (refer to the section 5.3.1, B.Reliability) for the cetified personal account and organization which can not be accurately measured for the time being, more data orders need to be challeneged (as 1 billion resources).

The future direction of this research will still focus on solving two basic issues: storage-query and ranking resources based on DLRV. About the paging technology (refer to section 5.2.5) in the 3-layers storage structure, large pages can be further divided into small pages. The issue "query timeout" when updating the information of resources can be improved by adding ECS (Elastic Compute Service) servers like [Amazon EC2](https://en.wikipedia.org/wiki/Amazon_Elastic_Compute_Cloud). About the weight variables in characteristic "Reliability" value calculating, by processing more data fitting, more real user feedback can make a more reasonable weight value.

In addition to solving the more issues found, our system must pass the actual test of Internet running, that means we need to put the software online to the Internet and provide it to students, teachers, institutions, etc. In terms of resource collection, more learning resources need to be published through the vast number of Internet users. We hope that this set of search engine system for learning and educational resources can be widely used in human's Internet learning life.

## Contributors

Youwei Huang

Cui Yu

## Copyright

Monmouth University
