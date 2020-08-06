## Project Overview

### Team roster

* Mercedes Garcia ([GitHub](https://github.com/Merced-es) & [LinkedIn](https://www.linkedin.com/in/mercedes-garcia-961403139/))
        -> worked on the client side of the app, created the fragments and organized the navigation 
           between them, fine-tuned the adapters and repositories
* Jan Gevaert ([GitHub](https://github.com/jangevaert-design) & [LinkedIn](https://www.linkedin.com/in/jan-b-gevaert/) )
        -> got the security in on the client- and the server side; took care of the documentation.
* Jeremy Brown ([GitHub](https://github.com/jeremybrown505) & [LinkedIn](https://www.linkedin.com/in/jeremy505/))
        -> created and worked in detail on the user interfaces

### Project introduction & description

#### General overview and intended functionality

>Budget Manager is a webservice accessed by a custom Android app that helps individuals manage and
track their spending on a daily or monthly basis.

>Users will assign their expenditures in different categories (by assigning a name to each budget to 
create those different categories) for monthly bills and expenses such as
gas, groceries, dining out, miscellaneous, personal spending, savings, and any other category of 
their choosing for any duration of time, recurring or not. 
Personal saving goals can also be created to establish better spending habits.
The user will enter all transactions on a daily basis. 
The due dates and any extra notes can be created for each bill for organizational purposes. 

#### Motivation for the development of this type of app

>Since there is a need for many of us to be able to check, update and follow our spending habits, 
>Budget Manager is the right app to assist you in this. This application, which you always have at 
>hand is designed in a way to make your updates easy and gives you the chance to check your savings 
>and budget goals on the go and in real time. 
>Since all fields are easy to customize this app can be adapted to the wishes of each
>user. Budget Manager has all the tools in house to make the user's life more comfortable and his 
>expenses easier to control.

#### Key functional elements of the application

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
When accessing _saving goals_ the user will have a detailed overview of his current status and 
>progress.


### [Budget Manager PDF overview](docs/pdf/budget-manager-android-app.pdf)

### Summary of current state of the project

#### Description of the current state

#### List of aesthetic improvements

#### List of functional stretch goals
   * progress notifications
   * banking API
   * access to camera to track and store receipts 
   * group based budgeting
   
## Functional documentation

### Intended Users & user stories

   * **A single mom**
        > As a single mom with two toddlers, I need to fit daycare and children's expenses 
          in my monthly budget to make sure our needs are met until the end of the month.
    
   * **A graduate, starting his first job and who wants to live on his own**
        > As a recent grad, I just landed my first job and, I need to learn how to manage my 
          spending and save money for a down payment, so I can buy a house in two years.
        
   * **A foreigner who just moved to the US**
        > As a new arrival in the United States, I need to learn how to compare my expenditures to
          my budget, so I can pay my bills and still send my family $200 each month.
                                                  
### [Wireframe](docs/wireframe.md)

### Basic user instructions

Once the system is running, the app will open on the Google Signin page. After signing in you will
arrive on the home screen that will guide you to either the budget screen or to the screen where
you can create a transaction.
In the budget fragment you can view a list of your budgets and/or create a new budget. When clicking
on a specific budget you will be directed to the transaction fragment which displays a list of 
transactions within that budget.
When you click on 'create transaction' from the home screen you will have the possibility to create 
a new transaction.

## Technical documentation

### [Entity Relationship Diagram](docs/erd.md)

### [Data Definition Language](docs/ddl.md)

### [Outline of technology stack](docs/technology-stack.md)

### [Javadoc documentation](https://github.com/budget-manager/budget-manager-server/tree/master/docs/javadocs)

### [REST service endpoint documentation](https://github.com/budget-manager/budget-manager-server/tree/master/src/main/java/edu/cnm/deepdive/budgetmanagerservice/controller)

### Build instructions

>Clone the repository for the app [here](https://github.com/budget-manager/budget-manager-android) 
and for the server side project [here](https://github.com/budget-manager/budget-manager-server)                                                                                         
Paste the cloned repository into "get from Version Control" on IntelliJ.
Run the server side project so that a connection with the end points can be established. Start up 
the application and enter data in the pop up screens and use the save button to check that the data
are sent and stored on the server side.


## [License notice](docs/notice.md)

Copyright 2020 Mercedes Garcia, Jeremy Brown & Jan Gevaert

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

> <http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.







<!---## External services/sources
   * [Google sign in](https://developers.google.com/identity/sign-in/android/start-integrating)
   >We will use Google sign in to the Android app and have the token passed on the web service for
   authentication. 

## [Entity classes](https://github.com/budget-manager/budget-manager-server/tree/master/src/main/java/edu/cnm/deepdive/budgetmanagerservice/model/entity)



## [Repositories](https://github.com/budget-manager/budget-manager-server/tree/master/src/main/java/edu/cnm/deepdive/budgetmanagerservice/service)

## [REST controllers and application logic services](https://github.com/budget-manager/budget-manager-server/tree/master/src/main/java/edu/cnm/deepdive/budgetmanagerservice/controller)
   
   

