# **Drover FE Assignment - Search Page**

Hello!

Drover is a vehicle rental marketplace where drivers can rent a vehicle from an owner, Drover facilitates these rentals.

As we are a marketplace we need a way for drivers to search what vehicles are available and filter them somehow.

### Your task will be to build our *Search Page*!

The page can be found at https://www.joindrover.com/cars/search and there are 2 versions of it (Consumer, Private-Hire) with very small differences between the two.

----

## What do we expect from you?

Using https://github.com/facebook/create-react-app as a boilerplate (or any other you might prefer) try and get as much done as possible.

We know people have different amounts of time to do this test so we have broken it down into sections based on amount of time you have. Please try and do as much as possible but if you only have time for one section we understand, of course, the more you do the better an idea we have of your skills.
 
 
#### 1. Basic

- Setup an app that calls our API to get vehicles for one user type
- Display vehicles in a list/table to the user with relevant data
- Allow at least 1 field in search to be user inputted (details below)

*Bonus:* add some styling

#### 2. Keep going

- Add all fields able to search by for one user type (details below)
- Write unit/snapshot tests for most if not all components
- Add styling to make it look like https://www.joindrover.com/cars/search


#### 3. All out!

- Search can search for both types of vehicles (Consumer & Private-Hire)
- Styling as close to original as possible
- Fully responsive

*Bonus:* add google autocomplete to the location in the search filters



## API info

API basic documentation here: 
https://app.joindrover.com/api/web/docs/1.0/vehicles/index.html

**Example request:**
```
curl --request POST \
  --url https://app.joindrover.com/api/web/vehicles \
  --header 'content-type: application/json' \
  --data '{
	"location": "London, Uk",
	"max_distance": 50,
	"number_of_months": 12,
	"number_of_weeks": 52,
	"order_by": "price",
	"order_direction": "asc",
	"page": 1,
	"per_page": 15,
	"price_max": 2500,
	"price_min" :100,
	"rolling": false,
	"start_date": "09/05/2018",
	"vehicle_type":"Consumer"	
}'
```
**Some things to note about the endpoint:**

start_date = 'dd/mm/yyyy'

vehicle_type = 'Consumer' or 'PCO'

------

## Notes

Build good and reusable code and think about components not just one-off rushed building if you can.

Use a FE library if you want. (We use http://getbootstrap.com 4)

** Please push the repo to your GitHub account and share the link with us, DO NOT create a fork **
