# Akshitha's Contribution

## Widget Tree and Lifecycle Notes

I reviewed the widget tree and controller lifecycle of our In-Class 01b Flutter application. The app uses a TabController to keep the TabBar and TabBarView synchronized.

One important concept I reviewed was the lifecycle of the TabController. It is initialized in initState() so that it is created once when the state object is initialized. It is then cleaned up using dispose() when the widget is removed. This prevents unnecessary resources, such as the controller's ticker, from remaining active.

I also reviewed the idea of using the tabs list as a single source of truth. Using tabs.length instead of repeating the number of tabs in multiple places makes the application easier to maintain and reduces the chance of mismatches between the TabBar and TabBarView.
