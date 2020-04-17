# S2Kv2
Convert structural readings to kml files for display in Google Earth etc.
Download the S2Kv2.xlsm excel spreadhseet with macro and the Symbols folder to convert your structural measurements into a kml file for display in Google Earth or other virutal globes. 
Blenkinsop, T., 2012. Visualizing structural geology: From Excel to Google Earth. Comput. Geosci. 45, 52–56.

S2Kv2 (Structures to KML) Read Me
1. Introduction
This macro enabled Excel spreadsheet creates structural symbols from field measurements in a KML file for visualizing using virtual globes such as Google Earth.
Download S2Kv2 and the Symbols folder onto your desktop. Put them together in a single folder.
From your virtual globe, open the example file MaryKathleneExample.kmz in the S2Kfolder. You can appreciate all the basic attributes of S2K from this example.
2. Create a KML file from your own data
1. Open the S2K workbook in Excel.
For Excel Windows or Macintosh 2011: Use S2Kv2.xlsm
For Excel Windows 2007 and 2004 Macintosh: Use S2Kv2.xls
Make sure that the macro is enabled:
Macintosh: Enable macros when asked by the dialogue box.
Windows 2011: FileèOptionsèTrust Center-Trust Center settingsèMacro settingsèEnable all macros
It might be a good idea to save the workbook with a different name in the S2K folder. This name will become the name of the kml document.
To test the workbook, skip the data entry steps 2 to 7 below, and make a kml file from the data already entered by going straight to step 8.
2. Enter a worksheet name in cell B1 of the first Worksheet. This name will become the name of a folder within the kml document. A worksheet may correspond to a particular lithology or a structural domain. Cells with thick black borders require entries. You can overwrite the values that are supplied in Blanksheet1.
3. Enter the Scale and Height factors in cells D1 and F1: use the default values of 10 to begin with.
4. Choose Yes from the drop-down menus in Cells H1 and J1 if you have jpg files for the Key and Stereoplot. Otherwise choose No.
5. Add the type of structure e.g. Bedding in the cell next to “Structure”. No data will be written into the kml file without an entry in this cell. Repeat for as many different types of structure as you have in the domain
6. Choose a colour and a symbol for each structure from the drop down menus in cells F3 and F4.
7. Add your field data, starting in row 6:
• Columns A and B are UTM coordinates – these are optional.
• Columns C and D are latitude and longitude as decimal degrees,
negative latitudes in the southern hemisphere. The WGS84 datum must
be used. No data are read from any row without an entry in column C.
• Columns E and F are for your first type of structure e.g. bedding. Enter
a descriptor in cell F2. This name will become the name of a folder within the Worksheet folder. Enter your data as Dip Direction (E6) and Dip (F6) for planar structures, or Trend (E6) and Plunge (F6) for linear structures.
• Each pair of subsequent columns (G+H etc) will have data from different types of structure.
8. Fill Blanksheet 2 with data from a different lithology or structural domain. Up to 10 worksheets are provided. Any worksheet with a blank name in cell A2 will not appear in the kmz file. You can edit the names in the tabs of the worksheets to correspond with the folder name in cell B1.
8. Run the KMLCreator macro when you have entered and saved your data: Macintosh: Under ToolsèMacroèMacros
Windows: ViewèMacrosèView Macros
Select and run the KMLCreator macro. You will need to specify a path to the folder where you have the Symbols and the spreadsheet which must be together
9. Open the kml file in your virtual globe. The kml document will be created in the S2K folder, with the same name as the workbook (e.g. S2K.kml). The kml file must reside in the same folder as the workbook and the Symbols folder.
10. You will probably want to edit the workbook to change settings such as scale, height, colour and symbol to achieve the best effects.
Advanced Options
1. You can edit any symbol by opening the model file from the SketchUpModels folder in Google SketchUp. Export the edited model to the Symbols folder as a Collada (.dae) model, with a similar name to those in the folder.
2. You can increase the choices in the dropdown menus to include your own models and colours. Unhide the Selection worksheet, and add new cells to the lists of colours and symbols. You may then need to revalidate the cells with the drop-down menus to include your additional choices.
3. You can create a stand-alone kmz file to export your results by selecting the kml file and the Symbols folder, and the Stereonet.jpg and Key.jpg files if you have them, and compressing them together. Replace the .zip suffix by .kmz
Additional Information and Updates to S2K may be available from
