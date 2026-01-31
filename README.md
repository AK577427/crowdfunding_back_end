## `README.md` Template Phase 1: API Plan

As your Crowdfunding back end grows, you'll have more and more information to put in the `readme.md` file. For now, you have a rough plan for your project, so let's mark it down!

Below is a template you can use to add your plan to your readme. As usual, {{ double brackets }} indicate places where you should insert your own content. So if your name was Sinead O'Connor, you would swap `Hi, my name is Anu'

If you're looking for a good way to create your Schema diagram in VS Code, check out [the draw.io integration extension for VS Code](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)!

To make editing tables in Markdown easier, you might enjoy [the Markdown All-In-One extension](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one). With this installed, you can hit tab inside of any "cell" in a table, and the editor will automatically resize all your columns and create a new row if necessary.

```markdown
# Crowdfunding Back End
CountOnMe - Support a cause. Make it count.

## Planning:
### Concept/Name
CountOnMe is a full-stack crowdfunding platform designed to connect people with causes, projects, and ideas they care about. It provides a space where users can create fundraisers and where supporters can pledge their help, making it easy to turn small contributions into meaningful impact.

This project was built using **Django REST Framework** for the backend API and **React** for the frontend.

### Intended Audience/User Stories
{{ Who are your intended audience? How will they use the website? }}
    As a user, I want to create a login
    As a user, I want to create a fundraiser with log in 
    As a user, I want to update a fundraiser
    As a user, I want to see the list of all fundraisers + resp pledges

    As a supporter, I want to pledge to a fundraiser without logging in
    As a supporter, I want to see the list of all fundraisers + resp pledges

### Front End Pages/Functionality
- Home page
    - List of Fundraisers
    - Click to view Fundraiser details
    - Make a Pledge
    - Login/Register
- Fundraiser Page
    - Fundraiser details
    - All the pledges made for that fundraiser
    - Create a Fundraiser
    - Make a pledge
- Login/Register
    - Register - if a user is new
    - Login - if the user is already registered

### API Spec
{{ Fill out the table below to define your endpoints. An example of what this might look like is shown at the bottom of the page. 

It might look messy here in the PDF, but once it's rendered it looks very neat! 

It can be helpful to keep the markdown preview open in VS Code so that you can see what you're typing more easily. }}

| URL             | HTTP Method | Purpose                     | Request Body        | Success Response Code | Authentication/Authorisation |
| --------------- |------------ | --------------------------- | ------------------- | --------------------- | ---------------------------- |
| /fundraisers/   |GET          |Get all fundraisers          |N/A                  |200                    |None                          |
| /fundraisers/1/ |GET          |Get fundraiser with pledges  |Fundraiser object    |200                    |None                          |
| /fundraisers/   |POST         |Create a new fundraiser      |N/A                  |201                    |Logged In                     |
| /pledges/       |GET          |Get all pledges              |N/A                  |200                    |None                          |
| /pledges/       |POST         |Create a new pledge          |Pledge object        |201                    |None                          |
| /users/         |GET          |Get all users                |N/A                  |200                    |None                          |
| /users/1        |GET          |Get an user                  |N/A                  |200                    |None                          |
| /users/         |POST         |Create a new user            |User object          |201                    |Logged In                     |


### DB Schema
![]( {{ ./relative/path/to/your/schema/image.png }} )
```
