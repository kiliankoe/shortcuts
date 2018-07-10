# 🏎 Shortcuts

Shortcuts created with Apple's new Shortcuts app, previously known as Workflow. Download them on your iOS device and open in Shortcuts to import. Please feel free to contribute changes and/or your own workflows 😊

By the nature of this repo these are probably a little biased by my personal interests, for more general stuff you should check out [Sharecuts](http://sharecuts.app).



### DVB Abfahrten

This shortcut has a predefined list of public transport stops for Dresden. You select the stop and a list of upcoming departures is shown. 

To adjust for your own stops edit the menu at the top and supply URL compatible names (I have no clue why the URLEncode action is of no help here) and a timeoffset of your choice (aka the time it takes to get to the stop - departures below that offset are not shown).



### Mensa

This is a shortcut for accessing today's meals in Dresden's canteens. It uses [this API](https://github.com/htwdd/emeal-server). To configure for yourself adjust the listed canteens in the menu and take the IDs from [here](https://github.com/HTWDD/emeal-server/blob/master/Config/canteen.json).



## Contributing

When not making trivial changes to the XML source itself, it's best to edit these within the Shortcuts app. Unfortunately shortcuts exports binary plists, so before contributing the changes it's best to convert them back to XML. This is easy to achieve using the following command which modifies the file in place.

```shell
$ plutil -convert xml1 MyShortcut.shortcut
```

