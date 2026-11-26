# AdverseChildhoodExperience
Using NHS commissioning data sets to seek to create a population view of children experiencing adverse events

This is a developmental piece of work, and is not finished although it is very close. 

There are 4 parts to the code shared here:

## ACEDataPrepCDS 
This quarto applies the ACEs in EHR code list <https://acesinehrs.com/> to NHS commissioning data sets Data sets in support of statutory duties - NHS England Digital <https://digital.nhs.uk//services/data-services-for-commissioners/datasets-in-support-of-statutory-duties>

The following direct translate into NHS commissioning data sets
-   Diagnosis list for inpatients ICD10
-   Procedure code list for inpatients OPCS4
-   OP code list is for treatment specialty
-   AE codelist is a historical code set not used in ECDS

  ### Additional Searches
-   Mental Health Minimum Dataset for any patient in MPI table
-   IAPT for any patient in MPI table
-   Alcohol dependency services
-   999 for assaults and MH
-   111 for MH
-   Deaths for assault/suicide
-   prescribing in primary care for antipsychotics and antidepressants

## ACEBSOLDataCaptureProcess
This quarto looks at how the codelist have transferred and being extended and which records are being returned.
The purpose is to understand whether there are any biases in the approch and whether there are any deficits.

## ACEparentalarrangementsCDS
#### Identifying parents from commissioning data sets
ACE is based on parental exposures, therefore need way to identify if the children are living with parents and who their parents are. Especially to look at parental separation. The only parental link directly recorded in commissioning data sets is between mother and their baby. At birth registration the Mother's and Father's Date of Births are recorded. Could this be sufficient to link to who a child is living with today.

## ACESummaryCDS
This quarto brings in the people who have matched the ACE in EHR criteria and the extension to other Commissioning data sets. 

It builds an exposure table, brings in the parental linkages and then identifies children in those households who could have experienced an adverse event. 
