## Introduction 

## Database tables
- ### Table name
> #### Description 
>> ##### Fields

- ### Table name
> #### Description 
>> ##### Fields

- ### Table name
> #### Description 
>> ##### Fields

- ### Table name
> #### Description 
>> ##### Fields


- ### Table name
> #### Description 
>> ##### Fields




## Pages
> ### Page ModelCriteria
> <img src="/home/bahri-khalid/Pictures/Screenshots/criteria1.png" alt="your-image-description" style="display:block; margin:auto;">
> <img src="/home/bahri-khalid/Pictures/Screenshots/criteria2.png" alt="your-image-description" style="display:block; margin:auto;">

> ### Page MCD

> <img src="/home/bahri-khalid/Pictures/Screenshots/criteriaMCD.png" alt="your-image-description" style="display:block; margin:auto;">

```
CREATE TABLE Bank (
  bank_id INT PRIMARY KEY auto_increment,
  name VARCHAR(50),
  country VARCHAR(50)
);
```
```
CREATE TABLE Selected_Feature (
  feature_ID INT PRIMARY KEY auto_increment,
  feature_Name VARCHAR(50),
  feature_Description VARCHAR(255),
  feature_Type VARCHAR(50)
);
```
```
CREATE TABLE Model_Criteria (
  model_Criteria_ID INT PRIMARY KEY auto_increment,
  label VARCHAR(50),
  bank_id INT,
  FOREIGN KEY (bank_id) REFERENCES Bank(bank_id)
);
```
```
CREATE TABLE Selected_Feature_Model_Criteria (
  feature_ID INT auto_increment,
  model_Criteria_ID INT,
  PRIMARY KEY (feature_ID, model_Criteria_ID),
  FOREIGN KEY (feature_ID) REFERENCES Selected_Feature(feature_ID),
  FOREIGN KEY (model_Criteria_ID) REFERENCES Model_Criteria(model_Criteria_ID)
);


```

---

> ### Page ModelParametrazation
> <img src="/home/bahri-khalid/Pictures/Screenshots/modelParam1.png" alt="your-image-description" style="display:block; margin:auto;">
> <img src="/home/bahri-khalid/Pictures/Screenshots/modelParam2.png" alt="your-image-description" style="display:block; margin:auto;">

> ### Page MCD

> <img src="/home/bahri-khalid/Pictures/Screenshots/modelMCD.png" alt="your-image-description" style="display:block; margin:auto;">

```sql
df
```

---


> ### Page Activation
> <img src="/home/bahri-khalid/Pictures/Screenshots/activation1.png" alt="your-image-description" style="display:block; margin:auto;">
> <img src="/home/bahri-khalid/Pictures/Screenshots/activation2.png" alt="your-image-description" style="display:block; margin:auto;">

> ### Page MCD

> <img src="/home/bahri-khalid/Pictures/Screenshots/activationMCD.png" alt="your-image-description" style="display:block; margin:auto;">

```sql
df
```