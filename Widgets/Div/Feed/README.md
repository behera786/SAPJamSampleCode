SAP Jam div-embedded feed widgets
=======================

These SAP Jam div-embedded feed widgets written in HTML5 and Javascript each use a different method of authentication to access your instance of SAP Jam. To use these files make sure to replace <jam#> in these source files with your SAP Jam instance name before you load them into a web browser.

### Pre-existing SAP Jam session
* The widget uses an existing SAP Jam session. It shows an error message if a session has not already been established.
* Div_Pre-existing_session.html

### SAP Jam session with Sign In
* The widget uses an existing SAP Jam session if one is available. If the session is not yet established, your page is replaced by the SAP Jam Sign In page. After signing in, the user is returned to your page.
* Div_Session_with_sign-in.html

### SAP Jam session with Sign In pop-up
* The widget uses an existing SAP Jam session if one is available. If the session is not yet established, a new window or browser tab shows the SAP Jam Sign-In page. After signing in, the window closes and the widget is displayed.
* Div_Session_with_sign-in_pop-up.html

### Single Use Token
* The widget uses a temporary authentication token provided by the SAP Jam Authorization API. A single-use token can be used to obtain a valid Jam UI session. Once the token has been used, it is no longer valid. A single-use token can be generated by performing a [POST] /v1/single_use_tokens API call.
* Div_single_use_token.html

### SuccessFactors IdentityProvider
* The widget uses an existing SAP Jam session if one is available. If the session is not yet established, it creates a new window or browser tab and looks for an existing SuccessFactors session. If the single sign-on fails, the new window displays the SuccessFactors Sign In page. Once a session is established, the window closes and the widget is displayed.
* Div_SuccessFactors_IDP.html


# License
Copyright 2014, SAP AG

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.