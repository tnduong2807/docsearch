# Week 5 Lab Report - Commands

## 3 interesting command-line options or alternate ways to use grep:

**1.Use -c to display the count of number of matches:**

Example #1:

```
grep -c "HIV" technical/plos/pmed.0010036.txt

56
```

Example #2:

```
grep -c "report" technical/biomed/1468*

technical/biomed/1468-6708-3-1.txt:6
technical/biomed/1468-6708-3-10.txt:22
technical/biomed/1468-6708-3-3.txt:0
technical/biomed/1468-6708-3-4.txt:3
technical/biomed/1468-6708-3-7.txt:7
```

Example #3: 

```
grep -c "ID" technical/plos/pmed.00202*

technical/plos/pmed.0020200.txt:0
technical/plos/pmed.0020201.txt:0
technical/plos/pmed.0020203.txt:0
technical/plos/pmed.0020206.txt:0
technical/plos/pmed.0020208.txt:0
technical/plos/pmed.0020209.txt:0
technical/plos/pmed.0020210.txt:0
technical/plos/pmed.0020212.txt:0
technical/plos/pmed.0020216.txt:37
technical/plos/pmed.0020226.txt:0
technical/plos/pmed.0020231.txt:0
technical/plos/pmed.0020232.txt:0
technical/plos/pmed.0020235.txt:0
technical/plos/pmed.0020236.txt:0
technical/plos/pmed.0020237.txt:0
technical/plos/pmed.0020238.txt:0
technical/plos/pmed.0020239.txt:0
technical/plos/pmed.0020242.txt:0
technical/plos/pmed.0020246.txt:64
technical/plos/pmed.0020247.txt:4
technical/plos/pmed.0020249.txt:12
technical/plos/pmed.0020257.txt:12
technical/plos/pmed.0020258.txt:2
technical/plos/pmed.0020268.txt:0
technical/plos/pmed.0020272.txt:0
technical/plos/pmed.0020273.txt:0
technical/plos/pmed.0020274.txt:0
technical/plos/pmed.0020275.txt:0
technical/plos/pmed.0020278.txt:5
technical/plos/pmed.0020281.txt:0
```

The grep -c command is to display the number of lines that matches the given string or pattern. It is useful because we can find how many lines that contain the pattern in the contents of the files and know if the contents of the file have the keyword or not.

**2.Use -l to display the file names that have the contents matches the pattern:**

Example #1:

```
grep -l "surgeon" technical/biomed/*

technical/biomed/1471-2369-3-10.txt
technical/biomed/1471-2407-2-3.txt
technical/biomed/1471-2415-3-1.txt
technical/biomed/1471-2415-3-4.txt
technical/biomed/1472-6874-2-1.txt
technical/biomed/1472-6882-3-1.txt
technical/biomed/1472-6963-3-11.txt
technical/biomed/1477-7819-1-10.txt
technical/biomed/cc1044.txt
technical/biomed/cc303.txt
technical/biomed/cc367.txt
technical/biomed/cc713.txt
```

Example #2:

```
grep -l "doctor" technical/911report/*

technical/911report/chapter-1.txt
technical/911report/chapter-13.4.txt
technical/911report/chapter-5.txt
technical/911report/chapter-7.txt
```

Example #3:

```
grep -l "technical" technical/plos/*

technical/plos/journal.pbio.0020001.txt
technical/plos/journal.pbio.0020010.txt
technical/plos/journal.pbio.0020116.txt
technical/plos/journal.pbio.0020121.txt
technical/plos/journal.pbio.0020146.txt
technical/plos/journal.pbio.0020147.txt
technical/plos/journal.pbio.0020183.txt
technical/plos/journal.pbio.0020187.txt
technical/plos/journal.pbio.0020215.txt
technical/plos/journal.pbio.0020228.txt
technical/plos/journal.pbio.0020310.txt
technical/plos/journal.pbio.0020394.txt
technical/plos/journal.pbio.0030024.txt
technical/plos/journal.pbio.0030056.txt
technical/plos/pmed.0020071.txt
technical/plos/pmed.0020102.txt
technical/plos/pmed.0020158.txt
technical/plos/pmed.0020182.txt
technical/plos/pmed.0020212.txt
technical/plos/pmed.0020242.txt
```

The grep -l command is to display the files that contains the given string/pattern. It is useful because we could locate the files that contains the given string and it could save so much time to find the names of the files.

**3.Use -n to show the line number while displaying the contents that conatains the string:**

Example #1:

```
grep -n "biomed" technical/biomed/*
technical/biomed/1471-2105-3-16.txt:16:        The availability of biomedical literature in electronic
technical/biomed/1471-2105-3-17.txt:526:        study aimed at enabling the biomedical community to cope
technical/biomed/1471-2164-3-18.txt:810:          in Gel/Mount (biomeda) containing 4',6
technical/biomed/1471-2164-3-7.txt:8:        of biomedical research. These include, but are by no means
technical/biomed/1471-2202-2-8.txt:334:          paper http://www.biomedcentral.com/1471-2202/2/9), and
technical/biomed/1471-2202-2-9.txt:499:        http://www.biomedcentral.com/1471-2202/2/8). It is now
technical/biomed/1471-2474-2-3.txt:7:        http://www.biomedcentral.com/1471-8219/2/5
technical/biomed/1472-6807-1-1.txt:17:        types of ligands could therefore have important biomedical
technical/biomed/1472-6882-1-12.txt:472:        biomedical framework. While the SR method has been used in
technical/biomed/1472-6882-3-3.txt:10:        literature search in biomedicine depends on the appropriate
technical/biomed/1472-6882-3-3.txt:17:        The controlled vocabulary for biomedicine has been
technical/biomed/1472-6882-3-3.txt:22:        biomedical literature [ 3 ] . With the recent development
technical/biomed/1472-6882-3-3.txt:49:        Other biomedical databases that include CAM literature,
technical/biomed/1472-6882-3-3.txt:240:          biomedicine and it has a subset focusing on complementary
technical/biomed/1472-6882-3-3.txt:620:          biomedicine, investigators and authors in the fields of
technical/biomed/1472-6920-2-3.txt:214:        international journals [ 5 ] . For biomedical disciplines
technical/biomed/1472-6947-3-5.txt:49:        another level of biomedical data integration in which array
technical/biomed/1472-6947-3-8.txt:56:          Creators of biomedical databases use terminologies to
technical/biomed/1472-6947-3-8.txt:624:        biomedical data sets. Public comment is welcomed.
technical/biomed/1475-9276-1-3.txt:143:        33 34 ] . This model has been widely applied in biomedical
technical/biomed/1477-7827-1-54.txt:695:        study increases the biomedical significance of findings
technical/biomed/gb-2001-2-4-research0012.txt:516:        biomedicine of the visual computer language paradigm [ 24,        
technical/biomed/gb-2001-2-4-research0012.txt:532:        to biomedical education, investigation and industry. For
technical/biomed/gb-2003-4-4-r28.txt:493:        biomedical research community. GoMiner is flexible both
technical/biomed/gb-2003-4-7-r46.txt:75:        gene annotations or concepts from the biomedical
```

Example #2:

```
 grep -n "billions" technical/plos/*

technical/plos/journal.pbio.0020053.txt:21:        Antibiotics have traditionally been plucked from nature's battleground. For billions of
technical/plos/journal.pbio.0020272.txt:68:        are replicated billions of times, which operate on a fast time scale and are easy to get
technical/plos/journal.pbio.0020276.txt:64:        elements of their immunoglobulin and T-cell receptor genes to create billions of clones
technical/plos/journal.pbio.0020347.txt:137:        the millions and billions of genetic trials and errors that have been evaluated by nature
technical/plos/journal.pbio.0020439.txt:167:        photosynthesis to the billions of years of living evolution on Earth. Relevant spatial
technical/plos/journal.pbio.0030024.txt:6:        Armed with billions of cells, elaborate circuitry, and a seemingly animate anatomy,
technical/plos/pmed.0020099.txt:10:        tuberculosis and malaria continue to affect billions of people, and a rapidly escalating
```

Example #3:

```
grep -n "millions" technical/biomed/*

technical/biomed/1471-2105-3-30.txt:118:          separately for each window and thus hundreds of millions
technical/biomed/1471-2164-3-10.txt:261:          ESTs (2.5 millions ESTs) from dbEST as well as the ESTs
technical/biomed/1471-2164-3-10.txt:262:          from Incyte Genomics' LifeSeq database (5.1 millions
technical/biomed/1471-2164-4-21.txt:457:        produces millions of fold amplification in as little as 20
technical/biomed/1471-2180-3-4.txt:288:        millions of years, under appropriate conditions. Cano and
technical/biomed/1471-2180-3-4.txt:433:        hundreds of millions of years in earthly systems further
technical/biomed/1471-2180-3-4.txt:487:        millions of years, even in the dry cold-storage environment
technical/biomed/1471-2334-1-10.txt:18:        the erroneous treatment of millions of non-malaria cases
technical/biomed/1471-2334-1-21.txt:168:          millions copies/mL. The median of viral load was 23,420
technical/biomed/1472-6963-1-8.txt:7:        hospitalizations, and millions of workdays lost each year.
technical/biomed/1477-7827-1-6.txt:369:        selection) for millions of years.
technical/biomed/cvm-2-1-038.txt:159:        testing - costing several years and tens of millions of
technical/biomed/gb-2000-1-2-research0003.txt:17:        studies, which often consist of millions of measurements. A
technical/biomed/gb-2001-2-8-research0027.txt:74:        containing tens of millions of nucleotides. The algorithm
technical/biomed/gb-2001-3-1-research0005.txt:244:        supposed to contain an identical distribution of millions
technical/biomed/gb-2002-3-10-research0052.txt:621:        refractory to analysis after millions of years of
technical/biomed/gb-2002-3-12-research0086.txt:1292:          chromosome arms to be maintained over millions of years.
technical/biomed/gb-2002-3-9-research0044.txt:71:        millions of single-pass sequence reads, have been generated
technical/biomed/rr167.txt:544:        1shows many millions of protegrin molecules are bound to an
```

The grep -n command is to show the line number of file with the line matched the given string. It is useful because we could locate the lines that conatins the given string in many different files that contains that given string and it could save so much time to find lines in differents files that have the given string.