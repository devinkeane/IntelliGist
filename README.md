
<table style="width: 100%;">
  <tr>
    <td style="text-align: left;">
      <img src="https://user-images.githubusercontent.com/12550831/235322400-fd10dd77-9d79-4813-9b56-873ff6c1a15e.png" alt="Alt Text" width="300">
    </td>
    <td style="text-align: right;">
      <img src="https://user-images.githubusercontent.com/12550831/235329063-7e8cd259-919c-4096-aef4-218a34da4056.png" width="550">
    </td>
  </tr>
</table>

---

IntelliGist is a Mac application that elegantly and cohesively summarizes any .pdf input of any research paper of any length. This is achieved despite the context length limits of GPT. Unlike other apps which claim to do the same thing, the end result is not simply a concatenation of smaller summaries. Rather, mixed AI techniques and utilities are used to generate one solid final essay of around 500 words that reflects the structure of the paper.

The program is free of charge, but to use the beta version, you must use your own API key generated from your OpenAI account, which you can easily insert into your own config.ini file and place into the appropriate directory.

---

## Setting up the config.ini file

1. Create a new plain text file named `config.ini`.
2. Copy and paste the following content into the file:

```
[openai]
api_key = <YOUR_OPENAI_API_KEY>
```

Replace `<YOUR_OPENAI_API_KEY>` with your actual OpenAI API key, which you can obtain from the OpenAI website.

3. **Important:** Make sure there are no extra characters or new lines after the content.

---

## Placing the config.ini file in the application package

1. Locate the `IntelliGist.app` file in Finder.
2. Right-click on `IntelliGist.app` and select "Show Package Contents".
3. Open the "Contents" folder, then open the "Resources" folder.
4. Drag and drop your `config.ini` file into the "Resources" folder.

---

## Installing and running the application

1. Drag the `IntelliGist.app` file to your "Applications" folder.
2. To launch the application, double-click on `IntelliGist.app` in the "Applications" folder or the original location where you placed the config file.

---

## Allowing the app to run on your Mac

Before you can run the application for the first time, you may need to allow your Mac to open it:

Attempt to open the IntelliGist.app by double-clicking it.
If a warning appears saying that the app cannot be opened, go to "System Preferences" on your Mac:
* Click on "Security & Privacy".
    * In the "General" tab, you should see a message about the blocked app.
    * Click on "Open Anyway" to allow the app to run.

If you encounter an error saying "IntelliGist is damaged and can't be opened", follow these steps:
1. Open the Terminal app (you can find it in Applications > Utilities).
2. Type the following command and press Enter:

   `xattr -cr /path/to/your/app`

   Replace `/path/to/your/app` with the actual path to the downloaded app. You can find the path by right-clicking on the app and choosing "Get Info", or you can simply drag and drop the app onto the Terminal window after typing `xattr -cr ` (with a space at the end).

3. After running the command, you should be able to open the app without the error message.

Now you're ready to generate an intelligent "gist" of any research paper of any length and of any detail!

---

<pre>
<span style="color: red;">              _                   __                                ,     ,</span>
<span style="color: blue;">             / )  / _ _       /  (     __/_ _   _                  (\____/)</span>
<span style="color: green;">  (c) 2023  (__(/()(-/ /)(//)/( __)(/_) /(-//)_)    L L C           (_oo_)</span>
<span style="color: orange;">               /      /            /                                  (O)</span>
<span style="color: purple;">                                                                    __||__    \)    </span>
<span style="color: brown;">                                                                 []/______\[] /</span>
<span style="color: red;">                                                                 / \______/ \/</span>
<span style="color: blue;">                                                                /    /__\         </span>
<span style="color: green;">                                                               (\   /____\</span>
</pre>
