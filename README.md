# ResidualCurrent-RSUA
Data Collected using NI MyDaq for Medical Devices : SyringePump-RSKI-2020-04-080213 and Patient Monitor AM1500-M014A011344

Files are in txt Format with two Data Columns : time and Voltage.

You can import it using Python Pandas in Dataframe format.

To read them, first skip 4 rows. You can use **pd.read_csv(file_path, delimiter='\t', skiprows=4)**

Then, Convert commas to dot in column 'Y[0]', it was saved using Indonesian numeric format. You can use **.str.replace(',', '.')**

Finally, Convert column 'Y[0]' to numeric type, using **pd.to_numeric()**

Don't forget to cite the article for the introduction or methods being used, at Energies

[https://www.mdpi.com/1996-1073/19/10/2309](https://www.mdpi.com/1996-1073/19/10/2309)
