# ucExplorer

Beta 0.9 now available
The control is now configured to build an ocx. The old test form is now in ucExplorerWithTestForm.twinproj. Corrected the version info failure bug making the control think it was on XP. 

ucExplorer is now entering alpha testing. The initial feature set is complete, and it's loading to the correct startup path, and the implemented interfaces are being called without raising errors in their default state. The selection changed events are successfully listing files, and the navigation event is successfully reporting new paths. There's a lot of features still to test.

Update: Alpha 0.2 fixes filtering not working when set in design mode, and adds a SetColumns method and a GetCurrentView method for getting the interfaces yourself. Also enables sizing the test form (sizing was working fine, just wasn't enabled). 
