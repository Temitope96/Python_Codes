# Python_Codes
Featured in this Repository are the personal projects I undertook using Python ranging from Solving Real-World problems to analyzing and visualizing large amount of datasets. 


## Tentative Financial Structure / Plan
This is a script that uses python to provide a Starter-Financial Plan or Structure that many can use to reduce financial stress due to lack of proper financial structure.


![financial_stress](https://spivacklaw.com/wp-content/uploads/2017/09/feeling-financial-stress.jpg?fit=scale)


##📙: Table of Contents
- 📰: Project Overview
- 🛠️: Tools & Skills
- 📖: Script/Code

## 📰: Project Overview
Depression, as one of the most common mental health problems, marked by sadness, loss of interest or pleasure, feelings of guilt, low self-worth, disturbed sleep and lack of appetence, feelings of tiredness as well as poor concentration, is a leading cause of disability and poor health on a global scale. 

Over the decades, research has shown that one of the economic determinant of depression is Financial Stress as positive associations are noticeable between financial stress and depression. Although, it is observed in high, low, and middle-income earners, studies have indicated that it is more prevalent and stronger among populations with low-income (impoverished societies).

This project stemmed from a resolve to mitigate/extenuate the depressive effects of Financial worries on Human Life and wellness. It seeks to provide a financial paln/structure by requesting only two informations  - Monthly Financial Income as well as Marital Status - from its users. It aims at reducing the amount of people living from Paycheck-to-Paycheck for the rest of their lives by practicing a simple and basic wealth creation technique - management and savings.

(Citation: PubMed Central (PMC), National Library of Medicine, https://pmc.ncbi.nlm.nih.gov/articles/PMC8863240/)


## 🛠️: Tools & Skills
- Jupyter Notebook
- Math Library
- Variables and Dictionary
- FOR Loop
- IF/ELSE Statements

## 📖: Script/Code
<details><summary>View Script</summary>
<p>
``` bash
import math
salary = int(input('How much do you earn monthly? E.g - 200000, 500000, 1000000, 2000000\n Do not add commas'))
status = input('What\'s your marital status? E.g - single, married')

Salary_plan_D = [{'category':'Tithe', 'value':(10/100 * salary)}, #===Tithe is for God bro
               {'category':'Savings', 'value':(50/100 * salary)}, #=== Savings is 50%
               {'category':'Survival', 'value':(15/100 * salary)}, #=== Survival is 10%
               {'category':'Fittings', 'value': (15/100 * salary)}, #=== Fittings is for equipping your body and home
               # After a while, this fittings can be saved as an EMERGENCY FUND
               {'category':'Charity/Lifestyle', 'value':(10/100 * salary)} #=== Lifestyle is for flex and can be added to survival
               ] #=== This is the plan for Two(2) million naira and above salary earners

Salary_plan_C1 = [{'category':'Tithe', 'value':(10/100 * salary)}, 
               {'category':'Savings', 'value':(50/100 * salary)}, 
               {'category':'Survival', 'value':(25/100 * salary)}, 
               {'category':'Others', 'value': (10/100 * salary)}, 
               {'category':'Charity/Lifestyle', 'value':(5/100 * salary)}
               ] #=== This is the plan for One(1) million naira and above salary earners who are single

Salary_plan_C2 = [{'category':'Tithe', 'value':(10/100 * salary)}, 
               {'category':'Savings', 'value':(50/100 * salary)}, 
               {'category':'Survival', 'value':(30/100 * salary)}, 
               {'category':'Others', 'value': (5/100 * salary)}, 
               {'category':'Charity/Lifestyle', 'value':(5/100 * salary)}
               ] #=== This is the plan for One(1) million naira and above salary earners who are married

Salary_plan_B1 = [{'category':'Tithe', 'value':(10/100 * salary)}, 
               {'category':'Savings', 'value':(50/100 * salary)}, 
               {'category':'Survival', 'value':(30/100 * salary)}, 
               {'category':'Others', 'value': (5/100 * salary)}, 
               {'category':'Charity/Lifestyle', 'value':(5/100 * salary)}
               ] #=== This is the plan for five hundred thousand (500k) naira and above salary earners that are single

Salary_plan_B2 = [{'category':'Tithe', 'value':(10/100 * salary)}, 
               {'category':'Savings', 'value':(50/100 * salary)}, 
               {'category':'Survival', 'value':(40/100 * salary)}
               ] #=== This is the plan for five hundred thousand (500k) naira and above salary earners that are married

Salary_plan_A = [{'category':'Tithe', 'value':(10/100 * salary)}, 
               {'category':'Savings', 'value':(30/100 * salary)}, 
               {'category':'Survival', 'value':(60/100 * salary)}
               ] #=== This is the plan for persons that earn below five hundred thousand (500k) naira
     

if(status == 'single'):
    if(salary >= 2000000):
        for s in Salary_plan_D:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')

    elif(salary >= 1000000):
        for s in Salary_plan_C1:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')
            
    elif(salary >= 500000):
        for s in Salary_plan_B1:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')
                        
    elif(salary <= 499999):
        for s in Salary_plan_A:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')

elif(status == 'married'):
    if(salary >= 2000000):
        for s in Salary_plan_D:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')
            
    elif(salary >= 1000000):
        for s in Salary_plan_C2:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')
            
    elif(salary >= 500000):
        for s in Salary_plan_B1:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')
                        
    elif(salary <= 499999):
        for s in Salary_plan_A:
            if(s['value'] > 0):
                print(f'{s['category']} is {math.floor(s['value'])}')

else:
    pass
```
  
</p>
</details>


(jupyter nbconvert --to markdown your_notebook.ipynb)

    
