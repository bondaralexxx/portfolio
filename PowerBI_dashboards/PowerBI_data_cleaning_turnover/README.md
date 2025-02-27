In this project I focuseed primarily on data preparation and cleaning.
On the example of the structure of wholesale turnover of wholesale enterprises of Ukraine, according to information from the Ministry of Statistics of Ukraine.

Initially I had the file in Power Query in the following form, which was absolutelly unsuitable for correct construction of the report. 

![initial_state_file_img_1](https://github.com/user-attachments/assets/eae74112-7b98-4db8-8040-acee0fd09cba)

![initial_state_file_img_2](https://github.com/user-attachments/assets/3109f24d-744e-4961-bc3c-ddfba3348118)

What was done:
1. Rows and columns with NULL values was removed.
2. The first row was made as a header ("Use First Row as Headers").
3. Columns were renamed to the correct names and columns data type was checked.
4. The Category column was edited to an acceptable form
   - "Transform" - Extract;
   - "Transform" - Format - Trim, Cleane.
5. From a "wide" table made a "long" table, which is more convinient for building PowerBI reports (using "Transform" - Transpose).
6. Unpiwot columns.

In the end we got the file in the following correct form:

![final_state_file_img](https://github.com/user-attachments/assets/a644f3fa-e47d-4aed-ac60-75935c1b1af0)

This helped to quickly and correctly build a simple report that shows the dynamics of turnover.

![report_img](https://github.com/user-attachments/assets/405f3a1a-92b3-45eb-8b2c-1753d086e4cd)



