# S2iD Database

The **S2iD** is a Brazilian database focused on both natural disasters (frost, floods, heavy rains, etc.) and man-made disasters (erosion, water contamination, etc.). It's structured by municipality and has data available from 2003 to 2016.

This database presents three primary challenges:

1. It is distributed across various .xls files, each corresponding to a specific Brazilian state and reference year.
2. Not all .xls files share the same structure, meaning there are differences in column numbers, variable names, and so on.
3. There's no standardization in disaster descriptions. For instance, some entries use the term 'TORNADO' while others use 'TORNADOS'.

To address these issues, I use Python to merge the .xls files into a single .csv file named `df_s2id.csv`. More details on this merging process can be found in the `concatenate_xls` file. Furthermore, I've categorized the diverse types of disasters into two classes— with the first being more detailed than the latter. These classifications are described in the `classes.csv` file.

After concatenation and classification, manipulating and extracting information from the S2iD database becomes more straightforward.

## Final Notes:
- For the years 2010, 2011, and 2012, the original database does not contain a column specifying the state to which the municipality belongs.
- Between 2010 and 2011, the 'RITO' variable was not disclosed.


![Alt text](https://raw.githubusercontent.com/fms-1988/datas/main/s2id.png)







