# Outlook URL handler

- A script to copy an Outlook Email message as a Markdown link
- An `info.plist` file for use in Alfred, which maps Command-Shift-C to that script
- a submodule from `acidx` that registers an `outlook://<message_number>` URL handler.

# Installation

```
git clone --recurse-submodules https://github.com/darrenpmeyer/outlook_url_handler.git 
cd outlook_url_handler
cp -rp OutlookURLHandler/OutlookURLHandler.app /Applications

mkdir -p ~/Library/Scripts/Applications/Microsoft/Outlook/
cp "Copy Outlook Email Link as Markdown.scpt" ~/Library/Scripts/Applications/Microsoft/Outlook/
```

Open the `/Applications` folder in Finder, right-click `OutlookURLHandler.app` and select `Open`. Confrim that you wish to open the application even though it is unsigned. This will register the URL handler.

# Use

After all install steps are completed, when an email message is selected in Outlook, press Command-Shift-C. A Markdown-formatted link with the subject of the email as the link text will be copied.


