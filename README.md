## Weather App made for internship task at DigitalPaani

### Description

- Weather application which lists a set of cities in the world
- Selected city should maintain stickiness across the browser sessions
- App should be responsive with the cards being stacked on portrait mode and placed horizontally when in landscape mode

### High Level Design:

- API for the weather information was provided by Open Weather Map this provides forecast details.


### Detailed Design:

- Built the app using react functional components with hooks to handle state and other life cycle methods
- App component acts as the core parent component of application, it takes care of loading the initial state, data communication and also handles how the data gets propagated to various underlying components
- Initial state of the application is set by looking up the browser storage for any pre-selected city for which the forecast can be fetched
- Every successful forecast is then updated back to the storage so that the subsequent visits would be handled accordingly
- Error handling is in place to address various scenarios like weather information for a given city is not available, or if no selection has been made et cetera.
- Kept the layout of the application simple to have any modification or enhancement in future to evolve the layout as required

### Front End Implementation:
- React

### API Details:

https://api.openweathermap.org/data/2.5/weather?q={city name}&appid={API key}

### Application Link:

Link to the Application hosted on Vercel [weather-app-digitalpaani-frontend-task.vercel.app](https://weather-app-digitalpaani-frontend-task.vercel.app/)

### How to Run the Application:

Clone the repo and setup the application

```shell
# clone the git repo
git clone repolink

cd foldername
npm install
npm start

```

### Advanced Features (To be built):

- Advanced search for cities
- Geo Location API integration
- Celsius to Fahrenheit Conversion
