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
| Device ID | |
| Package version |  |

## Testers
|       |       |
| :---- | :---- |
| Number of testers | |
| Tester qualification |Adequately trained on the operations of the device and the reporting applicaiton| 

## Validation schedule

| |  |
| :---- | :---- |
| Estimated number of working days to execute validation |  | 
| Criteria to complete the validation |No High Priority bugs are observed and are open |

## Bug prioritization
All the bugs that are observed during the validation shall be prioritised considering the impact of the issue to the user and the probability of usage of the feature. The SOP is documented in the document - Work instruction- bugs workflow and fix timelines - Document Id:L3-DD-WIB-040-Workinstruction-Bugs workflow and fix timelines V2.0

## Requirements traceability

Each test case of this validation protocol is derived from a user requirement. Each test-case is linked to it's corresponding user requirement. The completeness of the flow-down of user requirements to test cases in this validation protocol has been reviewed and established.

# Test Cases

## General requirements 

| Test Case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.GEN.001 | UR.GEN.001 | Power on the device | Connect the power cord of the device to a recommended power source | The power cord shall get connected properly to the power source |  |  |  |
|  |  |  | Turn the power switch ON | The device shall be powered ON and the login page shall be displayed |  |  |  |
| UT.GEN.002 | UR.GEN.002 | Login to the device application with valid credentials | Enter a valid user name.  | The user name shall be accepted |  |  |  |
|  |  |  | Enter valid password | The entered password shall be accepted |  |  |  |
|  |  |  | Select "Sign in" | The login to the device shall be successful |  |  |  |
| UT.GEN.003 | UR.GEN.002 | Login to the device application with invalid credentials | Enter invalid user name | The user name shall be accepted |  |  |  |
|  |  |  | Enter an invalid password.  | The entered password shall be accepted |  |  |  |
|  |  |  | Select "Sign in" | The login to the device shall not  be successful and an error message indicating invalid login shall be displayed |  |  |  |
| UT.GEN.004 | UR.GEN.002 | Login to the reporting application with valid credentials | Open the Browser and enter the URL of the application | The application shall get opened and the login page shall be displayed.  |  |  |  |
|  |  |  | Enter a valid user name.  | The user name shall be accepted |  |  |  |
|  |  |  | Enter valid password | The entered password shall be accepted |  |  |  |
|  |  |  | Select "Sign in" | The login to the reporting application shall be successful |  |  |  |
| UT.GEN.005 | UR.GEN.002 | Login to the reporting  application with invalid credentials | Open the Browser and enter the URL of the application | The application shall get opened and the login page shall be displayed.  |  |  |  |
|  |  |  | Enter invalid user name | The user name shall be accepted |  |  |  |
|  |  |  | Enter an invalid password.  | The entered password shall be accepted |  |  |  |
|  |  |  | Select "Sign in" | The login to the reporting application shall not  be successful and an error message indicating invalid login shall be displayed |  |  |  |
| UT.GEN.006 | UR.GEN.004 | Logout of the device application | Select the user profile icon present in the toolbar | The following user profile options shall be displayed. Tiem zone Change password Logout  |  |  |  |
|  |  |  | Select “Logout” | The user shall be logged out of the device. If there are any system operations in process, then those shall get terminated.  |  |  |  |
| UT.GEN.007 | UR.GEN.004 | Logout of the reporting application | Select the user profile icon present in the list report page | The following user profile options shall be displayed. Tiem zone Change password Logout  |  |  |  |
|  |  |  | Select “Logout” | The user shall be logged out of the application.  |  |  |  |
| UT.GEN.008 | UR.GEN.005 | Connect the device to the network using WIFI | Select the WIFI icon | The list of networks available for connection shall be displayed |  |  |  |
|  |  |  | Select a network from the list | The option to enter the password to connect to the network shall be displayed |  |  |  |
|  |  |  | Enter the password | The entered password shall be validated, and the device shall be connected to the selected network. This network shall be remembered by the system and shall get reconnected.  |  |  |  |
| UT.GEN.009 | UR.GEN.005 | Connect the device to a network using ethernet | Connect an ethernet cable to the device | The system shall detect the connection and connect to the network automatically.  |  |  |  |
| UT.GEN.010 | UR.GEN.005 | Connect an external display to the system | Connect an external monitor to the device through the HDMI port | The user shall be able to perform the reporting and the admin activities by accessing the application from the monitor.  |  |  |  |
| UT.GEN.011 | UR.GEN.005 | Connect to external input peripherals | Connect an external mouse and keyboard to the device | The user shall be able to provide inputs on the UI using the external mouse and keyboard.  |  |  |  |
| UT.GEN.012 | UR.GEN.001 | Power off the device | Select the power menu | The following power menu options shall be displayed Shutdown Restart |  |  |  |
|  |  |  | Select "Shutdown" | The system shall get powered off, and all the system operations (if any) shall be terminated.  |  |  |  |
| UT.GEN.013 | UR.GEN.001 | Restart the device | Select the power menu | The following power menu options shall be displayed Shutdown Restart |  |  |  |
|  |  |  | Select "Restart" | The system shall get restarted, and all the system operations (if any) shall be terminated before the system powers off.  |  |  |  |

## Scanning Requirements

| Test Case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.SCN.001 | UR.SCN.001 | Place the slides on the tray and  | Load the slides onto the tray | The slides shall be placed onto the tray without popout or breakage.  |  |  |  |
| UT.SCN.002 | UR.SCN.002 | Place the tray into the system. | Load the tray onto the device | The tray shall be placed in the device without any popout or breakage of the slide.  |  |  |  |
| UT.SCN.003 | UR.SCN.003 | View the decoded barcode information | Place the loaded tray into the system and select confirm | The barcode of the slides shall be captured and decoded by the system and shall be populated in the slide creation page |  |  |  |
| UT.SCN.004 | UR.SCN.004 | Enter/update the slide ID of the slide.  | Select the slide ID field | The slide ID field shall be editable, and the keypad shall be populated. The preview of the barcode region of the slide shall be displayed.  |  |  |  |
|  |  |  | Enter the slide ID | The entered details shall be validated and accepted |  |  |  |
| UR.SCN.005 | UR.SCN.006, UR.SCN.008 | Initiate the scans for the loaded slides | Select “Next” from the slide details page | The scan shall get initiated for the slides loaded in the tray after oil is dispensed.  |  |  |  |
|  |  |  | View the on-going scans | The progress and the status of scans for each slide, along with the warning and order status, shall be displayed. The scan summary shall be displayed along with the exceptions (if any) and the tray shall be ejected |  |  |  |
|  |  |  | Remove the tray and mark as "Done.” to finish the scans or “Insert another tray” to scan another tray of slides.  | The tray shall be taken back to the home position if “Done” is selected, or the slide insertion page shall be displayed if “Insert another tray” is selected.  |  |  |  |
| UT.SCN.006 | UR.SCN.007 | Abort the scans for one or more slides | Initiate the scans for a tray | The scans shall get initiated and the system shall capture the images |  |  |  |
|  |  |  | Select “Abort scans” | The option to abort either all queued scans or on-going scans shall be displayed |  |  |  |
|  |  |  | Select “Abort scans for all queued slides.” | All the slides that are in queue for scanning shall be aborted and the status shall get changed to aborted |  |  |  |
|  |  |  | Select “Abort scans” | The option to abort either all queued scans or on-going scans shall be displayed |  |  |  |
|  |  |  | Select “Abort scans for the in-progress slide” | The slide that is in the process of capturing the images shall be aborted, and the status shall get changed to aborted.  |  |  |  |
| UT.SCN.007 | UR.SCN.009 | View the history of scanned slides | Select "History" | The list of slides that were scanned on the device shall be displayed along with the status and the timestamp of scanning |  |  |  |
|  |  |  | Select the filter criteria as  Days Status	 | The list shall get filtered as per the criteria applied.  |  |  |  |

## Review and reporting requirements

| Test case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.RPT.001 | UR.REP.001 | View the list of reports | Login to the reporting application with valid credentials | The login shall be successful and the list of reports shall be displayed as  To be reviewed Preparing Reviewed  |  |  |  |
| UT.RPT.002 | UR.REP.001 | Search a report | In the list of reports, select “Search” | The option to enter the search keyword shall be displayed |  |  |  |
|  |  |  | Enter the slide ID to search the report | The reports with the mentioned slide id shall be displayed.  |  |  |  |
| UT.RPT.003 | UR.REP.001 | Filter the reports | In the list of reports, select "Filter”.  | The option to apply the filter criteria shall be displayed.  |  |  |  |
|  |  |  | Enter one or more filter criteria | The reports shall get filtered as per the filter criteria selected.  |  |  |  |
| UT.RPT.004 | UR.REP.001 | Bookmark a report | In the list of reports, for a report select the bookmark icon | The option to enter the comments to bookmark a report shall be displayed.  |  |  |  |
|  |  |  | Add a comment and save | The report shall be bookmarked,  |  |  |  |
| UT.RPT.005 | UR.REP.001 | Remove the bookmark for a report | In the list of reports, for a report that is already bookmarked, select the bookmark icon | The bookmark shall be removed for that report.  |  |  |  |
| UT.RPT.006 | UR.REP.011 | Assign a report to review | Open a report | The report shall get opened |  |  |  |
|  |  |  | Select a reviewer from the dropdown | A conformation for report assignment shall be displayed |  |  |  |
|  |  |  | Select "Re-assign" | The report shall get assigned to the selected reviewer |  |  |  |
| UT.RPT.007 | UR.REP.011 | Unassign a report from a reviewer | Open an assigned report | The report shall get opened |  |  |  |
|  |  |  | Select the unassign icon | A confirmation for report unassignment shall be displayed.  |  |  |  |
|  |  |  | Select "Re-assign" | The reviewer shall be unassinged froom the report,  |  |  |  |
| UT.RPT.008 | UR.REP.002 UR.REP.004 UR.REP.006 | View the results of a report | Open a report from the list of reports | The report shall get opened |  |  |  |
|  |  |  | Select "Slide info" | The details of the slide shall be displayed |  |  |  |
|  |  |  | Select "WBC" | The count and percentage of WBC cell types shall be displayed along with the patches |  |  |  |
|  |  |  | Select "RBC" | The grades of size, shape, colour and inclusions shall be displayed along with the patches |  |  |  |
|  |  |  | Select "Platelets" | The count and morphology of the platelets shall be displayed along with the images.  |  |  |  |
| UT.RPT.009 | UR.REP.002 UR.REP.004 UR.REP.006 | View the patch images in a report | Select the patch view in WBC | The patch images of selected cell type shall be displayed |  |  |  |
|  |  |  | Select the patch view in RBC (Size, shape, colour and inclusions) tab | The patch images of the selected cell type shall be displayed |  |  |  |
|  |  |  | Select the patch view in platelet morphology tab | The patch images of the selected cell type shall be displayed.  |  |  |  |
| UT.RPT.010 | UR.REP.002 UR.REP.004 UR.REP.006 | View the patches and the stitched images together | Select the split view in wbc/RBC/Platelet  tab (or) select a patch | The patches and the stitched image of the selected patch shall be displayed |  |  |  |
| UT.RPT.011 | UR.REP.002 UR.REP.004 UR.REP.006 | View the stitched image | Select the microscopic view in WBC/RBC/Platelet  tab | The stitched image shall be displayed along with the annotations and the  list of selected cell type |  |  |  |
| UT.RPT.012 | UR.REP.002 UR.REP.004 UR.REP.006 | Pan and Zoom the images | Select the microscopic view | The stitched image shall be displayed |  |  |  |
|  |  |  | Select "Zoom in"  | The image shall get zoomed in |  |  |  |
|  |  |  | Select "Zoom out" | The image shall get zoomed out |  |  |  |
|  |  |  | Select "Home" | The entire stitched image shall be displayed |  |  |  |
|  |  |  | Select an area on the image and move | The image shall get panned as per the movement made by the user.  |  |  |  |
| UT.RPT.013 | UR.REP.002 UR.REP.004 UR.REP.006 | Measure length in the stitched image | Select the Line tool in the stitched image | A line and the option to change the length of the line shall be  displayed.  |  |  |  |
|  |  |  | Enter the size of the line between 5 and 20 microns with or without decimal | The line shall get extended or reduced as per the size mentioned, and the user shall be able to navigate this line throughout the stitched image. |  |  |  |
|  |  |  | Enter the size of the line below 5 or above 20 microns with or without decimal. | An error message indicating that the size is invalid shall be displayed.  |  |  |  |
| UT.RPT.014 | UR.REP.002 UR.REP.004 UR.REP.006 | Measure diameter in the stitched image | Select the circle tool in the stitched image | A circle and the option to change the diameter of the circle shall be displayed.  |  |  |  |
|  |  |  | Enter the size of the diameter between 5 and 20 microns with or without decimal | The circle shall get extended or reduced as per the size mentioned, and the user shall be able to navigate this circle throughout the stitched image. |  |  |  |
|  |  |  | Enter the size of the circle below 5 or above 20 microns with or without decimal. | An error message indicating that the size is invalid shall be displayed.  |  |  |  |
| UT.RPT.015 | UR.REP.002 UR.REP.004 UR.REP.006 | View the area equivalent to 40x or 100x | Select "40x" from the option | A circle indicating the area equivalent to 40x shall be displayed and the user shall be able to move this circle throughout the stitched image.  |  |  |  |
|  |  |  | Select "100x" from the option | A circle indicating the area equivalent to 100x shall be displayed and the user shall be able to move this circle throughout the stitched image.  |  |  |  |
| UT.RPT.016 | UR.REP.002 UR.REP.003 | Review WBC differential count  | Open a self-assigned report | The report shall get opened |  |  |  |
|  |  |  | Select one or more patches of WBCs from a cell type and reclassify it to another cell type | The cells shall get classified from one type to another type and the visual cue shall be displayed.  |  |  |  |
| UT.RPT.017 | UR\>REP.004 UR.REP.005 | Review RBC cells | Open a self-assigned report | The report shall get opened |  |  |  |
|  |  |  | Modify the grades for one or more cell types | The grades shall get modified, and the visual cue shall be displayed.  |  |  |  |
| UT.RPT.018 | UR.REP.006 UR.REP.007 | Review Platelet counts | Update the counts of N,M,G for one or more FOVs | The counts shall get updated and there shall be an undo option to reverse the changes |  |  |  |
| UT.RPT.019 | UR.REP.006 UR.REP.007  | Review Platelet morphology | Select one or more patches from a cell type and reclassify it to another cell type | The cells shall get classified from one type to another type and the visual cue shall be displayed.  |  |  |  |
| UT.RPT.020 | UR.REP.009 | Add PS impressions | Enter the PS impressions for  WBC Morphology RBC morphology Platelet morphology Hemoparasites Impressions | All the data entered shall be accepted and shall be reflected in the final report once approved.  |  |  |  |
| UT.RPT.021 | UR.REP.010, UR.REP.013 | Approve a report with manual DC | In the summary of the report, select “Manual DC” | The values of calculated shall be copied to the column of manual DC |  |  |  |
|  |  |  | Enter the values  | The values entered shall be validated and accepted |  |  |  |
|  |  |  | Select “Approve” | The approval process for the report shall get initiated |  |  |  |
|  |  |  | Approve without adding images | The report shall get approved, and shall be submitted to LIMS (if configured) and the PDF of the report shall be generated.  |  |  |  |
| UT.RPT.022 | UR.REP.014,  UR.REP.013 | Approve a report by adding supporting images | Select “Approve” in a self-assigned report | The approval process for the report shall get initiated.  |  |  |  |
|  |  |  | Select “Add supporting images.” | The options to add images for all the cell types shall be displayed as per the configured rules.  |  |  |  |
|  |  |  | Modify the images for one or more cell types | The modified cell images shall be displayed in the preview |  |  |  |
|  |  |  | Select “Approve” | The report shall get approved and shall get submitted to LIMS (if connected) and the PDF report shall get generated.  |  |  |  |
| UT.RPT.023 | UR.REP.010 | Reject a report | Select “Reject” and select "Confirm.” | The report shall get rejected and the PDF shall not be generated for rejected reports |  |  |  |
| UT.RPT.024 | UR.REP.012 | View original and modified version of the report | Open a report that is modified.  | The report shall get opened |  |  |  |
|  |  |  | Select”View original: | The original report that does not contain the user modifications shall be displayed |  |  |  |
|  |  |  | Select “View modified.” | The modified report that has the user modifications shall be displayed.  |  |  |  |
| UT.RPT.025 | UR.REP.010 | Include or exclude Parameters in final report | In the preview of the report include or exclude  PS impressions RBC Platelets\\ And approve the report | The report shall get approved and the PDF of the report shall be generated as per the selections made.  |  |  |  |
|  |  |  |  |  |  |  |  |

## Product Lifecycle requirements

| Test case ID | User requirement ID | Use case | Test step | Expected result | Actual result | Status | Defect(s) |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| UT.LIF.001 | UR.LIF.003 | Replace Oil and perform oil priming | Login to the device  | Login shall be successful |  |  |  |
|  |  |  | Navigate to Maintenance | All the options that are available under maintenance shall be displayed |  |  |  |
|  |  |  | Select “Oil replacement” | The steps to replace oil pouch shall be displayed |  |  |  |
|  |  |  | Follow the steps guided in the UI | The oil replacement shall be successful.  |  |  |  |
| UT.LIF.002 | UR.LIF.003 | Perform oil priming | Login to the device  | Login shall be successful |  |  |  |
|  |  |  | Navigate to Maintenance | All the options that are available under maintenance shall be displayed |  |  |  |
|  |  |  | Select “Oil priming” | The steps to perform priming  shall be displayed |  |  |  |
|  |  |  | Follow the steps guided in the UI | The priming shall be successful.  |  |  |  |
| UT.LIF.003 | UR.LIF.003 | Initiate remote desktop connection | Navigate to Maintenance | All the options that are available under maintenance shall be displayed |  |  |  |
|  |  |  | Select “Remote connection” | The option to initiate remote connection shall be displayed |  |  |  |
|  |  |  | Select “Initiae” | The PIN and OTP shall be generated and the support member shall be able to access the device using the generated PIN and OTP.  |  |  |  |

# Dates and Signatures

The evaluators agree with the contents of this protocol. 

| Person | Designation | Role |
| :---- | :---- | :---- |
| Raamki K L | Product Manager | Author |
| Pratik Doshi | Group Product Manager | Reviewer |
| Dr.Selvarasu Sellappan | Director-QCRA | Reviewer |
| Apurv Manjrekar | Chief Product Officer | Approver |

# Acceptance Criteria
|Parameter|Criteria|
|---------|--------|
|No of high\highest prioirty Bugs| 0|
|No of safety issues reported|0|

# Adverse device events
The study is considered a very LOW risk validation. The Sponsor must immediately conduct an evaluation of all low-risk events and must report the results of the evaluation  to the
concerned regulatory bodies, after the sponsor ﬁrst receives notice of the eﬀect.
The following are the Low-risk events which may occur:
- Electric Shock
- Device breakdown
- Issues with scanning and results reported by the device
- Slide breakage

# Monitoring Plan 
## Device health
- The system qualiﬁcation shall be performed at speciﬁed intervals and recorded
- Each instance of system downtime shall be recorded and analyzed.
- Each instance of slide breakage inside the system shall be recorded and analyzed.
- The study shall be immediately paused for validation, if any adverse event is encountered

## Data Integrity
 The data traceability for each data point in the validation shall be checked periodically
# Accountability
## Site Laboratory
1. The laboratory shall provide a safe area for the Sponsor to store the slides during the validation

## Sponsor
1. The sponsor shall ensure that the operators are adequately trained before the validation begins.
2. The sponsor shall manage the traceability to the data.
3. The sponsor shall analyze the data and share the results for review with the appropriate authorities.

# Documentation
1. User manual
2. Adverse event form