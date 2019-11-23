# MirthConnect - Custom Fhir implementation 
MirthConnect - Custom Fhir implementation helps you do coding on the FHIR resources. 
It is very simple to use.

## How to?

### MirthConnect Server

* Download the Jar mirth-fhir1.0.0.jar to MirthConnect server
* Navigate to home folder of MirthConnect
* Open custom-lib folder 
* Put the downloaded mirth-fhir1.0.0.jar inside custom-lib folder.

### MirthConnect Administrator

* Log in to your MirthConnect Administrator.
* Click on Setting from the side window
* From the main content navigate to Resources Tab.
* Click on Reload resource from the side window.
* Click Yes on the confirmation window to let MirthConnect know mirth-fhir1.0.0.jar is loaded

#### MirthConnect Code Library

* Download Fhir.xml to your desktop
* Click Dashboard on the side window
* Click Channels on the side window
* Click on Edit Code Templates on the side window
* Click on Import Code Templates
* Select Fhir.xml from your desktop and Click Open

#### MirthConnect Channels

* On your Channel Summary, make sure you have Set Dependencies with imported(Fhir) Code Template library.
* In your Javascript you can initiate the fhirObject as given below
```java
var results = fhirObj.init('cerner');
channelMap.put('results',results);
```
HAPPY CODING !!
