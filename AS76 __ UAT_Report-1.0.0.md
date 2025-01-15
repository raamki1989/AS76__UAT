# Purpose

The purpose of this user acceptance testing is to sufficiently test the AS76 with PBS system and validate that it meets the user requirements.

# Regulatory Information of the device


| Product | Applicant | Regulation | Classification |
| :---- | :---- | :---- | :---- |
| AS76 with PBS | Sigtuple Technologies Private Limited | CE-IVDR | Class A |
|  |  | US-FDA 510(k) | Class II |
|  |  | CDSCO | Class A |

# Intended purpose of the device
The AS76 with PBS system is intended to locate and display images of white blood cells, red blood cells and
platelets acquired from peripheral blood smears and assist a qualiﬁed reviewer in conducting a WBC diﬀeren-
tial count, evaluating RBC morphology, estimating Platelet count, and evaluating Platelet morphology using
those images. It is meant for in vitro diagnostic use by a qualiﬁed professional only.

# Intended Population

This device is intended for use by the general population. 

# References

1. User requirement specification \- L4\_PM\_URS\_066  
2. User manual \- L3_PM_UMN_040

# Validation overview

## System configuration

| Device Id | System release |
| :---- | :---- |
| Device ID |FFP-007|
| Package version | 1.0.0-validation-drop-alpha-18 |

## Testers
|       |       |
| :---- | :---- |
| Number of testers |1|
| Tester qualification |Adequately trained on the operations of the device and the reporting applicaiton| 

## Validation schedule

| |  |
| :---- | :---- |
| Estimated number of working days to execute validation | 2 | 
| Criteria to complete the validation |No High Priority bugs are observed and are open |

## Bug prioritization
All the bugs that are observed during the validation shall be prioritised considering the impact of the issue to the user and the probability of usage of the feature. The SOP is documented in the document - Work instruction- bugs workflow and fix timelines - Document Id:L3-DD-WIB-040-Workinstruction-Bugs workflow and fix timelines V2.0

## Requirements traceability

Each test case of this validation protocol is derived from a user requirement. Each test-case is linked to it's corresponding user requirement. The completeness of the flow-down of user requirements to test cases in this validation protocol has been reviewed and established.

# Test Cases

## General requirements 

Date of execution: 09-Jan-25

| Test Case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.GEN.001 | UR.GEN.001 | Power on the device | Connect the power cord of the device to a recommended power source | The power cord shall get connected properly to the power source | The power cord is connected properly | Pass |  |
|  |  |  | Turn the power switch ON | The device shall be powered ON and the login page shall be displayed | The device is powered ON and the login page is displayed| Pass |  |
| UT.GEN.002 | UR.GEN.002 | Login to the device application with valid credentials | Enter a valid user name.  | The user name shall be accepted | The user name is accepted | Pass |  |
|  |  |  | Enter valid password | The entered password shall be accepted | Entered password is accepted | Pass |  |
|  |  |  | Select "Sign in" | The login to the device shall be successful | The login is successful |Pass  |  |
| UT.GEN.003 | UR.GEN.002 | Login to the device application with invalid credentials | Enter invalid user name | The user name shall be accepted | The user name is accepted | Pass |  |
|  |  |  | Enter an invalid password.  | The entered password shall be accepted |The password is accepted|Pass  |  |
|  |  |  | Select "Sign in" | The login to the device shall not  be successful and an error message indicating invalid login shall be displayed | Login to the device is unsuccessful and the eror messages are indicated |Pass  |  |
| UT.GEN.004 | UR.GEN.002 | Login to the reporting application with valid credentials | Open the Browser and enter the URL of the application | The application shall get opened and the login page shall be displayed. | The login page is displayed |Pass  |  |
|  |  |  | Enter a valid user name.  | The user name shall be accepted | The user name is accepted |Pass  |  |
|  |  |  | Enter valid password | The entered password shall be accepted |The password is accepted|Pass  |  |
|  |  |  | Select "Sign in" | The login to the reporting application shall be successful |The login to the reporting application is successful|Pass  |  |
| UT.GEN.005 | UR.GEN.002 | Login to the reporting  application with invalid credentials | Open the Browser and enter the URL of the application | The application shall get opened and the login page shall be displayed.  | The login page is displayed |Pass  |  |
|  |  |  | Enter invalid user name | The user name shall be accepted |The entered user name is accepted  | Pass |  |
|  |  |  | Enter an invalid password.  | The entered password shall be accepted |The entered Password is accepted| Pass |  |
|  |  |  | Select "Sign in" | The login to the reporting application shall not  be successful and an error message indicating invalid login shall be displayed | The login is unsuccessful and the error message is displayed | Pass |  |
| UT.GEN.006 | UR.GEN.004 | Logout of the device application | Select the user profile icon present in the toolbar | The following user profile options shall be displayed. Time zone, Change password and  Logout  | The mentioned options are displyed | Pass |  |
|  |  |  | Select “Logout” | The user shall be logged out of the device. If there are any system operations in process, then those shall get terminated.  | The user is logged out of the device | Pass |  |
| UT.GEN.007 | UR.GEN.004 | Logout of the reporting application | Select the user profile icon present in the list report page | The following user profile options shall be displayed. Tiem zone, Change password and Logout  |The mentioned options are displayed  |Pass  |  |
|  |  |  | Select “Logout” | The user shall be logged out of the application.  | The user is logged out of the application |Pass  |  |
| UT.GEN.008 | UR.GEN.005 | Connect the device to the network using WIFI | Select the WIFI icon | The list of networks available for connection shall be displayed |The list of network is displayed  | Pass |  |
|  |  |  | Select a network from the list | The option to enter the password to connect to the network shall be displayed | The option to enter the password is displayed |Pass|  |
|  |  |  | Enter the password | The entered password shall be validated, and the device shall be connected to the selected network. This network shall be remembered by the system and shall get reconnected.  | The device is connected to the selelcted network and is reconnected when rebooted | Pass |  |
| UT.GEN.009 | UR.GEN.005 | Connect the device to a network using ethernet | Connect an ethernet cable to the device | The system shall detect the connection and connect to the network automatically.  | NA | Not Executed |  |
| UT.GEN.010 | UR.GEN.005 | Connect an external display to the system | Connect an external monitor to the device through the HDMI port | The user shall be able to perform the reporting by accessing the application from the monitor.  | The reporting was possible with the extended monitor | Pass |  |
| UT.GEN.011 | UR.GEN.005 | Connect to external input peripherals | Connect an external mouse and keyboard to the device | The user shall be able to provide inputs on the UI using the external mouse and keyboard.  | Able to connect mouse and keyboard and provide inputs | Pass |  |
| UT.GEN.012 | UR.GEN.001 | Power off the device | Select the power menu | The following power menu options shall be displayed Shutdown and  Restart |The mentioend menu options are displayed  | Pass |  |
|  |  |  | Select "Shutdown" | The system shall get powered off, and all the system operations (if any) shall be terminated.  | The device is powered off | Pass |  |
| UT.GEN.013 | UR.GEN.001 | Restart the device | Select the power menu | The following power menu options shall be displayed Shutdown Restart | The mentioned options are displayed | Pass |  |
|  |  |  | Select "Restart" | The system shall get restarted, and all the system operations (if any) shall be terminated before the system powers off.  | The system is restarted | Pass |  |

## Scanning Requirements

| Test Case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.SCN.001 | UR.SCN.001 | Place the slides on the tray and  | Load the slides onto the tray | The slides shall be placed onto the tray without popout or breakage.  | The slides are placed without breakage | Pass |  |
| UT.SCN.002 | UR.SCN.002 | Place the tray into the system. | Load the tray onto the device | The tray shall be placed in the device without any popout or breakage of the slide.  | THe tray is placed in the device | Pass |  |
| UT.SCN.003 | UR.SCN.003 | View the decoded barcode information | Place the loaded tray into the system and select confirm | The barcode of the slides shall be captured and decoded by the system and shall be populated in the slide creation page |The barcode is decoded and is displayed in the slide details page  | Pass |  |
| UT.SCN.004 | UR.SCN.004 | Enter/update the slide ID of the slide.  | Select the slide ID field | The slide ID field shall be editable, and the keypad shall be populated. The preview of the barcode region of the slide shall be displayed.  | The barcode region is populated | Pass |  |
|  |  |  | Enter the slide ID | The entered details shall be validated and accepted | The entered slide details are accepted |Pass|  |
| UR.SCN.005 | UR.SCN.006, UR.SCN.008 | Initiate the scans for the loaded slides | Select “Next” from the slide details page | The scan shall get initiated for the slides loaded in the tray after oil is dispensed.  | The scans are initiated and the oil is also dispensed. | Pass |  |
|  |  |  | View the on-going scans | The progress and the status of scans for each slide, along with the warning and order status, shall be displayed. The scan summary shall be displayed along with the exceptions (if any) and the tray shall be ejected | As expected |Pass  |  |
|  |  |  | Remove the tray and mark as "Done.” to finish the scans or “Insert another tray” to scan another tray of slides.  | The tray shall be taken back to the home position if “Done” is selected, or the slide insertion page shall be displayed if “Insert another tray” is selected.  | As expected | Pass |  |
| UT.SCN.006 | UR.SCN.007 | Abort the scans for one or more slides | Initiate the scans for a tray | The scans shall get initiated and the system shall capture the images | The scan is initiated and the images are captured | Pass |  |
|  |  |  | Select “Abort scans” | The option to abort either all queued scans or on-going scans shall be displayed | The mentioned options are displayed | Pass |  |
|  |  |  | Select “Abort scans for all queued slides.” | All the slides that are in queue for scanning shall be aborted and the status shall get changed to failed | The queue slides are aborted | Pass |  |
|  |  |  | Select “Abort scans” | The option to abort either all queued scans or on-going scans shall be displayed | The mentioned options are displayed |Pass  |  |
|  |  |  | Select “Abort scans for the in-progress slide” | The slide that is in the process of capturing the images shall be aborted, and the status shall get changed to failed.  | The in progress slide is aborted | Pass |  |
| UT.SCN.007 | UR.SCN.009 | View the history of scanned slides | Select "History" | The list of slides that were scanned on the device shall be displayed along with the status and the timestamp of scanning | The list of slides are displayed | Pass |  |
|  |  |  | Select the filter criteria as  Days Status	 | The list shall get filtered as per the criteria applied.  | The list gets filtered as per the criteria applied | Pass |  |

## Review and reporting requirements

| Test case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.RPT.001 | UR.REP.001 | View the list of reports | Login to the reporting application with valid credentials | The login shall be successful and the list of reports shall be displayed as  To be reviewed Preparing Reviewed  |The login is successful and the list report page is displayed| Pass|  |
| UT.RPT.002 | UR.REP.001 | Search a report | In the list of reports, select “Search” | The option to enter the search keyword shall be displayed | The search option is available | Pass |  |
|  |  |  | Enter the slide ID to search the report | The reports with the mentioned slide id shall be displayed.  | The reports with the slide id is displayed| Pass |  |
| UT.RPT.003 | UR.REP.001 | Filter the reports | In the list of reports, select "Filter”.  | The option to apply the filter criteria shall be displayed.  | The option to apply the filter criteria is displayed | Pass |  |
|  |  |  | Enter one or more filter criteria | The reports shall get filtered as per the filter criteria selected.  | The list gets filtered as per the applied filter criteria | Pass |  |
| UT.RPT.004 | UR.REP.001 | Bookmark a report | In the list of reports, for a report select the bookmark icon | The option to enter the comments to bookmark a report shall be displayed.  |The option to bookmark a report and add comments is available |Pass  |  |
|  |  |  | Add a comment and save | The report shall be bookmarked,  | The report is bookmarked | Pass |  |
| UT.RPT.005 | UR.REP.001 | Remove the bookmark for a report | In the list of reports, for a report that is already bookmarked, select the bookmark icon | The bookmark shall be removed for that report.|  The bookmark is removed | Pass |  |
| UT.RPT.006 | UR.REP.011 | Assign a report to review | Open a report | The report shall get opened | The report is opened | Pass |  |
|  |  |  | Select a reviewer from the dropdown | A conformation for report assignment shall be displayed | The confirmation to report assignemnt is displayed | Pass |  |
|  |  |  | Select "Re-assign" | The report shall get assigned to the selected reviewer | The report gets reassigned | Pass |  |
| UT.RPT.007 | UR.REP.011 | Unassign a report from a reviewer | Open an assigned report | The report shall get opened | The report gets opened |Pass  |  |
|  |  |  | Select the unassign icon | A confirmation for report unassignment shall be displayed.  |  The confirmation to unassign is displayed | Pass |  |
|  |  |  | Select "reassign" | The reviewer shall be unassinged froom the report| The reviewer is unassigned from the report | Pass |  |
| UT.RPT.008 | UR.REP.002 UR.REP.004 UR.REP.006 | View the results of a report | Open a report from the list of reports | The report shall get opened | The report gets opened |Pass  |  |
|  |  |  | Select "Slide info" | The details of the slide shall be displayed | The details of the slide info is displayed | Pass |  |
|  |  |  | Select "WBC" | The count and percentage of WBC cell types shall be displayed along with the patches | The count and percentage of WBC Cell types along with the patches are displayed | Pass |  |
|  |  |  | Select "RBC" | The grades of size, shape, colour and inclusions shall be displayed along with the patches | The RBC cell types adn the grades and the patches are displayed | Pass |  |
|  |  |  | Select "Platelets" | The count and morphology of the platelets shall be displayed along with the images.  | The count and morphology of the platelets are displayed | Pass |  |
| UT.RPT.009 | UR.REP.002 UR.REP.004 UR.REP.006 | View the patch images in a report | Select the patch view in WBC | The patch images of selected cell type shall be displayed |The patches of the selected cell types are displayed | Pass |  |
|  |  |  | Select the patch view in RBC (Size, shape, colour and inclusions) tab | The patch images of the selected cell type shall be displayed |The patches of RBCs are displayed  | Pass |  |
|  |  |  | Select the patch view in platelet morphology tab | The patch images of the selected cell type shall be displayed.  | The patches are displayed | Pass |  |
| UT.RPT.010 | UR.REP.002 UR.REP.004 UR.REP.006 | View the patches and the stitched images together | Select the split view in wbc/RBC/Platelet  tab (or) select a patch | The patches and the stitched image of the selected patch shall be displayed |The patches and the stitched images are displayed |Pass  |  |
| UT.RPT.011 | UR.REP.002 UR.REP.004 UR.REP.006 | View the stitched image | Select the microscopic view in WBC/RBC/Platelet  tab | The stitched image shall be displayed along with the annotations and the  list of selected cell type | The stitched image and the annotations are displayed | Pass |  |
| UT.RPT.012 | UR.REP.002 UR.REP.004 UR.REP.006 | Pan and Zoom the images | Select the microscopic view | The stitched image shall be displayed | The microscopic view is displayed | Pass |  |
|  |  |  | Select "Zoom in"  | The image shall get zoomed in | The image gets zoomed in | Pass |  |
|  |  |  | Select "Zoom out" | The image shall get zoomed out | The image gets zoomed out | Pass  |  |
|  |  |  | Select "Home" | The entire stitched image shall be displayed | The entire image is displayed but the image is not completely zoomed out | Fail | https://app.clickup.com/t/86cvdj2dm |
|  |  |  | Select an area on the image and move | The image shall get panned as per the movement made by the user.  | Pan all over the image is possibel |Pass |  |
| UT.RPT.013 | UR.REP.002 UR.REP.004 UR.REP.006 | Measure length in the stitched image | Select the Line tool in the stitched image | A line and the option to change the length of the line shall be  displayed. | A line is dislayed | Pass |  |
|  |  |  | Enter the size of the line between 5 and 20 microns with or without decimal | The line shall get extended or reduced as per the size mentioned, and the user shall be able to navigate this line throughout the stitched image. | The length of the line gets changed as per the entered number | Pass |  |
|  |  |  | Enter the size of the line below 5 or above 20 microns with or without decimal. | An error message indicating that the size is invalid shall be displayed.  | An error message is not displayed - only box is highlighted in red | Fail |https://app.clickup.com/t/86cvkkzn6  |
| UT.RPT.014 | UR.REP.002 UR.REP.004 UR.REP.006 | Measure diameter in the stitched image | Select the circle tool in the stitched image | A circle and the option to change the diameter of the circle shall be displayed.  | A circle is displayed |Pass  |  |
|  |  |  | Enter the size of the diameter between 5 and 20 microns with or without decimal | The circle shall get extended or reduced as per the size mentioned, and the user shall be able to navigate this circle throughout the stitched image. | The size of the circle gets changed as per the entered number | Pass |  |
|  |  |  | Enter the size of the circle below 5 or above 20 microns with or without decimal. | An error message indicating that the size is invalid shall be displayed.  | An error message is not displayed but the box is indicated with red | Pass |  |
| UT.RPT.015 | UR.REP.002 UR.REP.004 UR.REP.006 | View the area equivalent to 40x or 100x | Select "40x" from the option | A circle indicating the area equivalent to 40x shall be displayed and the user shall be able to move this circle throughout the stitched image.  | A 40x equivalent circle is displayed |Pass|  |
|  |  |  | Select "100x" from the option | A circle indicating the area equivalent to 100x shall be displayed and the user shall be able to move this circle throughout the stitched image.  | A 100x equivalent circle is displayed | Pass |  |
| UT.RPT.016 | UR.REP.002 UR.REP.003 | Review WBC differential count  | Open a self-assigned report | The report shall get opened | The report is opened|Pass |  |
|  |  |  | Select one or more patches of WBCs from a cell type and reclassify it to another cell type | The cells shall get classified from one type to another type and the visual cue shall be displayed.  | The cells are classified and the visual cue is displayed | Pass |  |
| UT.RPT.017 | UR\>REP.004 UR.REP.005 | Review RBC cells | Open a self-assigned report | The report shall get opened |The report is opened  | Pass |  |
|  |  |  | Modify the grades for one or more cell types | The grades shall get modified, and the visual cue shall be displayed.  | The RBC grade change is successful | Pass |  |
| UT.RPT.018 | UR.REP.006 UR.REP.007 | Review Platelet counts | Update the counts of N,M,G for one or more FOVs | The counts shall get updated and there shall be an undo option to reverse the changes | The counts gets modified and undo is also possible |Pass  |  |
| UT.RPT.019 | UR.REP.006 UR.REP.007  | Review Platelet morphology | Select one or more patches from a cell type and reclassify it to another cell type | The cells shall get classified from one type to another type and the visual cue shall be displayed.  | The cell gets classified from one type to another |Pass  |  |
| UT.RPT.020 | UR.REP.009 | Add PS impressions | Enter the PS impressions for  WBC Morphology RBC morphology Platelet morphology Hemoparasites Impressions | All the data entered shall be accepted and shall be reflected in the final report once approved.  | The entered data is reflected in the final report | Pass |  |
| UT.RPT.021 | UR.REP.010, UR.REP.013 | Approve a report with manual DC | In the summary of the report, select “Manual DC” | The values of calculated shall be copied to the column of manual DC | The values of calculated are copied in manual column | Pass |  |
|  |  |  | Enter the values  | The values entered shall be validated and accepted |The entered values are accepted  |Pass  |  |
|  |  |  | Select “Approve” | The approval process for the report shall get initiated | The report preview is displayed | Pass |  |
|  |  |  | Approve without adding images | The report shall get approved, and shall be submitted to LIMS (if configured) and the PDF of the report shall be generated.  |The report PDF is generated with images when approved without selecting images  | Fail | https://app.clickup.com/t/86cxp6dyc |
| UT.RPT.022 | UR.REP.014,  UR.REP.013 | Approve a report by adding supporting images | Select “Approve” in a self-assigned report | The approval process for the report shall get initiated.  | The preview of the report is displayed |Pass  |  |
|  |  |  | Select “Add supporting images.” | The options to add images for all the cell types shall be displayed as per the configured rules.  |The option to add the supporting images is displayed |Pass  |  |
|  |  |  | Modify the images for one or more cell types | The modified cell images shall be displayed in the preview | The modified images are displayed |Pass  |  |
|  |  |  | Select “Approve” | The report shall get approved and shall get submitted to LIMS (if connected) and the PDF report shall get generated.  |The report is approved and the PDF is generated  | Pass |  |
| UT.RPT.023 | UR.REP.010 | Reject a report | Select “Reject” and select "Confirm.” | The report shall get rejected and the PDF shall not be generated for rejected reports | The report is rejected and the PDF report is not generated | Pass |  |
| UT.RPT.024 | UR.REP.012 | View original and modified version of the report | Open a report that is modified.  | The report shall get opened | The report shall get opened |Pass  |  |
|  |  |  | Select”View original: | The original report that does not contain the user modifications shall be displayed | The original report without any changes is displayed | Pass |  |
|  |  |  | Select “View modified.” | The modified report that has the user modifications shall be displayed.  | The modified report is displayed | Pass |  |
| UT.RPT.025 | UR.REP.010 | Include or exclude Parameters in final report | In the preview of the report include or exclude  PS impressions RBC Platelets and approve the report | The report shall get approved and the PDF of the report shall be generated as per the selections made.  | When only RBC is included, everytime the PS impressions and the supporting images are added to the final report | Fail | https://app.clickup.com/t/86cxp6dyc |


## Product Lifecycle requirements

| Test case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.LIF.001 | UR.LIF.003 | Replace Oil and perform oil priming | Login to the device  | Login shall be successful | Login is successful |Pass  |  |
|  |  |  | Navigate to Maintenance | All the options that are available under maintenance shall be displayed | The remote connection, oil despenser, calibration are displayed | Pass |  |
|  |  |  | Select “Oil replacement” | The steps to replace oil pouch shall be displayed |The steps are displayed |Pass  |  |
|  |  |  | Follow the steps guided in the UI | The oil replacement shall be successful.  | Oil replacement is successful | Pass  |  |
| UT.LIF.002 | UR.LIF.003 | Perform oil priming | Login to the device  | Login shall be successful | Login is successful | Pass |  |
|  |  |  | Navigate to Maintenance | All the options that are available under maintenance shall be displayed |The remote connection, oil despenser, calibration are displayed  | Pass |  |
|  |  |  | Select “Oil priming” | The steps to perform priming  shall be displayed | The steps for oil priming is displayed |Pass  |  |
|  |  |  | Follow the steps guided in the UI | The priming shall be successful.  | The priming is successful | Pass |  |
| UT.LIF.003 | UR.LIF.003 | Initiate remote desktop connection | Navigate to Maintenance | All the options that are available under maintenance shall be displayed | The remote connection, oil despenser, calibration are displayed | Pass |  |
|  |  |  | Select “Remote connection” | The option to initiate remote connection shall be displayed | Able to initiate the remote connection | Pass |  |
|  |  |  | Select “Initiae” | The PIN and OTP shall be generated and the support member shall be able to access the device using the generated PIN and OTP.  | The PIN and OTP is generated | Pass |  |

# Results
|Bug |Count|
|--|--|
|No of highest priority bugs||
|No of high priority bugs||
|No of medium priority bugs||
|No of low priority bugs||

There are no high or highest priority bug orsafety related issues observed. The test is considered as Pass. 
