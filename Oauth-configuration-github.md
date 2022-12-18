- Login to github. Click on the user profile and Click the settings option.
- On the left naviation bar, Click on the developer settings and choose Oauth apps.
- Click on New oauth button to create new integration.
- Register the app by providing application name of your choice.
- Provide the home page url of your application eg: https://frontendapp.azurewebsites.net/
- Enter the description - optional
- Provide the Authorization call back url including the homepage url of your application. eg:  https://frontendapp.azurewebsites.net/.auth/login/github/callback
- Click on register the application.
- Once the app is registered, we have to generate the Client secret. Client ID will be automatically created upon registering the application.
- Click on update application button after generating the secret.

Note: 
> - If you have configured slots then create an integration only for the slot webapp, Here you have to provide the slot webapp URL instead the prod url.
  - Its not recommended to have integration for the production webapp slot.
