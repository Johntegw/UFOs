
# UFOs- Module 12 Challenge
 
Overview of Project:

Background
Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape.

What You're Creating
This new assignment consists of one technical analysis deliverable and a written report. You will submit the following deliverables:

Deliverable 1: Filter UFO sightings on multiple criteria
Deliverable 2: A written report on the UFO analysis (README.md)
Instructions
Deliverable 1: Filter UFO sightings on multiple criteria
Using JavaScript and HTML, you’ll modify the code in your index.html file to create more table filters. In addition to the date filter you created in this module, you’ll add filters for the city, state, country, and shape, as shown in the following image:

The UFO finder web page with filters for the date, city, state, country, and shape for filtering the data.
Using JavaScript, you’ll replace the handleClick() function in your app.js file with a new function that saves the element, value, and id of the filter that was changed. Then, you’ll create a new function to loop through the dataset and keep only the results that match the search criteria. The webpage will be updated with the search criteria after pressing "Enter".

Follow the instructions below and the numbered comments in the starter code to complete Deliverable 1.

Download the ufo_starterCode.js, rename it app.js, and place it in the js folder of your UFOs GitHub repository. The starter code includes the code used to populate the table from this module.

NOTE
Before you rename the ufo_starterCode.js file, we suggest that you rename the app.js you created in this module as app_1.js or something similar to avoid using the wrong file for the Challenge.

In the index.html file, remove the list element that creates the button.

Create four more list elements: city, state, country, and shape. These will be similar to the "Enter Date" list element. Each element should have the same "id" as the object properties in the data.js file.

In Step 1 of the app.js file, create an empty filters variable to keep track of all the elements that change when a search is entered. This variable will be used in Step 5 to store the property “id” and the value that was entered from user input.

Next, you will need to write code for two functions whose names we’ve provided in the starter code, updateFilters() and filterTable().

The updateFilters() function will replace your handleClick() function and update the filters variable you created in Step 1.
The filterTable() function will filter the table data by the value that is entered for the "id" that has changed.
For Step 2, located before the buildTable(tableData) function at the end of the starter code, modify the event listener from this module so that it detects a "change" on each input element and calls the updateFilters() function.

In Step 3, we’ve provided the function, updateFilters(). Inside this function, you’ll write code in Steps 4-5 to update the filters based on user input.

In Step 4a, create a variable that saves the element that was changed using d3.select(this).

In Step 4b, create a variable that saves the value of the changed element’s property.

In Step 4c, create a variable that saves the attribute of the changed element’s id.

In Step 5, write an if-else statement that checks if a value was changed by the user (variable from Step 4b). If a value was changed, add the element’s id (variable from Step 4c) as the property and the value that was changed to the filters variable you created in Step 1. If a value was not entered, then clear the element id from the filters variable.

If you’d like a hint on how to update the filters based on user input, that’s totally okay. If not, that’s great too. You can always revisit this later if you change your mind.

HINT
In Step 6, inside the updateFilters() function, call the filterTable() function that will be used in Step 7.

In the filterTable() function in Step 7, write code to filter the table based on the user input that is stored in the filters variable.

In Step 8, create a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.

In Step 9, loop through the filters object and store the data that matches the filter values in the variable created in Step 8.

In Step 10, rebuild the table with the filtered data by passing the variable created in Step 8.

Deploy the web app on your GitHub pages.

Deliverable 2: A written report on the UFO analysis (README.md)
Initialize your repository with a README, and write your analysis of Deliverable 1. For your written analysis, be sure to use complete and coherent sentences. Your written analysis should contain three sections, which cover the following:


Results: 

Based on the required new criteria that Dana wanted to provide to the users of her webpage; we developed four new search boxes that can be used.
The image below represents the updated code for users to be able to search by category. The four categories that are represented is date, city, country, and shape. 

![image](https://user-images.githubusercontent.com/119356389/226412985-5e31927d-a808-4634-b6ab-e18cb2afe547.png)


The person can easily filter on the following fields and the table will sort accordingly. 

this one you can enter the date you are looking for: 
![image](https://user-images.githubusercontent.com/119356389/226413310-1f2e807b-9aaf-4e1e-839c-ba96a7d65292.png)


 The image below is a filter by city: 
![image](https://user-images.githubusercontent.com/119356389/226399796-74d20283-61d9-4c2e-b6ad-7441b7718613.png)

You can also filter by State just by entering the states abbreviations:
![image](https://user-images.githubusercontent.com/119356389/226399684-68a1aaff-c51e-461d-8c0f-0b020de3fa91.png)

 The image below is a filter by country: 

![image](https://user-images.githubusercontent.com/119356389/226399913-4e116bc8-75e5-497b-aecc-2331bdb1fff8.png)
 and or you can filter by shape:
![image](https://user-images.githubusercontent.com/119356389/226400092-ea83f4e5-4c65-416b-8097-42d57f3704f8.png)


Summary:

 This table is a dynamic table. It responds according to your choices entered in the filter. What I see as an issue is the ability to clear the fields when done entering in each filter. I had to zero out each section. This is one area I would change. Also I didn't see the clear function  as something that would be used when clearing the page. 
 
 Other than the  above issue, I find that this page is very informative and intresting. 
