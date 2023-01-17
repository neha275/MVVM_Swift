# MVVM in Swift

***

![platform](https://img.shields.io/badge/platform-iOS-orange)
[![GitHub license](https://img.shields.io/badge/License-Apache2.0-blue.svg)](LICENSE)

MVVM stand for Model-View-ViewModel. It's a different way to arrange responsibilities, changing a few roles comapared to MVC.


 ### Why MVVM ? ### 
-  MVVM is the steps towards future of apps. MVVM allows the application to be easily maintainable.
-  MVVM allows us to break down the application in smaller components.

 ### Model ### 

- This is the layer that does not change if compared to MVC. It still represents that data-model layer of your application and can hold business logic responsibilities as well. You may also want to create a manager class to manipulate the model objects and a network manager class to handle requests and data parsing.

 ### View ### 

- This change from MVC. The view layer in MVVM involves the interface including UIView subclasses, xib and storyboard. The view logic ( animations, drawing) and handling user input events (button clicks, transitions, etc). Those are the responsibilities of the view and the controller in the MVC. This means that  your views will remain the same, while your view controller subclasses will only contain a small subset of the responsibilities they have.

 ### ViewModel ### 

- That's the new home for most of your usual controller codes. The view model layer will request the data from the modal layer ( it can be local access to the database or network layer) and pass it back to the view, formatted in the way it will be displayed. But it's a two-way mechanism: user input when necessary will also get through the view model layer to update the model. 


 ### View Model vs Model ### 
 * View Model
      * View Model is simply providing some data on which you can perform some kind of validations.
      * View Model simply provide a data to UI end taken data from UI
              
 * Model:
      * In Model class we actual implemented bussiness rules. In short the brain of the application should present in this class.
      * In Model class we generally performed the actual logic
      
 ### MVVM Flow ### 
