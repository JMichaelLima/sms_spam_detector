# sms_spam_detector

## Requirements
### Create the SMS Classification Function
The features variable is set equal to the text message column of the DataFrame.

The target variable is set equal to the "label" column of the DataFrame.

The data is split into training and testing sets, and the test_size is set to 33%.

A Pipeline is built using the TfidfVectorizer and LinearSVC to transform the test set and compare it to the training set.

The model is fitted to the transformed training data and the model is returned.

The SMSSpamCollection.csv is read into a DataFrame.

The DataFrame is passed to the sms_classification function and the result is set equal to the "text_clf" variable.

### Create the SMS Prediction Function
A variable that holds the prediction of a new text is created.

A conditional statement that determines if the text message is "ham" or “spam” is created.

The conditional returns a message if the text is “ham”.

The conditional returns a message if the text is “spam”.

### Create the Gradio Interface Application
A Gradio Interface application is created with three parameters for the “function”, “outputs”, and “inputs”.

The “outputs” parameter is a textbox that contains a label to let the user know what to type in the box.

The “inputs” parameter is a textbox that contains a label to let the user know that the prediction will be displayed in the textbox.

The Interface application can be shared with other users with a public URL.

The Gradio Interface works as expected and there are no errors after a user submits a text message.