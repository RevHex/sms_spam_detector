# SMS Spam Detector

## Background
You'll be refactoring code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model. Once the model is created and trained, you will create a Gradio app to host the application, enabling users to test text messages. The application will provide feedback to users, indicating whether the text is classified as spam or not, based on the model's performance.

## Files
- Module 21 Challenge files (Downloaded from the course platform)

## Setup
- Create a repository named `sms_spam_detector`.
- Clone the repository locally.
- Add the starter files to your local Github.
- Push changes to GitHub.

## Instructions

### Part 1: Create the SMS Classification Function
**Set Features Variable**
   - Assign the text message column of the DataFrame to the `features` variable.
**Set Target Variable**
   - Assign the "label" column of the DataFrame to the `target` variable.
**Data Split**
   - Split the data into training and testing sets with a test size of 33%.
**Build Pipeline**
   - Create a pipeline to transform the test set to compare to the training set.
**Fit Model**
   - Fit the model to the transformed training data and return the model.
**Load Data**
   - Load the `SMSSpamCollection.csv` into a DataFrame.
   - Call the `sms_classification` function with the DataFrame and assign the result to the `text_clf` variable.

### Part2: Create the SMS Prediction Function

**Create Prediction Variable**
  - Create a variable that will hold the prediction of a new text.
**Conditional Statement**
   - Use a conditional statement to determine if the text message is "ham" or "spam".
**Return Message**
   - If the message is "ham", the function should return: 
     ```python
     f'The text message: "{text}", is not spam.'
     ```
   - If the message is "spam", the function should return:
     ```python
     f'The text message: "{text}", is spam.'
     ```

### Part 3: Create the Gradio Interface Application

**Create Interface**
  - Create a Gradio Interface application with:
     - A textbox for inputs.
     - A textbox for outputs.
  - Ensure textboxes have labels describing their contents.
**Launch Application**
  - Launch the application and provide the URL to share the application.

### Part 4: Test the Application

- Use the following text messages to test your application:
  1. You are a lucky winner of $5000!
  2. You won 2 free tickets to the Super Bowl.
  3. You won 2 free tickets to the Super Bowl. Text us to claim your prize.
  4. Thanks for registering. Text 4343 to receive free updates on medicare.

## Submission
Submit your GitHub repository URL through the course platform.

## Support
Utilized Xpert Learning Assistant, office hours, class Slack channel, and previous jupyter notebook classwork for help.
