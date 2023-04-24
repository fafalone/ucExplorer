# ucExplorer

ucExplorer is an Active-X control wrapper for the IExplorerBrowser object, which allows you to host an Explorer window on your form with options for interaction and configuration. This control is being built in [twinBASIC](https://twinbasic.com/), a 100% compatible successor to VB6, and can be used in tB, VB6, VBA6, VBA7 x87, VBA7 x64, and even Windows Forms in .NET. 

You should use the [most recent build](https://github.com/twinbasic/twinbasic/releases) of twinBASIC to build it yourself. If you intend to use it in VB6, be sure to run as admin when building and enable the 'Register to HKEY_LOCAL_MACHINE' option in project settings.

### Updates

4/24 Beta 0.9.3 fixes the sizing issue on scaled displays and attempts to address crash-on-close issue.

4/23 afternoon: OCXs updated to address small bug where GetCurrentView did not return all options. OCX test app has been updated to display selection and size the control; tbcontrol-version test app updated to sync code to master. Also confirmed ocx is working (both x86/x64) in tB, next step is to test in VB6 and VBA. Then .NET.

4/23 morning: I've added a test app for the compiled OCX, and compiled OCXs. Note that if you're not building the OCXs yourself, they'll need to be registered, there's currently reg-free sxs, though I will add a manifest for that at some point.

---

Beta 0.9.2 now available, this makes some final code cleanup and settings adjustments before build testing. Once I've confirmed it works in at least some hosts I'll post compiled OCX builds to Releases as well. 


Beta 0.9.1: The control is now configured to build an ocx. The old test form is now in ucExplorerWithTestForm.twinproj. Corrected the version info failure bug making the control think it was on XP. 

ucExplorer is now entering alpha testing. The initial feature set is complete, and it's loading to the correct startup path, and the implemented interfaces are being called without raising errors in their default state. The selection changed events are successfully listing files, and the navigation event is successfully reporting new paths. There's a lot of features still to test.

Update: Alpha 0.2 fixes filtering not working when set in design mode, and adds a SetColumns method and a GetCurrentView method for getting the interfaces yourself. Also enables sizing the test form (sizing was working fine, just wasn't enabled). 

![Screenshot](https://i.imgur.com/EEt3D8F.jpg)
