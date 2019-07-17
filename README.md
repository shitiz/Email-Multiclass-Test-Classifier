# Email-Multiclass-Test-Classifier
It's a multi class text classifier for emails saved as images.

The images are saved initially as tiff format which we initially convert to jpeg format for easy data extraction. The emails could belong to either of the six categories/classes.

The type of data on which the models are created are given for reference with each class sample as tiff image.

The data extraction is done through open source library Tesseract and then the body of the email is extracted to identify the class it belong to based upon its content. The preprocessing after extracting the email body includes adding corresponding numeric field for each class, removing stop words like a, an, the etc and any punctuation which are not required to judge the type of the content.

Once data is cleaned, it is vectorized to give a numeric represenation and feeded to 4 different models using sklearn to train & test.
- Naive Bayes
- SVC
- Random Forest
- Logistic Regression

The various metrics what we calculate the model performance are Accuracy, Confidence Score and full Summary report to have insight about various other metric values like F1 score, precision etc.
