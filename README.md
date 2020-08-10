# S.E-assigment
Marvi 2K18/CSM/53

                    LEARNING TO DETECT TABLE CLONES IN SPREADSHEETS:

This paper is written by Yakun Zhang, Wensheng Dou, Jiaxin Zhu, Dan Ye, and Bo Yang.2020.
learning to detect table clones in spreadsheets. In  proceedings of the 29th ACM Sigsoft international symposium on spoftware testing and analysis (ISSTA'20)July 18-22,2020, Virtual event ,USAm ACM, New York, NY, USA. it is consists of 13 pages.
INTRODUCTION:
     Spreadsheet is most succesfull and end-user programming platforms, it is used in diffrent bussines tasks, for the data storage , data analysis , financial reporting, etc.
In 2012 there was about 55 million user in united state work with spreadsheet.now days many more user are working with spreadsheet around the whole world. Spreadsheet are code too. In convential programming and in source code spreadsheet play similar role and code can be reused similar code reuse, end-user can reuse the existing spreadsheet to for speed up their devlopment productivity and saave the amount of time. for example the user can make a new financial report by copying-pasting-modifying the existing one . two tables which were created by copy-paste-modify, they share the same or similar computational semantics. we can refer them  as a table clone. it is similar to code clone in conventinal programming. table clones used to determined some important spreadsheet analysis scenarios. 
First, table is used to detect the same errors scattered in many spreadSheets.
Second, table improper modification may cause the error in table clones, and cause of financial losses.
Third, table mainly clones are used to perform the same bussines tasks , so the data analysis tools e.g: PowerBI can extract and analyze the all tables clones togather.
Fourth, table clones usually share common computational semantics and structures.
Microsoft excel has no records in spreadsheet systems.they are documenting that two tables are created by copy-paste-modify. so it is important to detect in spreadsheet table clones. and should focous on clone with the same data structure.
Our emperical study on the real-world spreadsheet from EUSES and Enron Corpora shows that 
58.5% of table clones involves in a structural changes, which can not find by existin  g approch. and also code clone detection in convential programs, e.g CCFinder, Deckad, clone detective , and CCLearner cannot be applied on spreadsheets. because programming model is totally diffrent in conventinol programs.
In this paper we propose LTC(learning to detect table clones) with or without structure changes in spreadsheet. if two tables has same structures and formats then they are to be a table clone, and also has same computaional semantics . therefore we are using table clone detection to classifying two tables as a clone or non-clone based on their structure and format similarities.
we evalute LTC on real-world spreadsheet form the EUSES and Enron. corpon, which are two of the most widely used corpora for spreadsheet resarch. The enviromental result show that LTC can detect table clones effectively, with a precision of 97.88% and recall of 92.1%, table clone precision of 37.5% and recall of 11.1%.
The main goal and contribution of this paper:
* we propose a commnly-used notation ion spreadsheet, table clone, in which two tables share the similar computational semantics.
* we suggest a lerning based approch LTC, to find table clone with or without structure changes.
* we implement LTC and evalute it on real world spreadsheet from the EUSES and Enron Corpora. the experimental results show that LTC and detect tables clones effictively.

RESARCH:
In this paper we prepare the following resarch question.
(RQ1) How effective is LTC in detecting table clone in spreadsheets?
(RQ2) How is LTC compared with existing techniques, e.g: Table-check?
(RQ3) Is LTC robust on diffrent dataset?

RESULT:
* we evalute LTC with the built ground truth and observe its performance . and LTC is a very effective in detecting table clones in spreadsheets. and the precision and recall for LTC is 97.8% and 92.1% .(RQ1)
*we evalute LTC and table check with the built ground truth to compare their performance  and  the LTC significantly outperforms taablecheck in table clone detection. the percision and recall for table check is 37.5% and 11.11%. as a comparision,the percission and recall for LTC is 97.8% and 92.1%, respectively,(RQ2).
*we evalute LTC on some larger data set e.g:FUSE, EUES, and Enron and manually validate the detected table clones ,Table clones are common in real-world spreadsheets.LTC can detect inter and intra spread-sheet table clones preciesely.

* In this papaer we observe that the tables in a table clone usually share the similar structure and formats. based on observation then we propose a learning based approcch, LTC detect the table clones with or without structural changes. Our experiments based on real world spreadsheets from the EUSES and Enron copra show that ,LTC can detect table clone effeectively, and significantly outperforms existing table clone detection tachniques. in future we also plan to purse the resarch directions.
 
