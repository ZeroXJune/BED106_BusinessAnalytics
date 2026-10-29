Checkpoint 3 Power BI project (v4)
=============================

DELETE ANY EARLIER COPY BEFORE YOU EXTRACT THIS.

Unzipping over a folder that already exists does NOT remove files that are no
longer in the archive. An earlier version of this project contained a file

    Checkpoint3_Dashboard.SemanticModel/definition/tables/DateTable.tmdl

which Power BI rejects with:

    The calculated column 'DateTable[Date]' cannot be used as a primary key
    of the table.

Power BI reads EVERY .tmdl file in the tables folder, so that one leftover file
breaks the project even though nothing refers to it any more.

What to do
----------
1. Delete the whole old Checkpoint3_Dashboard folder (and the two folders
   Checkpoint3_Dashboard.Report and Checkpoint3_Dashboard.SemanticModel).
2. Extract this zip into an empty folder.
3. Check: the tables folder must contain exactly these seven files —
      Annual.tmdl
      CategoryMonth.tmdl
      CustomerSegments.tmdl
      Geography.tmdl
      Monthly.tmdl
      Sales.tmdl
      SubcategorySegments.tmdl
   If DateTable.tmdl is there, you are still looking at the old folder.
4. Open Checkpoint3_Dashboard.pbip in Power BI Desktop.
5. It asks for FolderPath. The default is already

       C:\BED106\data\dashboard\

   Accept it if that folder holds the seven CSV files. If the CSVs sit
   directly in C:\BED106 instead, change it to

       C:\BED106\

   Either way it MUST end with a backslash. Check first: the folder you name
   has to contain monthly.csv, sales_detail.csv, category_month.csv,
   geography.csv, annual.csv, customer_segments.csv and
   subcategory_segments.csv.
6. Refresh, then File > Save as > Checkpoint3_Dashboard.pbix

If it still errors, build by hand instead: docs/PowerBI_Build_Guide.docx,
Part 1 onwards. Send me the exact message and I will fix the generator.
