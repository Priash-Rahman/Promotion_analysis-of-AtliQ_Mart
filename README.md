



#  Retail sales promotion analysis.

## Dashboard Link : https://app.powerbi.com/view?r=eyJrIjoiMWU1MTNkY2MtMjJkMS00ZDk5LWI5YzktYTI2OTAxYTY0MzZlIiwidCI6Ijg2OTY0MTdiLTM1NDgtNDFjNC04NTU3LWE0ZWRjN2U4NTQ4MSIsImMiOjEwfQ%3D%3D

## Problem Statement

AtliQ Mart is a retail giant with over 50 supermarkets in the southern region of India. All their 50 stores ran a massive promotion during the Diwali 2023 and Sankranti 2024 (festive time in India) on their AtliQ branded products. Now the sales director wants to understand which promotions did well and which did not so that they can make informed decisions for their next promotional period.  

### Steps followed 

- Step 1 : Load data into Power query , dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so we need to select "column profiling based on entire dataset".
- Step 4 : Create a dimension table for promotion to normalize data & merged prom_id to fact table .
- Step 5 : Segmented promo type to 3 distinct types for understanding promo performance .
- Step 6 : Segmented base price ( Low to high) for product analysis & to understand how promo correlates with  different priced products .
- Step 7 : Added a pricing order to sort pricing type from low to high . 

           
- Step 8 :DAX measures created for comprehensive & robust analysis and to create necessary kpi's .
           
           -Revenue pre_promo / Base revenue .
           -Revenue post_promo. 
           -IR (Incremental_revenue).
           -IR % .
           -ISU (Incremental sold unit) . 
           -ISU % .
           -QTY before_promo.
           -QTY after_promo .
           -Store dynamic top (For top toggle button )
         
           -Store dynamic bottom(For bottom toggle button)
           -Product dynamic top (For top toggle button ) .
           -Product dynamic bottom (For bottom toggle button ) .
           -Dynamic_Measures(For switching between measures) .
           -Adusted cancelad booking ( for scenario analysis ).

- Step 9 : 3 report page created Store , promotion , product analysis along with KPIs

- Step 10 : A power point template/theme made  that can be leveraged for 3 reports 

 ![Screenshot 2024-05-23 215639](https://github.com/Priash-Rahman/Hotel_booking_-analysis-_Project/assets/155983828/d07f211b-d820-46ef-af6f-81d2dda87c46)

- Step 11 : Answering business questions & provide Recommendations .



## Business request 1 : Which campaign succeeded  based on promotion , ISU% , IR% ? Diwali performs very poor in ISU %  , any explanation ?


![Screenshot 2024-05-25 150114](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/2a73d5e5-7989-4271-bdd2-f6321aad1b1c)
![Screenshot 2024-05-25 140610](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/78e5a0b6-c805-4223-93b2-1407a80eac35)

![Screenshot 2024-05-30 210255](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/fc00cf78-ac7c-4c34-959c-066b6c00f6b5)
![Screenshot 2024-05-25 141927](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/d24ab2e4-cd62-4c41-973e-9e278c65e200)

-  Diwali have the upper edge when it comes to 33% & cashback promo as it generates high isu%  ; 
- Even though when it comes to promotion based on product pricing sankranti clearly has the upper edge as  low to moderate pricing product has significant growth in sankranti due to its promo offer to certain products  ! ;
- Diwali also as high IR as it offers more 50% off promo in low price section on contrary 
   sankranti offers more BOGOF promo one of the reasons for its high ISU %  ;
- Based on IR% Diwali is Successful and based on ISU% Sankranti is heavy Successful.
- Sankranti is successful when it comes to balance between IR% and ISU% .
- Some products couldn't perform discount promo in diwali   , leveraging that sankranti offers BOGOF offer  for  stock clearance oppotunity is one of the reaosons of poor ISU% of Diwali .
      

## Business request 2 : What are the top 5 products that kept balance between IR% and ISU% ?
![Screenshot 2024-05-26 203133](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/28e9ca64-4046-4af3-9b64-ff86e7bd82b3)




## Business request 3 : Which promotion is Successful & unsuccessful in both of our campaigns  ?
 
![Screenshot 2024-05-26 233432](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/f5fcef02-bbd1-47fa-9df4-3be07bb93dfc)
![Screenshot 2024-05-29 200941](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/ef8830e2-f30f-438e-8ae2-8f44f384446c)
![Screenshot 2024-05-29 201034](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/30dcadad-f5dc-4d23-a24b-2abdd5ae3148)
![Screenshot 2024-05-30 202142](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/81c1624a-148c-41e4-b0e5-9a7a57ba2d15)


- Almost 97% of Incremental revenue is generated from cashback & BOGOF promo !
 - cashback promo is Successful in Diwali campaign & BOGOF is Successful in Sankranti festivel .
 - 25% promo is a failed promo when it comes to revenue &  sold quantity !

 
 ## Business request 4 : Identify the top & failed products  after promotion  

 ![Screenshot 2024-05-29 203644](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/0df2a8d2-5f50-451c-b4c2-6b3d4b088b93)
![Screenshot 2024-05-29 205559](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/d4edaedd-7cf6-44bf-90ae-c6993fa62894)

- Failed products are associated with 25% promo  ! .

## Business request 5 : Why 25% promo failed miserably  ? Explain .
![Screenshot 2024-05-31 201158](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/3fa48518-9d9c-49b6-a72c-a9930a492085)
![Screenshot 2024-05-31 203318](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/df5deba2-74cf-44c3-b094-160d2cd623a3)




- It seems base price has an effect on 25% promo  , 25% promo fails to attract customers considering its base price .
- Like in diwali for dishwash promo offer should have shifted towards 33% or 50% ,for oil 33% seems more attractive offer & consequntly for atta & container set 33% seems more attractive .
- In sankranti base price & offer type has'een changed for some products as it is ovious for business strategy , after a remakable failure of dishwash  in diwali offering 50% or BOGOF promo could have leveraged towards increased revenue & stock clearance opportunity , 50% promo for container set could also increase sales .
-  Ultimately there may be an inbalance of base price for 25% promo offer , customer may find competitve offer elsewhere for such products .


# #Dashboard
![Screenshot 2024-05-30 215147](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/71a59f2f-6a7d-4750-878d-b43b5450b6c2)
![Screenshot 2024-05-30 215213](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/d4da65b2-4bb2-4778-bf30-3c1e353cff1b)
![Screenshot 2024-05-30 215248](https://github.com/Priash-Rahman/Promotion_analysis-of-AtliQ_Mart/assets/155983828/ab4585f8-47cb-434a-b9eb-2669dc68d762)

 #  *Recommendations*


## Reassess Promotion Strategies:

* Current Issue: The 25% discount promotion is failing due to base price imbalance and competitive market alternatives.
* Future Action: Shift some products from the 25% promo to 33% or 50% discounts, particularly for low to medium-priced items. This adjustment aligns with observed customer preferences for higher discount rates.
## Competitive Pricing Analysis:

* Current Issue: Customers may find better alternatives elsewhere, leading to lower sales under the 25% promo.
* Future Action: Conduct a thorough competitive pricing analysis before setting discount levels, ensuring that AtliQ Mart's promotions are more attractive than local market alternatives.
## Product-Specific Strategy Adjustments:

* Current Issue: Certain products (e.g., dishwashers, oils, atta, container sets) underperformed with the 25% discount.
* Future Action: Customize promotions based on product type and past performance. For instance, offer 33% or 50% discounts on dishwashers and container sets during Diwali and Sankranti to boost sales and clear inventory.
## Continuous Monitoring and Adaptation:

* Future Action: Implement a robust monitoring system to track the performance of various promotions in real-time. Use these insights to quickly adapt and optimize promotional strategies, ensuring maximum effectiveness and customer engagement.
By implementing these recommendations, AtliQ Mart can refine their promotional strategies, ensuring better alignment with customer preferences and market conditions, ultimately driving higher sales and customer satisfaction in future promotional periods.
