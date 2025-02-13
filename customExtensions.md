## How to add custom extensions to ExtPrint3r
> [!WARNING]
> If this guide fails for you do not make an issue on it, this is only for advanced users.

### Step 1.<br>
First, you must find the extension's ID. To do this go to `chrome://extensions` and click on the extension of choice. Then look for the ID and copy it.<br>
![image](https://github.com/user-attachments/assets/2846982e-d22b-4b38-acad-45d465e7c24f)<br>
If the ID doesn't show up like on the image above, you can also find it in the URL.

### Step 2.<br>
Once you have the extension's ID, open the following link: `chrome-extension://id-here/manifest.json` (replace "id-here" with the ID you got earlier) Once you are in the page you have to find a web accessible resource with an explicit file name. These are typically near the bottom of the page. You'll want to look for something like this:<br>
![image](https://github.com/user-attachments/assets/de656ecf-ea46-4b5a-a7b5-c0a00c749126)

### Step 3.<br>
You can now copy any of the resources and replace the `manifest.json` part of the URL with your resource. Then go to the URL and confirm that it works, since if it doesn't you'll have to go back to step 2 and use a different resource.

### Step 4.<br>
Congrats! You can now enable developer mode from settings and add a temporary extension. Use this web accessible resource URL when you are prompted for it. You can also make a pull request on [this repository](https://github.com/Blobby-Boi/ExtPrint3r) for it to be added permanently.
