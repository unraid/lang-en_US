# lang-en_US

### READ THIS WHEN YOU WANT TO MAKE TRANSLATIONS TO ANOTHER LANGUAGE

There are sixteen text files included in this repository, each with their own section of translations:

<pre>
- <strong>translations.txt</strong>     -- these are <strong>general</strong> translations, used in many sections
- <strong>helptext.txt</strong>         -- these are translations for the <strong>Help</strong> section
- <strong>dashboard.txt</strong>        -- these are translations for the <strong>Dashboard</strong> section
- <strong>main.txt</strong>             -- these are translations for the <strong>Main</strong> section
- <strong>shares.txt</strong>           -- these are translations for the <strong>Shares</strong> section
- <strong>users.txt</strong>            -- these are translations for the <strong>Users</strong> section
- <strong>settings.txt</strong>         -- these are translations for the <strong>Settings</strong> section
- <strong>plugins.txt</strong>          -- these are translations for the <strong>Plugins</strong> section
- <strong>docker.txt</strong>           -- these are translations for the <strong>Docker</strong> section
- <strong>vms.txt</strong>              -- these are translations for the <strong>VMs</strong> section
- <strong>tools.txt</strong>            -- these are translations for the <strong>Tools</strong> section
- <strong>javascript.txt</strong>       -- these are translations for <strong>JavaScript</strong> scripts
- <strong>scripts.txt</strong>          -- these are translations for <strong>Local Scripts</strong>
- <strong>apps.txt</strong>             -- these are translations for the <strong>App</strong> section <em>(CA = Community Applications)</em>
- <strong>ca_settings</strong>          -- these are translations for the <strong>App Settings</strong> <em>(CA)</em>
- <strong>javascript.ca.txt</strong>    -- these are translations for the <strong>JavaScript Scripts</strong> referred to <em>CA</em> section
</pre>

All file names are in lowercase and <strong>must be included in the repository</strong> to make the translations complete.

Removing a particular file means no translations will be available for that section and the Graphical User Interface *(GUI)* will display text in the original English.

### TRANSLATIONS

Each text file contains regular text strings stored in UTF-8 format with Linux line endings.
Use a text editor that supports UTF-8 and Linux line endings, like [Notepad++](https://notepad-plus-plus.org/downloads).

The content of each text file is separated into two parts:


### PART 1

These are single line entries which are in the format:

<pre>original English text=translated Foreign text</pre>

Only modify the text after the equal sign **(=)** and leave the original English text at the left untouched.
Removing a line or omitting a translation after the equal sign, results in the *GUI* displaying this line with the original English text.

The translated text may have “special characters”, such as *slashes*, *parenthesis* or *brackets* which are not included in the key text,
but which are used to display text accordingly. 
E.g.:

<pre>Options see Help=Options (see Help)</pre>

The characters \* and \*\* are used to display text in *italics* and **bold** respectively. 
E.g.:

"Array must be Stopped to change=*Array* must be **Stopped** to change".

It is recommended to translate per section — that is, one file at a time — and verify the correctness of the translations in the *GUI*
before proceeding with the next section.

Keep in mind the length of the translations and try to make them similar length as the original text and avoid space issues in the *GUI*.


### PART 2

These are multi line entries used to translate multiple lines at once.
Multi line translations have a unique opening and closing tag:

**:unique_tag_name_plug:** - unique opening tag used for any multi line text section

**:end**    - closing tag

⚠️ Do not remove or alter these tags and **only translate** the text between the opening and closing tags!


### HELP TEXT

All help text of the *GUI* is stored in a single file **helptext.txt**.

This file has multiple help text sections. 
Each section is enclosed by a unique opening tag and corresponding closing tag:

**:unique_tag_name_help:** - unique opening tag used for a help text section

**:end**    - corresponding closing tag

⚠️ Do not remove or alter these tags; **only translate** the text between the opening and closing tags!

NOTE: *Markdown* styling syntax is used. This must be preserved.


### LOCAL TESTING

Once the translations are complete and you want to test locally the (intermediate) results, the text files need to be **zipped into a single ZIP file**.

Give the ZIP file the name of your language, e.g.: "**Italian.zip**".

In the Unraid *GUI* go to: **Tools -> webGUI -> Language** (*switch to Developer view*)

- By default only the English language is installed (built-in).
- Choose the ZIP file you have created earlier as the source file.
- If the language name is recognized, it will be automatically selected; otherwise choose the language from the dropdown menu to install.
- Click "Upload" to add your translations to the *GUI* under the selected language name.

NOTE: If your language is not available from the dropdown menu, please make a request on the [Multi-Language Thread in Unraid Forum](https://forums.unraid.net/forum/75-multi-language-section/)

Now your language is available for local testing!

In the Unraid *GUI* go to: **Settings -> Display Settings -> Language**

- Select the preferred language from the dropdown menu. Note that only the available language choices are displayed here.


### GITHUB

A *language repository* will be made available at [GitHub](https://github.com/unraid), where translators can create *Pull Requests (PR)* and submit their work.

Once you are satisfied with your results, use *GitHub* (an account is required) to *fork* the respective language repository and create a *PR* with your modifications.

**Limetech** will review this and merge your work when approved.


### UPDATES

When updated source text files in English become available in the future, these updates will be made available through *GitHub*.

Translators can use the *GitHub* system to see which changes are made and update their translations accordingly.


### CREDITS

Your efforts are much welcomed and to show our appreciation, your name and language are credited on the **Credits page** under **Tools** in the *Unraid GUI*.

Please let us know which credentials to use.

Thank you for your collaboration and commitment ❤️
