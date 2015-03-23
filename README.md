Crontab Syntax Highlighting
===========================

Installation
------------

1. Open Sublime Text 2/3
2. Locate Preferences in the menu, click on "Browse Packages..."
3. Create a folder named Crontab and copy everything from this repository in that folder
4. Enjoy


Optional
-----------

A recent addition was using a few different sytax types like `constant` and `keyword`
in the language definition syntax. This is a bit of a hack because Sublime Text does not
seem to have an [easy way for a plugin to suggest colors][1] for the language scopes. In
addition, it is hard to know what scopes will be available in a theme, so with most
`meta.hour.crontab` and `meta.minute.crontab` will show up the same. This led me to believe
the plugin was 'broken' when it was first installed because everything was one color.

The syntax will look acceptable with most themes with these revised scopes:

	keyword.at.crontab
	keyword.minute.crontab
	constant.hour.crontab
	class.dayofmonth.crontab
	keyword.month.crontab
	constant.dayofweek.crontab
	string.command.crontab

This will at least give it some syntax coloring with most themes - but still allow themes
to override the colors.

If you would like to make the colors look more like the `vim darkbg` style,
add the definitions from the included `optional-add-to-theme.xml` file to your theme, or
perhaps use the [Sublime Theme Editor](http://tmtheme-editor.herokuapp.com/) to customize.

![vim dark][2]





Credits
-------

[WheresWardy](https://github.com/WheresWardy)
[kevinior](https://github.com/kevinior)


[1]: http://stackoverflow.com/questions/19235792/change-color-of-specific-words-in-sublime-text-3
[2]: http://puu.sh/gMCo3/df588859e4.png "screenshot"
