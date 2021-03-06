# Generate Emails with customised Content Automatically

Be it sending automatic alert mails when our IOT system crosses thresholds, or attracting more footprint to our ecommerce site through sending personalised offers, you're at the right place to tedious monotonous work.

Let's see how we can leverage Python to generate and send custom emails targeted to different users automatically!

## 1. Storing list of contacts in a txt file:
For this, we will store the list of contacts in `Contacts.txt` file, in the following format:

NAME EMAILID

Below is how our `Contacts.txt` file looks:

![](https://github.com/archanago/Automatic_Email_Generation_Python/blob/master/Contacts%20List.PNG)

Our program will be reading from this list and will send mail to each one

## 2. Storing the message template in a txt file:
Use Template Strings in Python and type in the message to be sent to every user and store it in a `txt` file.
Later on, our program reads this template and replaces template strings objects with respective values and finally sends mesage to each of the contacts in Contacts List.

Below is the content of our message template:

![github-small](https://github.com/archanago/Automatic_Email_Generation_Python/blob/master/Message%20Template.PNG)

## 3. Email Generation:

### A. Connecting to the Server:
It is first essential to establish a successful connection with our server. For this, we'll connect through Port 

### B. Reading the list of contacts:
The List of contacts are read into two lists namely `names` to contain the list of all names in `Contacts.txt` and `emails`to contain the list of corresponding EmailIDs.

### C. Reading the message template:
The `Message.txt` file is read into our program as a Template object. This step is crucial, as the values are to be addressed before finally sending the emails.

### D. Generating Emails:
The email is finally generated by replacing the Template Strings with corresponding values. This generated email content is finally sent to the set of all recepients at one go!

We can see the automatic mail received. Observe that the `$NAME` is changed to 'Honey' (actual value)

![github-small](https://github.com/archanago/Automatic_Email_Generation_Python/blob/master/Automatic%20mail.JPG)

This way, we can save our wokday by leveraging Python.
