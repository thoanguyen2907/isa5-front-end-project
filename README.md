# Frontend React Project

This is your final project for the frontend module combine with react + redux toolkit + typescript

## Instructions

### General

Fork this repo, then clone the **fork** to your machine and start working on it. You can open a pull request as soon as possible (no need to wait until finished)
For styling, you can use whatever css solution you want: css, bootstrap, Material UI, etc.
You need to install the css library yourself.
Checkout the separate branch when you finish each step. 

### Step 1
Write the codes in typescript

Write the first custom hook, that:

- Fetch all the countries and return the data
- Example usage of the hook is like this:

```
// countries variable will be an array of 250 countries
const [error, countries, loading] = useCountries()
```

Write the second custom hook, that:

- Given a country name as argument (international or native), returns the data about that country from [countries APIs](https://restcountries.com/).
- Example usage of the hook is like this:

```
// country variable is an object, with details about Suomi (Finland)
const [error, country, loading] = useCountry('Suomi')
```

### Step 2

- Use the first custom hook you created to fetch all the countries data
- Render this data in a table, you can use html table tag, or component library like Material UI
- Include loading while waiting to fetch data and error in case something is wrong


### Step 3

- Integrate react router into your project and create 2 pages: `home`, and `country`
- Homepage will contain the countries table that we created above
- Country page will render the data about one specific country only
- When a user click on the name of the country in the table, they will be routed to the `country` page

### Step 4

- Set up all the redux toolkit folders for the project
- Think about what reducer and the elemements in the reducer
- Apply redux toolkit to call API 
- Move the state that contains all countries to redux store


### Step 5

Take your time to implement the following features:

- Implement a search bar to search for a country
- Add/remove the countries to/from favorite list
- Sort the table based on name, region, etc.
- Maker sure the  favorite list is saved in local storage to persist across refreshes of the page 

## References

[Demo](https://flagify.netlify.app/)

