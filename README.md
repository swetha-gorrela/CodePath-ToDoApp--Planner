# CodePath-ToDoApp--Planner
This is the basic version of ToDo list android app developed for codepath bootcamp application
# Pre-work - Plannner

Planner is an android app that allows building a todo list and basic todo items management functionality including adding new items, editing and deleting an existing item.

Submitted by: **Swetha Gorrela**

Time spent: **3.5** hours spent in total

## User Stories

The following **required** functionality is completed:

* [Yes] User can **successfully add and remove items** from the todo list
* [Yes] User can **tap a todo item in the list and bring up an edit screen for the todo item** and then have any changes to the text reflected in the todo list.
* [Yes] User can **persist todo items** and retrieve them properly on app restart

The following **optional** features are implemented:

* [ ] Persist the todo items [into SQLite](http://guides.codepath.com/android/Persisting-Data-to-the-Device#sqlite) instead of a text file
* [ ] Improve style of the todo items in the list [using a custom adapter](http://guides.codepath.com/android/Using-an-ArrayAdapter-with-ListView)
* [ ] Add support for completion due dates for todo items (and display within listview item)
* [ ] Use a [DialogFragment](http://guides.codepath.com/android/Using-DialogFragment) instead of new Activity for editing items
* [ ] Add support for selecting the priority of each todo item (and display in listview item)
* [ ] Tweak the style improving the UI / UX, play with colors, images or backgrounds

The following **additional** features are implemented:

* [ ] List anything else that you can get done to improve the app functionality!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
http://imgur.com/5mDmwX4
<img src='http://imgur.com/5mDmwX4.gif' title='Video Walkthrough' width='600' alt='Video Walkthrough' />

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Project Analysis

As part of your pre-work submission, please reflect on the app and answer the following questions below:

**Question 1:** "What are your reactions to the Android app development platform so far? Compare and contrast Android's approach to layouts and user interfaces in past platforms you've used."

**Answer:** I have woked on web appliction so far. Based on my previous expereince I feel android app development is similar to web development.Having good knowlegede of web pages and javascript is ery helpful in understanding android development 
Layouts in Android sudio are similar to web pages. The design tab/xml can be compared to HTML wih CSS.It also has similarity in terms of onClick method which is siilar to javascript onClick() method dfined in HTML. Alert in javascript is similar to Toast in Android.


**Question 2:** "Take a moment to reflect on the `ArrayAdapter` used in your pre-work. How would you describe an adapter in this context and what is its function in Android? Why do you think the adapter is important? Explain the purpose of the `convertView` in the `getView` method of the `ArrayAdapter`."

**Answer:** 
Adaper Defition:An Adapter object acts as a bridge between an AdapterView and the underlying data for that view.
In the ToDO app, ArrayAdapter is used to dispaly an array of items. It is used to display toDo items in a listview. It takes the each element in the array and tansform into the android compatible format so as to display it on the layout. 
Why is adaper important: If there is not adapter, then each of the todo item should be placed in a text view. When the number if items are more, then scroll functionality should be imlemented. And for each click event on the item, there should be a code for that functionality. For persistence, all these text view items should be taken and converted to array while storing in a file or database. This would increase the complexity of the program and might result in some errors. So an ArrayAdapter makes it easy to conver array view to adnroid compatible views
'convertView' in 'getView' is used to reuse a view. In this case, when there are more toDo items which cannot be fit into one screen, then scrolling functionality is used. In that scenario, an ArrayAdapter creates a view with the number of items that can be displayed on the screen. Once user scrolls down, then the adapter should load the next list of items/objects to be displayed. To do so, they should be loaded into a view. Insitead of creating a new view for every scrol, convertview is sed to re-use the intially created view to display the next set of toDo items from the array.

## Notes

Describe any challenges encountered while building the app.

## License

    Copyright [2017] [swetha gorrela]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
