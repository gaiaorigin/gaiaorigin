Custom versions of the addon ZIP were created, due to the 100MB file size limit imposed on free GitHub repos. The Elementum All-In-One package exceeds the 100MB limit and can therefore not be added to the repo, otherwise GitHub will limit the monthly bandwidth of the repo and require the installtion of Git LFS.

The individual platform/architecture packages can also not be added to the repo. When Kodi has automatic addon updates enabled (by default), it will update the Elementum addon with the FIRST platform/architecture version in the list, instead of using the platform/architecture from the user's first installation. For instance, if you install the "linux_x64" version, on reboot Kodi will replace this version with "android_arm", since it is the first item in the list. Kodi cannot distinguish between versions that contain a word after the last ".".

The versions in Gaia's repo are a copy of the All-In-One package with the following changes:
  1. One version for each OS was created: Windows, Linux, Mac, Adnroid.
  2. The executables in the "bin" directory that are not compatible with the current OS were deleted to reduce the ZIP file size.
  3. In "addon.xml" the Elementum addon version was changed for each OS.
  4. In "addon.xml" the <platform> tag was updated for each OS.
