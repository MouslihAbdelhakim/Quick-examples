# Quick-examples
## Introduction
This repo hosts examples files for [the Quick tool hosted here](https://github.com/MouslihAbdelhakim/Quick)
## Content of repository
This reporsitory contains 4 pairs of files, these are grouped into two pairs of files and orginized under two different directories.

The delimited directory contains files with a CSV format and a ';' char as the columns delimiter. The fixedlength directory contains files with a fixedlength columns with different width. Inside each of these directories you'll find two subdirectories containing each a pair of files.

The identical subdirectory contains two files that Quick will consider as containing the same information using the filesDescriptions.xml in the project's root directory. The different subdirectory contains two files that Quick will consider as containing different information using the filesDescriptions.xml in the project's root directory.

To prepare for these examples :
  * [get the Quick jar from here](https://github.com/MouslihAbdelhakim/Quick/releases)
  * download this repo by either cloning it or downloading it as a zip file
  * copy quick.jar into the project's directory

After the preparation execute any or all of the following cammands: 

  * compare two different delimited files
    
    `java -jar quick.jar -d filesDescriptions.xml -i delimited delimited/different/ordersTableDump-01-12-2017.csv delimited/different/ordersTableDump-01-01-2018.csv`

  * compare two identical delimited files
    
    `java -jar quick.jar -d filesDescriptions.xml -i delimited delimited/identical/ordersTableDump-01-12-2017.csv delimited/identical/ordersTableDump-01-01-2018.csv`

 * compare two different fixed length files
    
    `java -jar quick.jar -d filesDescriptions.xml -i fixedlength fixedlength/different/ordersTableDump-01-12-2017.csv fixedlength/different/ordersTableDump-01-01-2018.csv`

* compare two identical fixed length files
    
    `java -jar quick.jar -d filesDescriptions.xml -i fixedlength fixedlength/identical/ordersTableDump-01-12-2017.csv fixedlength/identical/ordersTableDump-01-01-2018.csv`
