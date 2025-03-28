# Source
- Data set: https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&search=toy
- Data Analyst Portfolio Project: Toy Store KPI Report in Power BI [https://www.youtube.com/watch?v=-TmginxY0vw]

# Tools
- Power BI

# Steps
## Loading Tables

- Date was _text_ had to change into _date_ + remove errors (right click).
- Product price was again _text_ and also contained $ sign. Had to change . -> , to get floating number.
  
  ![image](https://github.com/user-attachments/assets/42d76a45-c43f-47ec-8518-4f652c5cc2f0)


- The columns quick overview about quality and data  **View**  -> Column Quality / Column distincion
![image](https://github.com/user-attachments/assets/a5728389-b27a-45b1-9d84-c6c4cd06426d)
As profiling is based on 1000 first row, but we can change it to cover th whole table
![image](https://github.com/user-attachments/assets/f56dae80-dce7-4b5a-b3c9-305bd5d9101c)


- To grab easily lowest and highest product **View** -> **Profile**
![image](https://github.com/user-attachments/assets/d41495a4-7f35-40d7-bcd0-50d03577e8c3)
Click on the bar - 2.99 and it gives the product's name
![image](https://github.com/user-attachments/assets/9ab0bb2d-4d73-4d28-819e-ff007d3eec47)
NB! Do not forget to clear the filter.
![image](https://github.com/user-attachments/assets/3aa90344-574c-4ac6-88ce-70ce80937b9d)

  - Adding two columns _Start_Month_ and _Start_Week_ into _Calendar_ table.

## Creating Relational Model
 ![image](https://github.com/user-attachments/assets/eb07fd8f-7ced-4465-9b84-318564b84b4f)

### Star Model & Many:1 Relation
 ![image](https://github.com/user-attachments/assets/75172a2b-c5f1-4e43-bbff-548b294b194c)

### Creating Hierarchy
- Again right click
![image](https://github.com/user-attachments/assets/4e2a5407-ce4c-4cfb-a405-7f8947cb61f6)
- Then in attribute section choose&drag&drop
![image](https://github.com/user-attachments/assets/8ebbe538-98db-4e4b-a180-ae452b99f335)
- Result: ![image](https://github.com/user-attachments/assets/880258e3-225a-41fc-87e3-2346ff7a9cc8)

### Hiding Foreign Fields
Not to be shown in the reports
- Variant A: being on the field and click on the eye
- Variant B: turning on hiding on the right panel

![image](https://github.com/user-attachments/assets/6bfc1e37-a206-4d8d-9d0a-8d715030249e)

## Calculations
![image](https://github.com/user-attachments/assets/49841419-f271-49ae-b808-3ef90b07f06d)
- Adding new column _Cost_
![image](https://github.com/user-attachments/assets/53ae4779-5427-4453-84f7-e5a5d1f6f559)
- Pulling the data from another table with **RELATION** function

