# Overview of Project: 
## Background
Dana’s webpage and dynamic table are working as intended, but she wanted us to provide a more in-depth analysis of UFO sightings. She wanted the users to have the freedom to filter based on multiple criteria at the same time. Apart from the existing date filter, we added additional filters for the city, state, country, and shape.

## Purpose 
To create a web page and dynamic table so that users can filter the data not just on the date criteria but also on the city, state, country, and shape. 
# Results: 
We added additional filters and created a loop using a conditional if else statement. These filters are based on the id mentioned for example if the user wishes to view the UFO sightings based on the city, they can do so. If they don’t set a filter, then the entire table can be viewed. 

<img width="1439" alt="Website_info" src="https://user-images.githubusercontent.com/111670866/202312856-ff51b005-f079-46cd-918c-079520a6a7e2.png">


```
// 4a. Save the element that was changed as a variable.
let changedElement = d3.select(this);

// 4b. Save the value that was changed as a variable.
let elementValue= changedElement.property("value");
console.log(elementValue);

// 4c. Save the id of the filter that was changed as a variable.
let filterId= changedElement.attr("id");
console.log(filterId);

// 5. If a filter value was entered then add that filterId and value
// to the filters list. Otherwise, clear that filter from the filters object.
if (elementValue) {
  filters[filterId] =elementValue;
  }
else {
  delete filters[filterId];
  }
  
```
<<<<<<< HEAD
=======
<img width="1409" alt="Without_filters" src="https://user-images.githubusercontent.com/111670866/202312432-4258f33a-31c8-40a5-83cb-d06a4fd2db57.png">
>>>>>>> refs/remotes/origin/main

/Users/Rochelle/Desktop/JavaScript_Bootstrap_UFOs/UFOs/static/css/images/Without_filters.png

The above image is without any filters. The user can view the entire table since they haven’t put any search criteria. 

<img width="1409" alt="With_filters" src="https://user-images.githubusercontent.com/111670866/202312479-168d763a-3f2f-4c01-9c43-6ba421fe1de2.png">


This image is with two filters in place, the shape is set to circle and the city is set to mason. There is one entry corresponding to these filter criteria. 

# Summary: 
To conclude, this is quite an improvement over the previous design. Earlier the user could filter the UFO sightings based on the date filter only. Now we’ve added additional filters giving the user the opportunity to be more specific and narrow their search down. 
However, this system has a potential drawback, in that the user must be accurate with the spellings. If they type in the wrong spelling or even the wrong case is used the search doesn’t yield any results. In the below image, the name of the city is typed in Sentence case (Benton) in the search bar and it hasn't brought up any entry. When the city name is typed in in lowercase (benton), we get one entry. 

<img width="1409" alt="Filter_Sentencecase" src="https://user-images.githubusercontent.com/111670866/202312570-99c8bb52-7393-471d-af0e-fb32613dd1a2.png">

 <img width="1409" alt="Filter_lowercase" src="https://user-images.githubusercontent.com/111670866/202312576-4f370298-8975-43a2-aebe-cd7465cf1d0e.png">


# Recommendations:
### 1)The website could include images/video clips along with comments to make a more powerful impact on the users.
### 2)A Call to action, meaning what is the top action that Dana wants of the users. If she wants to create an ongoing connection with the website users, then an email sign-up box could be inserted. 
### 3)A contact button could be included on the webpage. This will give users some contact information in case they wish to connect with Dana or her team members. 

