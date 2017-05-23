# Raw.Phenotype.Active.F4.txt
```
#%%
#!/usr/bin/env python

# we want to parse a raw file and extract information based on bytes position
# we only extract the bytes position based on format 4
# In python, index starts from 0 not 1 and always excludes the number on the right side. For examples, while extracting bytes position from 3 to 19(17-digit-animal-id), we have to give values like [2:19]

InFileName = "DRMS_UFL_Penagaricano_F4_Archive.txt"
InFile = open(InFileName,"r")
outputFile = open("Final_DRMS_UFL_Penagaricano_F4_Archive.txt", 'w')
#LineNumber = 0
string1 = []
i = 1
for Line in InFile:
    
    string1 = []
    Line = Line.strip('\n')
    string1 = (Line[2:19]  + " ")
    string1 = (string1 + Line[19:36] + " ")
    string1 = (string1 + Line[36:53] + " ")
    string1 = (string1 + Line[70:78] + " ")
    string1 = (string1 + Line[110:114] + " " )
    string1 = (string1 + Line[127:135] + " " )
    string1 = (string1 + Line[135:138] + " " )
    string1 = (string1 + Line[141:143] + " " )
    string1 = (string1 + Line[143:146] + " " )
    string1 = (string1 + Line[158:160] + " " )
    string1 = (string1 + Line[250:253] + " " )
    string1 = (string1 + Line[255:256] + " " )
    string1 = (string1 + Line[263:267] + " " )
    string1 = (string1 + Line[267:269] + " " )
    string1 = (string1 + Line[269:271] + " " )
    string1 = (string1 + Line[271:273] + " " )
    string1 = (string1 + Line[273:276] + " " )
    string1 = (string1 + Line[278:279] + " " )
    string1 = (string1 + Line[286:290] + " " )
    string1 = (string1 + Line[290:292] + " " )
    string1 = (string1 + Line[292:294] + " " )
    string1 = (string1 + Line[294:296] + " " )
    string1 = (string1 + Line[296:299] + " " )
    string1 = (string1 + Line[301:302] + " " )
    string1 = (string1 + Line[309:313] + " " )
    string1 = (string1 + Line[313:315] + " " )
    string1 = (string1 + Line[315:317] + " " )
    string1 = (string1 + Line[317:319] + " " )
    string1 = (string1 + Line[319:322] + " " )
    string1 = (string1 + Line[324:325] + " " )
    string1 = (string1 + Line[332:336] + " " )
    string1 = (string1 + Line[336:338] + " " )
    string1 = (string1 + Line[338:340] + " " )
    string1 = (string1 + Line[340:342] + " " )
    string1 = (string1 + Line[342:345] + " " )
    string1 = (string1 + Line[347:348] + " " )
    string1 = (string1 + Line[355:359] + " " )
    string1 = (string1 + Line[359:361] + " " )
    string1 = (string1 + Line[361:363] + " " )
    string1 = (string1 + Line[363:365] + " " )
    string1 = (string1 + Line[365:368] + " " )
    string1 = (string1 + Line[370:371] + " " )
    string1 = (string1 + Line[378:382] + " " )
    string1 = (string1 + Line[382:384] + " " )
    string1 = (string1 + Line[384:386] + " " )
    string1 = (string1 + Line[386:388] + " " )
    string1 = (string1 + Line[388:391] + " " )
    string1 = (string1 + Line[393:394] + " " )
    string1 = (string1 + Line[401:405] + " " )
    string1 = (string1 + Line[405:407] + " " )
    string1 = (string1 + Line[407:409] + " " )
    string1 = (string1 + Line[409:411] + " " )
    string1 = (string1 + Line[411:414] + " " )
    string1 = (string1 + Line[416:417] + " " )
    string1 = (string1 + Line[424:428] + " " )
    string1 = (string1 + Line[428:430] + " " )
    string1 = (string1 + Line[430:432] + " " )
    string1 = (string1 + Line[432:434] + " " )
    string1 = (string1 + Line[434:437] + " " )
    string1 = (string1 + Line[439:440] + " " )
    string1 = (string1 + Line[447:451] + " " )
    string1 = (string1 + Line[451:453] + " " )
    string1 = (string1 + Line[453:455] + " " )
    string1 = (string1 + Line[455:457] + " " )
    string1 = (string1 + Line[457:460] + " " )
    string1 = (string1 + Line[462:463] + " " )
    string1 = (string1 + Line[470:474] + " " )
    string1 = (string1 + Line[474:476] + " " )
    string1 = (string1 + Line[476:478] + " " )
    string1 = (string1 + Line[478:480] + " " )
    string1 = (string1 + Line[480:483] + " " )
    string1 = (string1 + Line[485:486] + " " )
    string1 = (string1 + Line[493:497] + " " )
    string1 = (string1 + Line[497:499] + " " )
    string1 = (string1 + Line[499:501] + " " )
    string1 = (string1 + Line[501:503] + " " )
    string1 = (string1 + Line[503:506] + " " )
    string1 = (string1 + Line[508:509] + " " )
    string1 = (string1 + Line[516:520] + " " )
    string1 = (string1 + Line[520:522] + " " )
    string1 = (string1 + Line[522:524] + " " )
    string1 = (string1 + Line[524:526] + " " )
    string1 = (string1 + Line[526:529] + " " )
    string1 = (string1 + Line[531:532] + " " )
    string1 = (string1 + Line[539:543] + " " )
    string1 = (string1 + Line[543:545] + " " )
    string1 = (string1 + Line[545:547] + " " )
    string1 = (string1 + Line[547:549] + " " )
    string1 = (string1 + Line[549:552] + " " )
    string1 = (string1 + Line[554:555] + " " )
    string1 = (string1 + Line[562:566] + " " )
    string1 = (string1 + Line[566:568] + " " )
    string1 = (string1 + Line[568:570] + " " )
    string1 = (string1 + Line[570:572] + " " )
    string1 = (string1 + Line[572:575] + " " )
    string1 = (string1 + Line[577:578] + " " )
    string1 = (string1 + Line[585:589] + " " )
    string1 = (string1 + Line[589:591] + " " )
    string1 = (string1 + Line[591:593] + " " )
    string1 = (string1 + Line[593:595] + " " )
    string1 = (string1 + Line[595:598] + " " )
    string1 = (string1 + Line[600:601] + " " )
    string1 = (string1 + Line[608:612] + " " )
    string1 = (string1 + Line[612:614] + " " )
    string1 = (string1 + Line[614:616] + " " )
    string1 = (string1 + Line[616:618] + " " )
    string1 = (string1 + Line[618:621] + " " )
    string1 = (string1 + Line[623:624] + " " )
    string1 = (string1 + Line[631:635] + " " )
    string1 = (string1 + Line[635:637] + " " )
    string1 = (string1 + Line[637:639] + " " )
    string1 = (string1 + Line[639:641] + " " )
    string1 = (string1 + Line[641:644] + " " )
    string1 = (string1 + Line[646:647] + " " )
    string1 = (string1 + Line[654:658] + " " )
    string1 = (string1 + Line[658:660] + " " )
    string1 = (string1 + Line[660:662] + " " )
    string1 = (string1 + Line[662:664] + " " )
    string1 = (string1 + Line[664:667] + " " )
    string1 = (string1 + Line[669:670] + " " )
    string1 = (string1 + Line[677:681] + " " )
    string1 = (string1 + Line[681:683] + " " )
    string1 = (string1 + Line[683:685] + " " )
    string1 = (string1 + Line[685:687] + " " )
    string1 = (string1 + Line[687:690] + " " )
    string1 = (string1 + Line[692:693] + " " )
    string1 = (string1 + Line[700:704] + " " )
    string1 = (string1 + Line[704:706] + " " )
    string1 = (string1 + Line[706:708] + " " )
    string1 = (string1 + Line[708:710] + " " )
    j = str(i)
    #print(j + " " + string1[0:] + "\n")
    outputFile.write(j + " " + (string1[0:]) + "\n")
    i = i + 1
InFile.close()
outputFile.close()

```


```
join string in python

#%%
InFileName = "Raw.MILK.Phenotype"
InFile = open(InFileName,"r")
outputFile = open("outputfile_MILK_Active.txt", 'w')
#LineNumber = 0
string1 = []
i = 1
for Line in InFile:
    #print(len(Line))
    string1 = []
    Line = Line.strip('\n')
    ElementList = Line.split(' ')
    s = "-";
    seq = ElementList[1]
    print(s.join([seq[:4],seq[4:6],seq[6:]]))
    #print(ElementList[7])
    #print(ElementList[1] )
    #rint(ElementList[6] + " " + ElementList[7] + '\n')
InFile.close()
outputFile.close()

```


```
how to extract a particular column in python using csv module

```

```
import pandas as pd
df = pd.read_csv("may22.csv",usecols = [1,2,5,9,10,11,12,15,16,17,20,21,22,25,26,27])
                                      #30,31,32,35,36,37,40,41,42,45,46,47,50,51,52,55,56,57,
                                      #60,61,62,65,66,67,70,71,72,75,76,77,80,81,82,85,86,87,
                                      #90,91,92,95,96,97,100,101,102,105,106,107)
print(df)
df.to_csv("columns_milk", sep='\t')

```


