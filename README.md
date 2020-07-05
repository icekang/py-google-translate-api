# Google Translate API with Python request

Python library is cool, as many know that we can simply use https://pypi.org/project/googletrans/ which is free and unlimited.
But how about we do it ourselves for fun-sake! With basic POST request you can directly make a call to google translate!

Google Translate API documentation (that I mimick the "curl" example)
https://cloud.google.com/translate/docs/basic/setup-basic

## Getting start
1. Please follow the [document](https://cloud.google.com/translate/docs/basic/setup-basic) on the official website
2. You should now have...
    - created a project for google translation api
    - download private json key
    - set GOOGLE_APPLICATION_CREDENTIALS env variable to the full PATH to your json file
    - install **gcloud sdk**

To check if you're ready for curl request, try running this command on your console:
`gcloud auth application-default print-access-token`
This should reture access token for google translation API

Note: `json` file contains key and links need for you to refresh you token after it expires. Running the `gcloud` commands does all the work for requesting for a token or refreshing the token
