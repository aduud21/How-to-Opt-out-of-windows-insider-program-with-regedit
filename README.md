# ⚠️ Take caution upon following this tutorial, Do not just randomly delete, edit or add REGEDIT keys as it can make your system instable (bsod) ⚠️
### OS TESTED: Microsoft Windows 11 (On Real Hardware)
# Steps
1. Win+R or type "Run" (without the quotes)
2. Open "regedit" (enter regedit in the textbox)
3. Go to `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\Applicability`
4. if `EnablePreviewBuilds` is set to `1` then set it to `0`
5. Open Settings > Windows Update > Windows insider program, Once there, it should say "Get started", if it says that then you successfully opt-outed!
  
# Optional:
After opt-out, you can as well leave the progam for good here
https://www.microsoft.com/en-us/windowsinsider/leave-program

# To hide the Windows insider page
1. Follow step 1,2 (above)
2. Go in `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsSelfHost\UI\Visibility`
3. Create a new `DWORD (32-bit) value`
4. Name the DWORD `HideInsiderPage`
5. Change the value from `0` to `1`
