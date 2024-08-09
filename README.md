# TaskMagic Automation Cheat Sheet

## 1. Trigger

- **What it Means (ELI5):** A trigger is like an alarm clock that starts your automation when a specific event happens.
  
- **When to Use It:** Use a trigger when you want your automation to start automatically based on certain conditions (e.g., a new email arrives, a specific time of day).
  
- **How to Use It:** Set up a trigger by selecting a condition like a scheduled time, a change in a Google Sheet, or an action in another app.

- **Use Cases:**
  - Starting a data scrape every day at 9 AM.
  - Triggering an automation when a new row is added to a Google Sheet.

- **Examples:**
  - **Google Sheets Trigger:** Set up to start when a new row is added to the sheet.
  - **Time-Based Trigger:** Schedule an automation to run every morning at 8 AM.

## 2. Pause/Delay

- **What it Means (ELI5):** A pause is like taking a short break before doing the next task.
  
- **When to Use It:** Use a pause when you need to wait for something to load or to give the system time to process before moving to the next step.

- **How to Use It:** Add a delay step and specify the duration of the pause in seconds.

- **Use Cases:**
  - Waiting for a webpage to load fully before scraping data.
  - Pausing between sending emails to avoid being flagged as spam.

- **Examples:**
  - **Delay Step:** Add a 5-second delay to ensure the next page loads completely.

  - *Thanks to Paul Parry for the below correction:*
    - One small error. Pause and Delay are different; you have then grouped and discussed as the same item.
    - Delay with the value set to say 0.1 mins delays for 6 seconds before carrying on with the automation.
    - Pause stops the automation until you press the play button in the control center.
    - The latter is useful for desktop scenarios, where you need to do something else you have not included in the automation.

## 3. Scrape

- **What it Means (ELI5):** Scrape is like using a spoon to scoop up information from a webpage.
  
- **When to Use It:** Use scraping to collect data from websites automatically.
  
- **How to Use It:** Select "Scrape Text" for single data points or "Scrape List" for multiple items.

- **Use Cases:**
  - Collecting a list of product names and prices from an e-commerce site.
  - Gathering user information from a social media platform.

- **Examples:**
  - **Scrape List:** Select two usernames in a row on a webpage to scrape the entire list.
  - **Scrape Text:** Click on a price to scrape just that piece of information.

## 4. Click

- **What it Means (ELI5):** Click is like pressing a button on a webpage.
  
- **When to Use It:** Use a click to interact with elements on a webpage, like buttons, links, or menus.
  
- **How to Use It:** Record a step where you click on a specific element.

- **Use Cases:**
  - Clicking a "Submit" button after filling out a form.
  - Navigating through pages by clicking "Next."

- **Examples:**
  - **Click Step:** Record the step where you click the "Login" button.

## 5. Input Text

- **What it Means (ELI5):** Input text is like typing on a keyboard into a text box.
  
- **When to Use It:** Use input text to enter data into fields on a webpage.
  
- **How to Use It:** Record a step where you type into a specific field.

- **Use Cases:**
  - Entering login credentials on a sign-in page.
  - Filling out a search query on a search engine.

- **Examples:**
  - **Input Text Step:** Type "John Doe" into a name field.

## 6. Filter

- **What it Means (ELI5):** A filter is like a decision-maker that decides what to do next based on certain conditions.
  
- **When to Use It:** Use a filter to control the flow of your automation based on specific criteria.
  
- **How to Use It:** Set conditions that the data must meet to proceed to the next step.

- **Use Cases:**
  - Sending an email only if a form submission includes a certain keyword.
  - Skipping steps if a value is missing.

- **Examples:**
  - **Filter Step:** Check if a Google Sheet cell contains "Yes" before continuing.

## 7. Custom Data (Variables or Custom Data)

- **What it Means (ELI5):** Custom data is like a placeholder for information that can change each time the automation runs.
  - A variable is like a storage box that holds information you might need later.
  
- **When to Use It:** Use variables to store dynamic data that your automation needs to use later.
  
- **How to Use It:** Define variables during the recording and use them in subsequent steps.

- **Use Cases:**
  - Storing a user's name to personalize an email.
  - Keeping track of item prices during a scrape.
  - Keeping track of product IDs to use in multiple steps.

- **Examples:**
  - **Variable Step:** Save the scraped price as a variable to use in a calculation later.
  - **Set Variable Step:** Store the user's name from a form input to use in a follow-up email.

## 8. Navigate (URL or Go To Page)

- **What it Means (ELI5):** Navigate is like typing a new web address into your browser and hitting enter.
  
- **When to Use It:** Use navigate to change the webpage you're working on.
  
- **How to Use It:** Record a step where you type in a URL and load a new page.

- **Use Cases:**
  - Moving from a homepage to a product page.
  - Accessing different sections of a website.
  - Accessing different pages in a workflow.

- **Examples:**
  - **Navigate Step:** Enter "www.example.com/products" in the browser.
  - **Navigate Step:** Go to "www.example.com/login" to start a login process.

## 9. Play Steps

- **What it Means (ELI5):** Play steps is like pressing the play button on a video to watch your recorded actions happen automatically.
  
- **When to Use It:** Use play to test & run your automation and see it in action.
  
- **How to Use It:** Click the "Play" button to start your automation and execute the recorded steps.

- **Use Cases:**
  - Testing your automation to ensure it works correctly.
  - Running the automation to perform the recorded tasks.

- **Examples:**
  - **Play Steps Button:** Run the automation to log in and scrape data from a website.
  - **Play Button:** Execute the recorded automation to perform the steps.

## 10. Error Handling

- **What it Means (ELI5):** Error handling is like having a plan for what to do if something goes wrong.
  
- **When to Use It:** Use error handling to manage steps that might fail.
  
- **How to Use It:** Enable the "Allow Error" option for steps that could cause issues.

- **Use Cases:**
  - Continuing the automation even if a website element is not found.
  - Logging errors for review later.

- **Examples:**
  - **Allow Error:** Enable this for a step that sometimes fails due to network issues.

## 11. Loop

- **What it Means (ELI5):** A loop is like a repeat button that keeps doing the same thing over and over.
  
- **When to Use It:** Use a loop to repeat a set of steps multiple times.
  
- **How to Use It:** Define the start and end points of the loop, and set the number of repetitions.

- **Use Cases:**
  - Sending multiple personalized emails.
  - Scraping multiple pages of data.

- **Examples:**
  - **Loop Step:** Repeat the process of clicking "Next Page" and scraping data 10 times.

## 12. Schedule

- **What it Means (ELI5):** A schedule is like setting an alarm clock to remind you to do something at a specific time.
  
- **When to Use It:** Use a schedule to run automations at specific times or intervals.
  
- **How to Use It:** Set the date and time for the automation to run.

- **Use Cases:**
  - Running a report at the end of every week.
  - Checking for updates on a website every hour.

- **Examples:**
  - **Schedule Trigger:** Set the automation to run daily at 8 AM.

## 13. Webhook

- **What it Means (ELI5):** A webhook is like a messenger that sends data from one app to another automatically.
  
- **When to Use It:** Use a webhook to send data to or receive data from another application.
  
- **How to Use It:** Set up the webhook URL and configure the payload.

- **Use Cases:**
  - Sending form submission data to a CRM system.
  - Triggering an automation when new data is posted to a webhook.

- **Examples:**
  - **Webhook Step:** Send scraped data to a Google Sheets webhook for storage.

## 14. Action

- **What it Means (ELI5):** An action is something your automation does, like clicking a button or typing text.
  
- **When to Use It:** Use actions to perform tasks within your automation.
  
- **How to Use It:** Record or add actions like clicking, typing, or navigating.

- **Use Cases:**
  - Filling out forms.
  - Clicking through a sequence of pages.

- **Examples:**
  - **Click Action:** Automate clicking the "Submit" button on a form.

## 15. Selector

- **What it Means (ELI5):** A selector is like a pointer that tells your automation exactly where to click or type.
  
- **When to Use It:** Use selectors to identify elements on a webpage.
  
- **How to Use It:** Define or update the selector for a web element.

- **Use Cases:**
  - Clicking specific buttons or links.
  - Typing into specific text fields.

- **Examples:**
  - **Update Selector:** Adjust the selector to ensure it correctly targets the "Login" button.

## 16. Condition

- **What it Means (ELI5):** A condition is like a decision-maker that chooses what to do next based on certain rules.
  
- **When to Use It:** Use conditions to create branches in your automation based on specific criteria.
  
- **How to Use It:** Set conditions that must be met for different actions to occur.

- **Use Cases:**
  - Sending a different email based on the user's input.
  - Skipping steps if certain data is missing.

- **Examples:**
  - **Conditional Step:** Send a follow-up email only if the user hasn't responded within 3 days.

## 17. Screenshot

- **What it Means (ELI5):** A screenshot is like taking a photo of your computer screen.
  
- **When to Use It:** Use screenshots to capture the state of a webpage at a specific step.
  
- **How to Use It:** Add a screenshot step to capture the screen at any point in your automation.

- **Use Cases:**
  - Verifying that a page loaded correctly.
  - Keeping a record of data displayed on a webpage.

- **Examples:**
  - **Screenshot Step:** Capture the screen after filling out a form to verify the entered data.

## 18. Dynamic Data

- **What it Means (ELI5):** Dynamic data is like ingredients in a recipe that change each time you make the dish.
  
- **When to Use It:** Use dynamic data to make your automation adaptable to different inputs.
  
- **How to Use It:** Capture data during the automation run and use it in subsequent steps.

- **Use Cases:**
  - Personalizing email messages with names.
  - Using product IDs in multiple steps.

- **Examples:**
  - **Dynamic Data Use:** Insert a scraped product name into a Google Sheet.

## 19. Log

- **What it Means (ELI5):** A log is like a diary that keeps track of everything your automation does.
  
- **When to Use It:** Use logs to review the actions and results of your automation runs.
  
- **How to Use It:** Access logs from the TaskMagic interface to debug or verify automation steps.

- **Use Cases:**
  - Troubleshooting failed automations.
  - Verifying that all steps executed as expected.

- **Examples:**
  - **View Log:** Check the log to see where an error occurred in the automation.

## 20. Capture Steps

- **What it Means (ELI5):** Capture steps is like recording a video of your actions so you can play them back later.
  
- **When to Use It:** Use capture steps to create the initial recording of your automation.
  
- **How to Use It:** Click the "Start Capturing" button and perform the actions you want to automate.

- **Use Cases:**
  - Recording a login sequence.
  - Capturing the steps to fill out a form.

- **Examples:**
  - **Capture Steps Button:** Click to start recording your actions on a webpage.

## 21. Edit Step

- **What it Means (ELI5):** Edit step is like editing a single frame in a movie to change what happens.
  
- **When to Use It:** Use edit step to modify any recorded action.
  
- **How to Use It:** Click the three dots next to a step and choose "Edit" to make changes.

- **Use Cases:**
  - Correcting a mistyped value.
  - Changing the target of a click action.

- **Examples:**
  - **Edit Step Option:** Modify the selector used for a click action.

## 22. Custom JavaScript

- **What it Means (ELI5):** Custom JavaScript is like writing your own special instructions to make the automation do exactly what you want.
  
- **When to Use It:** Use custom JavaScript to perform complex tasks that aren't covered by standard actions.
  
- **How to Use It:** Add a custom JavaScript step and write your script.

- **Use Cases:**
  - Interacting with web elements in advanced ways.
  - Performing calculations or data manipulation.

- **Examples:**
  - **Custom JavaScript Step:** Scroll down a webpage by executing a custom script.

## 23. Convert Step

- **What it Means (ELI5):** Convert step is like changing a recipe ingredient to something else that still works.
  
- **When to Use It:** Use convert step to change the type of an existing step to another type.
  
- **How to Use It:** Select the step to convert and choose the new type.

- **Use Cases:**
  - Changing a click action to a hover action.
  - Converting a scrape text step to a scrape list step.

- **Examples:**
  - **Convert Step Option:** Change a click action to a scrape action.

## 24. Duplicate Step

- **What it Means (ELI5):** Duplicate step is like making a copy of a favorite recipe so you can use it again.
  
- **When to Use It:** Use duplicate step to reuse an action in your automation.
  
- **How to Use It:** Select the step and choose the "Duplicate" option.

- **Use Cases:**
  - Repeating a form submission with different data.
  - Scraping multiple similar sections on a webpage.

- **Examples:**
  - **Duplicate Step Option:** Copy a click action to use it again later in the automation.

## 25. Import Data

- **What it Means (ELI5):** Import data is like bringing in ingredients from another kitchen to use in your recipe.
  
- **When to Use It:** Use import data to bring external data into your automation.
  
- **How to Use It:** Connect to data sources like Google Sheets and use the data in your steps.

- **Use Cases:**
  - Using a list of email addresses from a spreadsheet.
  - Loading product details for processing.

- **Examples:**
  - **Import Data Step:** Pull in data from a Google Sheet to use in a form submission.

## 26. Export Data

- **What it Means (ELI5):** Export data is like sending a copy of your recipe to a friend.
  
- **When to Use It:** Use export data to save the results of your automation to an external source.
  
- **How to Use It:** Connect to data destinations like Google Sheets or webhooks and send the data.

- **Use Cases:**
  - Saving scraped data to a spreadsheet.
  - Sending form responses to a CRM.

- **Examples:**
  - **Export Data Step:** Save scraped product prices to a Google Sheet.

## 27. Schedule (Cron Job)

- **What it Means (ELI5):** Schedule is like setting a timer to do something at regular intervals.
  
- **When to Use It:** Use schedule to run automations at specific times or intervals.
  
- **How to Use It:** Set the timing and frequency for the automation to run.

- **Use Cases:**
  - Running a daily report.
  - Checking for website updates every hour.

- **Examples:**
  - **Schedule Step:** Set an automation to run every Monday at 9 AM.

## 28. API Integration

- **What it Means (ELI5):** API integration is like making a phone call to another app to get or send information.
  
- **When to Use It:** Use API integration to connect with other applications and exchange data.
  
- **How to Use It:** Set up API calls with the necessary endpoints and parameters.

- **Use Cases:**
  - Pulling data from a weather service.
  - Sending data to a project management tool.

- **Examples:**
  - **API Step:** Retrieve weather data from an API and use it in an automation.
