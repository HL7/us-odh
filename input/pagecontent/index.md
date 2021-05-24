### Overview

**HL7 FHIR Profile: Occupational Data for Health (ODH), Release 1.1 (Standard for Trial Use)**

This Implementation Guide is a reconciled version, containing changes in response to comments received in the Sept. 2018 ballot. It has been updated to FHIR R4.0.1.

**Introduction and Guidance**

This Implementation Guide (IG) contains profiles to implement support for Occupational Data for Health (ODH). ODH describes structured work information primarily designed to facilitate clinical care, including population health and value-based care. ODH also can be used to support public health reporting. ODH is not designed to support billing activities. 
This set of FHIR profiles is specified as a composition resource, but it is not intended to be used as a stand-alone composition. Rather, the desired content should be included in broader IGs and available as a response to requests for ODH information. Some use cases may leverage only a subset of the ODH profiles, and these should be specified within those work products. For instance, in the Vital Records Death Reporting (VRDR) IG, the data requirements for work information are limited to  those in the Usual Work profile.
While this profile is specified for the US Realm, the design is intended to also support international needs. Three of the referenced value sets—Occupation, Industry, and Supervisory Level— are necessarily US specific. The remaining three value sets—Work Schedule, Employment Status, and Work Classification—use international concepts. Input is requested regarding whether these should be specified as ‘extensible’, ‘required’ (using ‘text only’ where a concept does not yet exist such as a new occupation), or as an ‘example’ for those US specific concepts.

**Background**

The majority of adults in the U.S. spend more than half their waking hours at work. Therefore, health and work are inextricably inter-related. For example, the management of chronic conditions requires taking the patient’s work environment into consideration. Work-related conditions are often first brought to the attention of a primary care provider. Some conditions related to exposure to hazards in the workplace can have a long latency, requiring knowledge of a person’s work history for recognition, diagnosis, and treatment. The recognition of new conditions related to previously unknown workplace hazards has often come from astute clinicians, which requires knowledge of the patient’s work. ONC has indicated recognition of the value of work information for health care.
The incorporation of ODH into Electronic Health Records (EHRs) and other health IT systems presents an opportunity to improve health in relation to work. ODH provides a structure and standardization for work information that can be used across systems to take advantage of system tools for clinical decision support, population health, and public health. Research has been conducted and guidance is available to support clinicians, and the use of ODH by health IT systems can support identification of patients that would benefit the most from this knowledge.

**Scope**

The Occupational Data for Health (ODH) FHIR IG covers information about a patient’s work, including some voluntary work, or a patient’s household members’ work. ODH is designed for the social history section of a medical record, to facilitate clinical care in multiple disciplines and delivery environments. ODH can be used for clinical decision support, population health activities and value-based care, and public health reporting. The scope of the work information in ODH includes:

•	Employment Status

•	Retirement Date

•	Combat Zone Period

•	Past or Present Job for the patient or a household member, which includes:
		
		o	Past or Present Job Occupation
		
		o	Past or Present Job Industry
		
		o	Work Classification
		
		o	Work Schedule, which includes:
				
				- Weekly Work Days
				
				- Daily Work Hours
		
		o	Job Duty
		
		o	Occupational Hazard
		
		o	Employer name
		
		o	Employer address
		
		o	Related Subject (when it is Past or Present Job of a household member of the person)
		
		o	Start/End Dates

•	Usual Work of the patient or a household member, which includes:
		
		o	Usual Occupation
		
		o	Usual Industry
		
		o	Usual Occupation Duration
		
		o	Related Subject (when it is Usual Work of a household member of the person)
		
		o	Start Date

**Known Issues and Limitations**

This IG includes more extensive occupational data than typically collected in current systems. The content and structure of this IG is intended to inform clinical care, support population health, and contribute to public health activities. While there may be some overlap with administrative and billing information maintained by some systems, the information in this IG is not designed to support billing and administrative needs.
While multiple retirement dates are supported, the retirement date is not linked to any specific job, or usual occupation.

**Credits**

Co-Editor:
Lori Reed-Fourquet
e-HealthSign, LLC
lfourquet@ehealthsign.com

Co-Editor:
Rob Hausam
Hausam Consulting
rob@hausamconsulting.com

Co-Editor:
Mark Kramer
MITRE Corporation
mkramer@mitre.org

This set of FHIR profiles was produced and developed through the efforts of a project of the National Institute of Occupational Safety and Health (NIOSH), the U.S. federal agency responsible for conducting research and making recommendations for the prevention of work-related injury and illness. NIOSH is a part of the U.S. Centers for Disease Control and Prevention (CDC). NIOSH consulted stakeholders in clinical care, public health, health IT, health informatics and  U.S. government agencies to develop ODH. The HL7® Public Health and Emergency Response Work Group sponsored development of this set of FHIR profiles. Co-sponsoring HL7® Work Groups were Orders and Observations (OO), Patient Administration (PA), and Clinical Quality Initiative (CQI).
The following individuals provided subject matter expertise for this set of FHIR profiles: Genevieve Barkocy Luensman, NIOSH; Eileen Storey, Professional Services Partners, formerly NIOSH; Margaret S. Filios, NIOSH; Christina Socias-Morales, NIOSH; Lauren Brewer, NIOSH; Barbara Wallace, Professional Services Partners.

**Authors**

Name	Email/URL
HL7 International - Public Health	http://www.hl7.org/Special/committees/pher



### Authors

<table>
<thead>
<tr>
<th>Name</th>
<th>Email/URL</th>
</tr>
</thead>
<tbody>
<tr>
<td>HL7 International - Public Health</td>
<td><a href="http://www.hl7.org/Special/committees/pher" target="_new">http://www.hl7.org/Special/committees/pher</a></td>
</tr>
</tbody>
</table>


