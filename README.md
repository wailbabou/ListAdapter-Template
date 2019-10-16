# ListAdapter-Template
ListAdapter template for Android studio : Kotlin

## Adding to Android Studio
File -> Settings -> Editor -> File and Code Template -> Add

## Usage
  <img src="https://github.com/wailbabou/ListAdapter-Template/blob/master/Screen%20Shot%202019-10-16%20at%201.47.31%20PM.png" width="70%" />

An Example : 

 <img src="https://github.com/wailbabou/ListAdapter-Template/blob/master/Screen%20Shot%202019-10-16%20at%201.50.33%20PM.png" width="70%" />
 
 There is :
 - File name
 - Listener name
 - Model name
 - View Holder Header name
 - View Holder name
 - View Holder Item Binding name
 - View Holder Header Item Binding name
 
 
 In the example above we need 
 
 - item_test.xml 
 ```xml
 <layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <variable
            name="item"
            type="bellal.ouail.project.models.Test" />
        <variable
            name="clickListener"
            type="bellal.ouail.project.adapters.TestAdapter.TestListener" />
    </data>

    <!-- your view here -->
</layout>
 ```
 
 - item_header.xml
 ```xml
 <layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <variable
            name="clickListener"
            type="bellal.ouail.project.adapters.TestAdapter.TestListener" />
    </data>

    <!-- your view here -->
</layout>
 ```
 
 ## TO DO
 - Bind data to the itemview in the bind function of the ViewHolder.
 - Define the areItemsTheSame and areContentsTheSame functions.
 - Override id inside sealed class DataItem
