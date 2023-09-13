# HDRToggle
Simply toggles HDR on Windows 11 when executed.

## Why?
This is primarily to be used with Sunshine so that on launching a stream, HDR is disabled which prevents washed out/overly bright colors when streaming to a non-HDR display. When exiting the stream, the toggle can be triggered automatically again re-enabling it.

## How?
This was done by simply creating an auto hotkey profile to press the key combination to toggle HDR in Windows 11: `Windows + Alt + b`. Since auto hotkey can also compile the script as an executable, I did that too so that AHK doesn't need to be installed on the host. If you don't trust precompiled executables (which you shouldn't), feel free to do the same with the provided AHK script.

## Using With Sunshine
To use with Sunshine, simply download/compile the executable somewhere and put the following in BOTH the `Do` and `Undo` commands:
```
cmd /c "<PATH\TO\EXE>\toggle_hdr.exe"
```
You can select `Elevated` if you get permission issues.
