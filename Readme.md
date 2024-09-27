## Exercise_8-UiPath-Basic_Web_Automation-Fill_a_Web_Form

## Aim:
To automate the process of filling out a web form using the Application/Browser activity in UiPath Studio.

## Equipment Required:
UiPath Studio installed on your computer.<br>
Web Browser (e.g., Chrome, Edge, with UiPath extensions installed).<br>
Computer with:<br>
Minimum 4 GB RAM.<br>
Minimum 2.0 GHz CPU.<br>
Windows operating system.<br>
A Web Form to be automated.

## Procedure:
### Create a New Project in UiPath Studio:
Open UiPath Studio and create a new project by selecting Process under the New Project tab.<br>
Name the process (e.g., Web Form Automation Using Application/Browser) and click Create.

### Install the Browser Extension:

To interact with a web browser, install the necessary UiPath browser extension:<br>
Go to the Tools section in UiPath Studio.<br>
Install the extension for the browser you will use (e.g., Chrome or Edge).

### Use Application/Browser Activity:

Instead of using the Open Browser activity, we will use the Use Application/Browser activity.<br>
In the Activities panel, search for Use Application/Browser and drag it into the Main sequence.<br>
In the Application/Browser field, click Indicate Application on Screen, then navigate to the browser where the web form is located and indicate the web form window or tab.<br>
Once the browser is selected, it will embed the browser as part of the automation.

### Navigate to Web Form:

After setting up the Use Application/Browser activity, use the Navigate To activity to navigate to the web form’s URL.<br>
Inside the Use Application/Browser container, search for Navigate To and add it to the workflow.<br>
In the URL property of Navigate To, enter the URL of the web form.

### Fill in Web Form Fields:

To input data into the form, use Type Into activities for each field on the form.<br>
Steps:<br>

Search for the Type Into activity in the Activities panel and drag it into the sequence under the Navigate To activity.<br>
Click the Indicate on Screen button in the Type Into activity and select the form field where you want to enter the data (e.g., the Name field).<br>
Enter the text (e.g., "John Doe") in the Text property of the Type Into activity.<br>
Repeat this step for each form field, such as Name, Email, Phone, etc.

### Select Dropdowns or Checkboxes (if applicable):

For dropdown fields, use the Select Item activity.<br>
For checkboxes or radio buttons, use the Check activity.<br>
Steps:<br>
Search for Select Item for dropdowns. Indicate the dropdown field and specify the value in the Item property.<br>
Use Check to select checkboxes or radio buttons, and indicate the field on the web form.

### Submit the Form:

To submit the form, use the Click activity.<br>
Drag the Click activity below the fields that you filled out.<br>
Click Indicate on Screen in the Click activity and select the Submit button on the web form.

### Save and Run the Workflow:

Press CTRL+S to save the workflow.<br>
Click the Run button to execute the automation.<br>
The robot will open the web form in the browser, fill in the details as provided in the Type Into activities, and submit the form.

## UiPath WorkFlow:
![alt text](<img/Screenshot 2024-09-26 214141.png>)
![alt text](<img/Screenshot 2024-09-26 214337.png>)
![alt text](<img/Screenshot 2024-09-26 214406.png>)
![alt text](<img/Screenshot 2024-09-26 220051.png>)
![alt text](<img/Screenshot 2024-09-26 220132.png>)
![alt text](<img/Screenshot 2024-09-26 220358.png>)
![alt text](<img/Screenshot 2024-09-26 220412.png>)
![alt text](<img/Screenshot 2024-09-26 220412.png>)
![alt text](<img/Screenshot 2024-09-26 220522.png>)
![alt text](<img/Screenshot 2024-09-26 220616.png>)

## Result:
The web form is successfully filled and submitted using UiPath Studio with the Application/Browser activity, demonstrating the automation of a web-based form without explicitly opening a browser each time.