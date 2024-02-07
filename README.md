# Urban Lunch

**Project Overview:**

Urban Lunch is an application designed to customize business lunches by consolidating orders from various eateries within the city. The inspiration behind creating this app stems from the fact that individuals have diverse culinary preferences, whereas most restaurants typically specialize in only one type of cuisine. Consequently, business lunches ordered from such establishments may lack the desired variety.

The app addresses this issue by providing a diverse selection of foods in a single business lunch. You have the flexibility to combine all different kinds of dishes with just a few clicks. The entire order can then be conveniently collected from a restaurant of your choosing.

My primary responsibility involved conducting manual testing of the application's features related to the core user process of placing food orders and monitoring delivery. This testing was carried out within Android Studio, using a Google Pixel 5 emulator with API version 31.

**Your Role and Contributions:**

In this position, I conducted quality assurance for the key functionalities of the application integral to the primary user journey, which involves selecting a pick-up point, placing a food order, and overseeing the eventual delivery.

My duties encompassed the following:
- Examining the designated layouts in Figma and aligning them with the requirements against the current layout of the mobile app.
- Developing a testing checklist derived from the specified requirements for thorough examination.
- Executing tests on the requirements by leveraging the Pixel 5 emulator within Android Studio.

**Project Deliverables:**

I generated a testing checklist that not only comprises the test cases and their respective statuses but also integrates links to bug reports on JIRA and provides a succinct overview of the count of both passed and failed test cases. The checklist can be found [here](https://docs.google.com/spreadsheets/d/10EoGeT7xNjJdwcYxs9e8QoyDQR0NROXI8uhdMttXlZ0/edit?usp=sharing).

**Testing Approach:**

The testing primarily involved manual smoke testing activities, wherein test conditions were extrapolated from the requirements, encompassing both positive and negative testing scenarios. Additionally, manual testing of the user interface was performed.

Given that this marks the first version of the application, ensuring the thorough testing of fundamental features is of paramount importance.

**List of Tests Conducted:**

The following tests were done:

_Selecting a pick-up location_		
- The map shows the order of pickup points
- None of the pick-up points are selected by default
- When you tap on a pick-up point, it's highlighted and considered selected
- A repeated tap on a pick-up point cancels the selection
- Tapping on a pick-up point when another pick-up point is selected changes the selection to the new pick-up point
- The drop-down list contains a list of restaurants from which the customer can pick up their lunch
- When you select an item from the drop-down list, it's selected on the map and considered selected

_Choosing dishes_
- The dishes are displayed as a list in the "choice of dishes" screen
- Each item on the list in the "choice of dishes" screen contains the name of the dish, the -/+ buttons, and an arrow
- Tapping in any area of the list in a dish's corresponding region in the "choice of dishes" screen except + takes you to the "dish details" screen
- When you click + on the order dishes screen, the dish is added to the order list from the nearest restaurant to the pick-up point
- There is a "Next" button in the footer
- The "Next" button is inactive if there are no dishes in the order list
- To the left of the name of the dish in the dish details screen is a return arrow
- The arrow in the dish details screen takes the user back to the dish list when pressed
- By tapping on the restaurant name (igiven below the dish ingredients) in the dish details screen, the dish is added to the order list

_Confirming order_
- If the list of orders is too long in the order confirmation screen, you can scroll through it
- The total amount contains the price of all prepared dishes and delivery in the order confirmation screen
- A tap on the "Order" button in the order confirmation screen takes the user to the order tracking screen

_Order tracking_
- The map on the order tracking screen shows the pick-up point from which you can pick up your order
- The map on the order tracking screen shows the restaurants where the dishes are prepared
- The map on the order tracking screen shows the routes from the restaurants to the pick-up point
- The order screen shows the cost of all dishes ordered at the restaurant
- The order screen shows the remaining cooking time from the restaurant to the pick-up point
- The order screen shows the remaining delivery time from the restaurant to the pick-up point
- If there are many items on the list in the order tracking screen, and they do not fit on the screen, the list is scrollable

_Order being delivered_
- Switching to the "Order is delivered" screen is automatic when the timer expires
- The map in the "order is delivered" screen shows the point on the map where the desired pick-up point is located
- After clicking on the "I got the order" button in the "order is delivered" screen, the order is considered completed
- After the order is considered completed, the user is shown a feedback bar
- After the user answers with feedback, they are taken back to the beginning, where they can select a pick-up point for a new order

_Error notifications_
- If you don't allow the app to access geolocation, an error message appears
- If you try to order without adding any dishes, an error message appears

_Data integrity_
- The dishes and their restaurants match according to the price of dishes table in requirements
- The dishes and their prices match according to the price of dishes table in requirements

_User interface_
- The UI of the "selecting a pick-up point" screen matches the requirements
- The UI of the "choice of dishes" screen matches the requirements
- The UI of the "dish details" screen matches the requirements
- The UI of the "order confirmation" screen matches the requirements
- The UI of the "order tracking" screen matches the requirements
- The UI of the "order delivery" screen matches the requirements

**Test Results:**

Out of 41 test cases, 33 has passed while 8 has failed.

The following tests conducted have failed:
- The map shows the order of pickup points
- The total amount contains the price of all prepared dishes and delivery in the order confirmation screen
- The order screen shows the remaining cooking time from the restaurant to the pick-up point
- The dishes and their prices match according to the price of dishes table in requirements
- The UI of the "choice of dishes" screen matches the requirements
- The UI of the "dish details" screen matches the requirements
- The UI of the "order tracking" screen matches the requirements
- The UI of the "order delivery" screen matches the requirements

**Challenges Faced:**

During my initial attempt, I inadvertently overlooked testing two requirements. I appreciate my reviewer for bringing this to my attention. This experience has underscored the importance of cross-checking and being more diligent in ensuring all requirements are thoroughly examined.

**Results and Outcomes:**

From the 41 test cases, 33 had passed while 8 had failed. Respective bug reports have been filed. The bugs are now ready to be fixed and hopefully confirmation tested.

**Key Takeaways:**

In the course of this project, I have refined my skills in the following areas:
- Grasping the essentials of mobile app testing
- Employing Android Studio as a testing tool
- Gaining proficiency in obtaining error logs for developers

**Conclusion:**

The project facilitated the acquisition of proficiency in mobile testing.

I extend my gratitude to Ivan Pavlov for correcting and enhancing my work.
