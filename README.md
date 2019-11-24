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
var fhir = new fhirObj().init();
responseMap.put('results',fhir.getPatient("100000006"));
```
## Documentation on methods and it's usage

1. The <code>getPatientFull(PatientID)</code> method will return full details about the patient which includes all the sections.
``` javascript
fhir.getPatientFull("100000006")
```
2. The <code>getPatient(PatientID)</code> method will return Demographics of the patient.
``` javascript
fhir.getPatient("100000006")
```
3. The <code>getPatients()</code> method will return list of all patients.
``` javascript
fhir.getPatients()
```
4. The <code>getPractitioners()</code> method will return list of all practitioners.
``` javascript
fhir.getPractitioners()
```
5. The <code>getPatientAllergyIntolerance(PatientID)</code> method will return AllergyIntolerance of the patient.
``` javascript
fhir.getPatientAllergyIntolerance("100000006")
```
6. The <code>getPatientAppointment(PatientID)</code> method will return Appointment of the patient.
``` javascript
fhir.getPatientAppointment("100000006")
```
7. The <code>getPatientCondition(PatientID)</code> method will return Condition of the patient.
``` javascript
fhir.getPatientCondition("100000006")
```
8. The <code>getPatientDiagnosticReport(PatientID)</code> method will return DiagnosticReport of the patient.
``` javascript
fhir.getPatientDiagnosticReport("100000006")
```
9. The <code>getPatientDocumentReference(PatientID)</code> method will return DocumentReference of the patient.
``` javascript
fhir.getPatientDocumentReference("100000006")
```
10. The <code>getPatientEncounter(PatientID)</code> method will return Encounter of the patient.
``` javascript
fhir.getPatientEncounter("100000006")
```
11. The <code>getPatientImmunization(PatientID)</code> method will return Immunization of the patient.
``` javascript
fhir.getPatientImmunization("100000006")
```
12. The <code>getPatientMedication(PatientID)</code> method will return Medication of the patient.
``` javascript
fhir.getPatientMedication("100000006")
```
13. The <code>getPatientObservation(PatientID)</code> method will return Observation of the patient.
``` javascript
fhir.getPatientObservation("100000006")
```

:+1: :sparkles: :camel: :tada: :rocket: :metal: :octocat:  HAPPY CODING :+1: :sparkles: :camel: :tada: :rocket: :metal: :octocat: 
