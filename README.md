# Historical Weather Data Sheets :sunny: :umbrella: :cloud: 

This service retrieves historical weather data for a submitted city and exports the data as a new sheet into a Google Spreadsheet. Each row in the new sheet represents a day and the columns are data that can help visualize weather trends. Uses Weatherbit Historical Weather API to get weather data and Google Sheet API to edit the spreadsheet.

A FrontEnd Javascript application built using [React](https://reactjs.org/). This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## To Run Project Locally

### Prerequisites
In order to run this project locally, you should have the following installed:

- [NPM](https://www.npmjs.com/)

You should also:
  1) Set up a Google Sheets API:
    Register a new app and enable “Google Sheets API” [Google Developers Console](https://console.developers.google.com). Head over to    “Credentials” and click the “Create credentials” button and select “API Key”. Click the “Restrict Key” and set a name for it. Under      “Application Restrictions” set it to “HTTP referrers” and add http://localhost:3000 for now. Under “API Restrictions” select the            “Google Sheets API” and save. <b>Make a note of the API key.</b>
      
*Since the application is modifying a spreadsheet, the request must be authorized by an authenticated user who has access to that data.*
  2) Obtain OAuth 2.0 credentials from the Google API Console: Click Create credentials > OAuth client ID. Set the application type to Web application. Add http://localhost:3000 as an Authorized Javascript origins. <b>Make a note of the Client ID.</b>
      
  3) Signup for a Weatherbit API key (https://www.weatherbit.io/api). <b>Make a note of the API key.</b>


### Installation & Startup
1) Fork this repo
2) Clone the fork
3) Install Dependencies: `$ npm install`
4) Add a .env.development.local file to your project's root directory and set REACT_APP_WEATHERBIT_APIKEY to your weatherbit API key
      ``` JavaScript 
      REACT_APP_WEATHERBIT_APIKEY=<your_weatherbit_api_key>
      ```

    <kbd>
    <img src=""> 
    </kbd>

5) You wil also need your Google API Key and Client ID in the .env.development.local file and name them REACT_APP_GOOGLE_APIKEY and
REACT_APP_GOOGLE_CLIENTID, respectively
      ``` JavaScript 
        REACT_APP_GOOGLE_APIKEY=<your_google__api_key>
        REACT_APP_GOOGLE_CLIENTID=<your_google_client_id>
      ```
      <kbd>
      <img src=""> 
      </kbd>

6) Start the Development Server: `$ npm start`
7) Visit http://localhost:3000/

Enjoy! :blue_heart:
