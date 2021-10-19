
# Applied Data Analytics

## Wedge Project
Getting everything uploaded correctly was difficult/tedious as I was not able to get it to work entirely programmatically. I was able to get the small (inactive files) to load but not the larger ones. The method I worked with Katherine to figure out where we uploaded to Google Cloud Storage and then made a transfer took quite a bit of time to figure out how to do correctly. Once we got it figured out it was pretty easy.
However, I was concerned about the potential for errors, missing a file, saving the wrong name and so on. When Andrew asked about how many rows we should have I figured I should check and did find I was missing quite a few. I think I was able to correct them for the most part. 


### Task 1
Task_1_HP.ipynb
Conects to GBQ and loads inactive files into into GBQ data set, and fixes one file that I couldn't get to transfer.

schema_for_cloud.txt
Schema file that was used when creating and uploading tables

### Task 2
Task_2_HP.ipynb
Connects to GBQ, creates list of owners, creates sample of owners, saves a xopy of the file locally and uploads both of these to GBQ. It then extracts records for all owners in the sample, and then checks the file size to see if I can upload it programaticly.
I did try to upload but it times out.

### Task 3

Task_3_Dept_Lookup_Table_HP.ipynb
Creates and loads a lookup table that translates department number to a text description

Task_3_Queries_HP.ipynb
Runs queries and creates txt files to be used in creation of database

Task_3_DB_HP.ipynb
Creates a SQL database with txt files

Wedge_Task_3_HP.db
Is the SQL Database that contains 3 tables; sales_by_date_by_hour, sales_by_owner_by_year_by_month, and 
sales_by_product_description_by_year_by_month.



## Query Comparison Results

Fill in the following table with the results from the 
queries contained in `gbq_assessment_query.sql`. You only
need to fill in relative difference on the rows where it applies. 
When calculating relative difference, use the formula 
` (your_results - my_results)/my_results)`. 



|  Query  |  Your Results  |  My Results | Difference | Rel. Diff | 
|---|---|---|---|---|
| Total Rows  | 85760126 | 85760139 | 13 | 1 |
| January 2012 Rows  | 1070906 | 1070907 | 1 | 1 |
| October 2012 Rows  | 1042286 | 1042287 | 1 | 1 |
| Month with Fewest  | February | February | Yes | NA  |
| Num Rows in Month with Fewest  | 6556770 |6556770 | 0 | 0 |
| Month with Most  | May | May | Yes | NA  |
| Num Rows in Month with Most  | 7578372 | 7578372 | 0 | 0 |
| Null_TS  | 7123792 | 7123792 | 0 | 0 |
| Null_DT  | 0 | 0 | 0 | 0 |
| Null_Local  | 234843 | 234843 | 0 | 0 |
| Null_CN  | 0 | 0 | 0 | 0 |
| Num 5 on High Volume Cards  | 14987.0 | 14987.0 | Yes | NA  |
| Num Rows for Number 5 |460630| 460630 | 0 | 0 |
| Num Rows for 18736  | 12153 | 12153 | 0 | 0 |
| Product with Most Rows  | banana organic | banana organic | Yes | NA  |
| Num Rows for that Product  | 908639 | 908639 | 0 | 0 |
| Product with Fourth-Most Rows  | avocado hass organic, if you consider the green patch donation a product, broccoli organic
if you don't |avocado hass organic, if you consider the green patch donation a product, broccoli organic
if you don't | Yes | NA  |
| Num Rows for that Product  | 456771 for avocados, and 344657 for broccoli| 456771 avocado, 344657 broccoli | 0 | 0 |
| Num Single Record Products  | 2769 | 2769 |   |   |
| Year with Highest Portion of Owner Rows  | 2014 | 2014 | Yes/No  | NA |
| Fraction of Rows from Owners in that Year  | 0.7592 | 0.7591 |-0.0001 | 1 |
| Year with Lowest Portion of Owner Rows  | 2011 | 2011 | Yes | NA |
| Fraction of Rows from Owners in that Year  | 0.7372 | 0.7372 | 0 | 0 |

## Reflections

<!-- I'd love to get 100-200 words on your experience doing the Wedge Project --> 

The project did feel a little daunting at times, but once everything was loaded it went pretty smoothly. I think it would help to have a little more practice loading the big files, I know several others who had the same problem. Maybe the SQL assignment could be in GBQ, that would give a little more practice with that interface. I appreciate how powerful that Could Platform is but it was very difficult to navigate at first. I did get to work with some classmates that I don't normally work with which was nice.
Once everything was loaded, I enjoyed some of the work. I thought it was really cool that you could run a GBQ query though Python.
I also thought it was interesting to learn how a database can be made, I have not done that before, and had wondered how they were created.
