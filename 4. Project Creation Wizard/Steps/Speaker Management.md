- [[Project Manager (PM)]] can select already added speakers from the list. System will send them invite for the project.
	- Languages of each speaker is displayed.
	- Rating of each speaker is displayed.

![[step2_speaker_management.png]]

In addition to selecting already added speakers, [[Project Manager (PM)]] can also add a speaker manually.
In this case, system will send Sign Up link on speakers email.

Fields are:
- **Speaker Name *(Required Field)*:** Name of the speaker.
- **Email *(Required Field)*:** Email of the speaker on which to send Sign Up link.
- **Languages *(Required Field)*:** All languages which speaker can speak separated with comma.
	- First language will be set as Primary Language in Speaker Profile. 
	- Second language will be set as Secondary Language in Speaker Profile. 
	- Others will be set in additional languages in Speaker Profile.

![[step2_add_speaker_manually.png]]

Also speakers can be added using excel file. System will import all users from excel file: 
- Will send Invite Link to the speakers which already exists in database.
- Will send Sign Up Link to the speakers which does not exist in database.

![[step2_add_speaker_from_file.png]]

The format of excel file is as follows:
- Speaker ID will be removed in actual app.

| Name             | Email                                               | Role     | Speaker ID | LanguageA | LanguageB | LanguageC_list |
| ---------------- | --------------------------------------------------- | -------- | ---------- | --------- | --------- | -------------- |
| Sarah Martinez   | [sarah@example.com](mailto:sarah@example.com)       | recorder | SPK1       | EN-US     | ES-MX     |                |
| Carlos Rodriguez | [carlos@example.com](mailto:carlos@example.com)     | recorder | SPK2       | ES-MX     | EN-US     | FR-FR          |
| Marie Dubois     | [marie@example.com](mailto:marie@example.com)       | recorder | -          | FR-FR     | EN-US     |                |
| James Thompson   | [james@example.com](mailto:james@example.com)       | recorder | SPK4       | EN-US     |           |                |
| Emma Wilson      | [emma@example.com](mailto:emma@example.com)         | recorder | -          | EN-US     |           |                |
| Lucas Torres     | [lucas@example.com](mailto:lucas@example.com)       | recorder | SPK6       | ES-MX     |           |                |
| Ana Silva        | [ana@example.com](mailto:ana@example.com)           | recorder | SPK7       | PT-BR     | ES-MX     | EN-US          |
| Diego Perez      | [diego@example.com](mailto:diego@example.com)       | recorder | SPK8       | ES-MX     | EN-US     |                |
| Sophie Laurent   | [sophie@example.com](mailto:sophie@example.com)     | recorder | -          | EN-US     |           |                |
| Maria Lopez      | [maria@example.com](mailto:maria@example.com)       | recorder | SPK10      | ES-MX     | PT-BR     |                |
| John Smith       | [john@example.com](mailto:john@example.com)         | recorder | SPK11      | EN-US     |           | FR-FR, PT-BR   |
| Gabriela Santos  | [gabriela@example.com](mailto:gabriela@example.com) | recorder | SPK12      | EN-US     |           |                |
