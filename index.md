## Project description


>Budget manager is a webservice accessed by a custom Android app that helps individuals manage and
track their spending on a daily 
or monthly basis. 
Users will assign their expenditures in different categories (by assigning a name to each budget to 
create those different categories) for monthly bills and expenses such as
gas, groceries, dining out, miscellaneous, personal spending, savings, and any other categories of 
their choosing for any duration of time, recurring or not. 
Personal savings goals can also be created to establish better spending habits.
The user will enter all transactions on a daily basis. 
The due dates and any extra notes can be created for each bill for organizational purposes. 

>The webservice will support the functionalities of persistent storage, tracking of transactions 
>versus budget and will take care of the automatic computation of transactions into budget.

>To access the app the user must log in to his Google account and will be directed to the home 
screen. This screen will display buttons directing you to three different fields: 
  * budgets
  * transactions
  * saving goals
>In _budget_ the user will see a dropdown menu with the predefined categories, and an option to
create his own budget. 
If _transactions_ is selected the user will be prompted to enter either positive or negative 
transactions to record their spending habits.
When accessing _saving goals_ the user will have a detailed overview of his current progress.


## Intended Users & user stories


   * **A single mom**
        > As a single mom with two toddlers, I need to fit daycare and children's expenses 
          in my monthly budget to make sure our needs are met until the end of the month.
    
   * **A graduate, starting his first job and who wants to live on his own**
        > As a recent grad, I just landed my first job and, I need to learn how to manage my 
          spending and save money for a down payment, so I can buy a house in two years.
        
   * **A foreigner who just moved to the US**
        > As a new arrival in the United States, I need to learn how to compare my expenditures to
          my budget, so I can pay my bills and still send my family $200 each month.
                                                  

## External services/sources
   * [Google sign in](https://developers.google.com/identity/sign-in/android/start-integrating)
   >We will use Google sign in to the Android app and have the token passed on the web service for
   authentication. 
 

## [Entity Relationship Diagram](docs/erd.md)

## [Entity classes](https://github.com/budget-manager/budget-manager-server/tree/master/src/main/java/edu/cnm/deepdive/budgetmanagerservice/model/entity)

## Team roster

* Mercedes 
* Jan
* Jeremy

## Stretch goals

   * progress notifications
   * banking API
   * access to camera to track and store receipts 
   * group based budgeting
   
   

