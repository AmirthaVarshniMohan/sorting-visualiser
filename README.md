# sorting-visualiser
An app to display the working and implementation of various sorting algorithms in data structures, such as merge sort, bubble sort, quick sort, insertion sort and heap sort using Reactjs. We randomly create lines of variable length with number of lines of our choice and sort them length wise using the sorting algorithms. The app is made with react.js with the required components.

![image](https://user-images.githubusercontent.com/105651923/228267169-3a249f9f-4320-4e2d-bf6d-24d1412fcc6e.png)
![image](https://user-images.githubusercontent.com/105651923/228267230-f7e576ff-2308-4035-95ab-963f81ec6b62.png)
![image](https://user-images.githubusercontent.com/105651923/228267289-ef79eeeb-c373-4a9a-a8d0-bba2c830f3a4.png)


FUNCTIONAL SPECIFICATION
1.	Size Slider
•	Sliders allow users to make selections from a range of values. Sliders reflect a range of values along a bar, from which users may select a single value.
•	Slider lets the user decide how many numbers of bars they need to sort.

2.	Randomize
•	Randomize is the button, that when selected would randomly rearrange the bars.
•	It rearranges the bars randomly, so the user can sort any order of the bars.

3.	Sorting Methods
•	Various sorting methods such as Bubble sort, Heap sort, Insertion Sort, Merge Sort, Quick Sort are provided for the user to select via buttons.
•	The sorting method selected by the user, will be used to sort the bars according to their lengths. 

4.	Sort
•	Sort button when clicked would sort the bars according to the sorting method selected.

5.	Notification 
•	Notification is provided when the user selects any sorting methods or any other options while the sorting is taking place such that “Sorting is taking place”.
•	When the sorting of bars has been completed, the user is notified that “Successfully sorted”.
•	When an algorithm of sorting is not selected and the user clicks the Sort button, a notification that says “Select an Algorithm!” is shown.

6.	Animation 
•	The colour of bars will be yellow when they aren’t sorted. 
•	The bar that is compared to the other bars when sorting will change colour to orange. 
•	The bars change colour from yellow to green when the sorting is completed.

TECHNICAL SPECIFICATION

COMPONENTS
Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML.
•	Two main components are used : sortingVisualizer and sortingAlgorithms
 
•	Each of the components has its own set of properties to make debugging more accessible. They help in easy re-usability of the code.
•	It is used to pass properties from parent to child for easy development.
•	SortingVisualizer component has the animation and the states for presentation, which is shown in the screen.
•	SortingAlgorithm has the implementation of the data structures which is exported to the sortingVisualizer component.
HOOKS
Hooks allow function components to have access to state and other React features.
•	UseState and UseEffect hooks are used.
•	UseState hook is used to manage the state within a component and keep track of it.
•	  
•	The useEffect Hook allows you to perform side effects in your components. Some examples of side effects are: fetching data, directly updating the DOM, and timers.
•	Here it is used to update the size of the array when changed.
STATES
•	It is an object that is used to store properties values for those attributes to a component that could change over some time.
•	Some of the states like array, type, size and started are used to set their values with their respective functions for updating changes to the states.
REACT-HOT-TOAST
•	Used for adding custom CSS for notifications that are required by the react app.
•	It notifies the state of the sorting process in the app at an instance.
ANIMATIONS
•	Animations are used for shifting the lines for the sorting process having a particular time set for the movement of lines.
•	The state of the sorting process is differentiated and shown using different colours for clear picture of the steps taking place.
