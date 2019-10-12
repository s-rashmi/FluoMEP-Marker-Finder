# FluoMEP-Marker-Finder
Tool to find unique markers from FluoMEP profiles
System Requirements

1.Windows, Linux, Solaris or Mac OS
2.Java Runtime Environment (JRE) or J2SE - can be downloaded from http://java.sun.com/

Installation of FMF in Windows

1.Download FluoMEP_Marker_Finder_1.0.zip and save the file in desired location.
2.Extract the files in the zip folder. NOTE: Make sure all the files in the zip folder are extracted to the same location.
3.Double-click FluoMEP_Marker_Finder_1.0.jar to start the application

User Manual for FMF

1.Double-click FluoMEP_Marker_Finder_1.0.jar to start the application. 

2.In the Input Data tab, click Open. A file chooser pops up. Choose the desired *.csv file. The name of the file appears in the text box.
	
3.Click Male Markers tab. 

4.In the panel Number of Profiles & Percentage for 1 Combination, specify the user parameter required.
a.MALE (FEMALE) is the number of male (female) profiles present in each primer combination in the dataset.
b.Selecting Pooled Samples indicates the dataset contains data from pooled samples. The percentage options are deactivated. 
c.Selecting Individual Samples indicates the dataset contains data from individual samples. The percentage options are activated.
d.Min. percentage of males required to show expression is the minimum number of male samples required (in percentage) to show presence of a peak, for the peak to be considered a male marker. For pooled samples, this option is deactivated and a default value of 100% is used.
e.Min. percentage of females required not to show expression is the minimum number of female samples not required (in percentage) to show presence of a peak, for the peak to be considered a male marker. For pooled samples, this option is deactivated and a default value of 100% is used.

5.In the Threshold panel, the minimum peak height filter is set. For males, a default of 300 rfu is set. Thus, male peaks below height of 300 rfu are rejected. For females, a default of 0 rfu is set as all female peaks are considered for comparison against males.

6.	In the Fold panel, the minimum factor the male peak heights must be greater than the female peak heights to be considered a marker. The default setting is 3, i.e. a male peak height must be at least 3 times higher than the corresponding female peak height to be considered a marker.

7. Click Marker to get your results.
The output file would be in the same destination as the input file

Things to Note

1.All input files must contain the three columns Sample File Name, Size and Height. If the other columns (Dye/Sample Peak, Marker, Allele, Area and Data Point) are present in the file, then they must appear in the following order: Dye/Sample Peak, Sample File Name, Marker, Allele, Size, Height, Area, Data point.
2.Troubleshooting for JAR files: http://www.netbeans.org/kb/articles/javase-deploy.html 
	
