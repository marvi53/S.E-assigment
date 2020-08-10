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

2nd summary:
                  DETERMINING THE INTRINSIC STRUCTURE OF PUBLIC SOFTWARE DEVLOPMENT HISTORY:


This is written by Antoine Pietri(paris, france) ,Stefano Zacchiroli(paris, france) ,Guillaume Rousseau(paris, france) they are determining the intersinc structure of public software devlopment history. In 7th international conference on mining software Repositories, October 5-6,2020,seoul repulic of korea,ACM, Newyork, NY, USA it is about to be 4 pages .
INTRODUCTION:
    free open source software(FOSS) and collabrative devlopment platforms become more popular and famous , and past deacades has made publicly avalable and the wealth of software source code(any type of code) artifacts(type).source code fiels contains commits which is called metadata(it is data about data or code),tagged relased etc. which is more usefull and benificaal in software engneering(ESE) and mining software repository(MSR) research, basically version controll system(VCS) (is a system that records  changes to a file or set of files over time) has been frequently analyzed due to advance software evolution which makes easy to exploitation.now days systematic initatives has been devloped to collect as much public VCS data as possible in a single logical place.By the main structure we will use here software heritage and its data set.It is the largest and many type of collection of diffrent type of code(source code). it is about more than 5 billion source code files(which are unique and diffrent) and contain 1 billion unique commits. which were collected 1 billion unique commits,which were collected from more than 80 million software projects.
Merkle DAG: it is large global graph linking together fully duplicated source code and its types(files, commits,directories,release,etc).but the actual source code files are reprsented as blob nodes. to that place which will distribute them (e.g: Git repositories), providing a unified and diffrent view on the whole software commas. the global version controll system (VCS) is a large and very difficult complex network which will genrate in result of human activity of software devlopment system . we can understand it easily and study it by using the classic techniques from network theory or network topology of the software heritage, network topology is the way in which the network is arranged inculude its physical apperance or loggical description of how the links nodes are setup to realate to each others.
software heritage: largest platform  and more popular system for collabrative devlopment system.

the main goal of this resarch is to collect or conduct the first sytematic resarch study on the intrinsic structure (internal structure) of the global graph of source code and its artifacts(type) which are stored in all publicaly available version control system. 

RESEARCH: specifically  we will perform an resarch(exploratory) study . in this research not any kind of hypothesis included.
Q1 what is the distribution of indegrees, out degrees and local clustering? which law do they fit?  (topology based)

Q2 what is the distribution of connected component sizes?     (Modularity)

Q3 what is distribution of shortest path lengths from roots to leaves?   (Height of network)

RESULT:
1,obtain the most recent new version of the software heritage graph dataset.
2,we have compressed a graph using compression techniques, so that the VCS graph structure can be fits in to memory.these graph can be accesses from on will be in the compressed graph representation via the web graph java API.
3, compute indegress/out degress and local clustering using standard algorithms(RQ1).
4, compute connected components using standard algorithms(RQ2).
5, create shortest path and spaning trees to graph leaves trhen measure lengths. this can be implemented with custom java code realizing Dijkstra is algorithm on top of the webgraph API.

* we will analyze the global version control system graph as a naturally occuring complex network and determine its internsic structure.
* to that end we will start from the software heritage graph dataset, compress it, and apply standard analysis techniques from network theory.
* findings will allow to compare the global VCS graph to other large networks and help determining how to analyze all public code in future MSR|ESE studies.

