# BITSO-IOS-TEST

Created by : Manikandan

# Project Name : BitsoIos

IDE : Xcode 10.0 language : Swift 4.2

## Design Patern : MVC (Model view controller)

# API integrated : https://api.bitso.com/v3/ticker/
 
# Dependency manager : Cocoapod

Pods Used : SVProgressHUD used to display activity indicator (load view)    
Please install : pod 'SVProgressHUD' 

## Networking : URLSession

## Completed Functionalities :

# First Screen:
             * Displaying list of books available in BITSO API along with Prices in TableView
             * Displaying a loader(activity indicator) when loading data from API
             * Pull to refresh 
             
# Second Screen : 
              * Navigate to Second screen with details
              * Displaying selected Book from first screen and displays the details
              * Displaying Book Name,Last Price,Bid,Ask,Low,High,24hr volume and spread value


# Not yet Completed Functionalities :
              * Chart view
              * Autorefresh in 30 seconds and Autoscroll 


## Class and Files :

## BooksAndPriceListViewController.swift :
      In this class displaying the List of Books and Prices in TableView
      
## BookCell.swift : 
      This is a tableViewCell class and its displays Book name and Last Price, this class objects has been displayed in BooksAndPriceListViewCntroller's tableView.
      
## BookDetailViewController.swift :
      In this class displaying the selected Book's name, Last price,bid,Ask,low,high,24hr Volume and Spread .

## Book.swift :
      Its a Model class and its properties are created according to BITSO API ticker's response JSON value
      
## BitsoAPIServiceHandler.swift :
      Its a Service handler class created to access BITSP API service and response, also we are stroring the results in Books array which contails Book Model class's objects
     

     
