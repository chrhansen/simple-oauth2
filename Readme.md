Simple OAuth 2.0

Currently setup for Google API (Gmail, Google+ etc.) but should work for other OAuth 2.0 services.

1. Register and app here: https://code.google.com/apis/console/ (or other OAuth 2.0 service)

2. Insert your Client ID and Client Secret in ViewController.m (and optionally change the authentication-url and token-url if you're not using Google API)


3. Run the app. The sign method is called in viewDidLoad in ViewController.m

4. When the user has successfully authenticated your viewController:finishedWithAuth:error: will be called (it's also in ViewController.m), here you can also retrieve the access_token for later authentication.

 