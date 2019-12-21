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
var fhir = new fhirObj().init("cerner","DSTU2");
```
## Documentation on methods and it's usage

1. The <code>getPatientFull(PatientID)</code> method will return full details about the patient which includes all the sections.
``` javascript
fhir.getPatientFull("100000006")
```
2. The <code>getPatientDemographics(PatientID)</code> method will return Demographics of the patient.
``` javascript
fhir.getPatientDemographics("100000006")
```
3. The <code>getUserList("Patient")</code> method will return list of all patients.
``` javascript
fhir.getUserList("Patient")
```
4. The <code>getUserList("Practitioner")</code> method will return list of all practitioners.
``` javascript
fhir.getUserList("Practitioner")
```
5. The <code>getPatientResourceList(PatientID,"AllergyIntolerance")</code> method will return AllergyIntolerance of the patient.
``` javascript
fhir.getPatientResourceList("100000006","AllergyIntolerance")
```
6. The <code>getPatientResourceList(PatientID,"Appointment")</code> method will return Appointment of the patient.
``` javascript
fhir.getPatientResourceList("100000006","Appointment")
```
7. The <code>getPatientResourceList(PatientID,"Condition")</code> method will return Condition of the patient.
``` javascript
fhir.getPatientResourceList("100000006","Condition")
```
8. The <code>getPatientResourceList(PatientID,"DiagnosticReport")</code> method will return DiagnosticReport of the patient.
``` javascript
fhir.getPatientResourceList("100000006","DiagnosticReport")
```
9. The <code>getPatientResourceList(PatientID,"DocumentReference")</code> method will return DocumentReference of the patient.
``` javascript
fhir.getPatientResourceList("100000006","DocumentReference")
```
10. The <code>getPatientResourceList(PatientID,"Encounter")</code> method will return Encounter of the patient.
``` javascript
fhir.getPatientResourceList("100000006","Encounter")
```
11. The <code>getPatientResourceList(PatientID,"Immunization")</code> method will return Immunization of the patient.
``` javascript
fhir.getPatientResourceList("100000006","Immunization")
```
12. The <code>getPatientResourceList(PatientID,"MedicationOrder")</code> method will return Medication of the patient.
``` javascript
fhir.getPatientResourceList("100000006","MedicationOrder")
```
13. The <code>getPatientResourceList(PatientID,"Observation")</code> method will return Observation of the patient.
``` javascript
fhir.getPatientResourceList("100000006","Observation")
```

:+1: :sparkles: :camel: :tada: :rocket: :metal: :octocat:  HAPPY CODING :+1: :sparkles: :camel: :tada: :rocket: :metal: :octocat: 
