# ShaderGraph-UI-Masking-Fixer
A fixer for UI Masking ShaderGraph-generated shaders in Unity 2020.x

![usage](https://github.com/user-attachments/assets/6c716b17-9000-4d94-a32a-8f71ce1bb416)

Original discussion thread on [Unity Discussions](https://discussions.unity.com/t/ui-mask-not-working/803565), adapted & modified by Xeraclom14 (https://twitter.com/Xeraclom14).
If you're here, you may have noticed that masking doesn't really work when using sprite shaders generated from ShaderGraph.
This script adds a few lines to the generated shader code to enable stencil shenanigans, (hopefully) making masking work.

Installation:
Copy the FBXAnimationClipOrganizer.cs script into Scripts\Editor.
 
Usage:
1) To open, go to Window -> ShaderGraph UI Masking Fixer.
2) Select the desired shader made in ShaderGraph in the inspector.
3) Click the "Copy Shader" button in the inspector.
4) Click the "Load from clipboard" button.
5) Optionally change the path and/or file name where the fixed shader will be generated.
6) Click "Save to file" to generate the fixed shader file.
7) Go to each affected material with the old shader and change it for the new, fixed one.
8) Yep.

Example of a bad shader with masking not working (the icon inside it is a regular sprite, masking works):
![bad_mask](https://github.com/user-attachments/assets/756f5c68-0012-4683-8029-d970a1257b07)

Example of the same, but fixed shader:
![good_mask](https://github.com/user-attachments/assets/bec6af51-d00f-4596-a57f-dedb89284970)

Enjoy!
