
Changelog Jeedom V4
=========

4.1.0
=====
- Synthesis : Adding a new page **Home → Summary** offering a global visual synthesis of the parts.
- Research : Add of a search engine in **Tools → Search**.

- Dashboard : Edit mode now inserting the moved tile.
- Dashboard : We can now click on the * time * of the time actions widgets to open the history window of the linked info command..
- Dashboard : The size of a new equipment&#39;s tile adapts to its content.
- Dashboard : Ctrl Click on an info opens the history window with all the historicized commands of the equipment visible on the tile. Ctrl Click on a legend to display only this one, Alt Click to display them all.
- Dashboard : Ability to blur background images (D'actualité -> Interface).
- Tools / Widget : The * Apply on * function shows the linked commands checked, unchecking one will apply the default core widget on this command.
- Widget : Ability to add class css to a widget (see widget documentation).
- Widget : Adding a core * sliderVertical widget*.
- Update Center : Updates are checked automatically when the page is opened if it is 120 mins older.
- Update Center : The progress bar is now on the * Core and plugins * tab, and the log open by default on the * Information tab*.
- Update Center : If you open another browser during an update, the progress bar and the log indicate it.
- Update Center : If the update finishes correctly, display of a window asking to reload the page.
- Core updates : Implementation of a system for cleaning up old unused Core files.
- Widget / Objects / Scenarios / Interactions / Plugins Pages :
	- Ctrl Clic / Clic Center on a Widget, Object, Scenarios, Interaction, plugin equipment : Opens in a new tab.
	- Ctrl Clic / Clic Center also available in their context menus (on the tabs).
- New ModalDisplay page:
	- Analysis menu : Ctrl Click / Click Center on * Real time* : Open the window in a new tab, in full screen.
	- Tools menu : Ctrl Clic / Clic Center on * Notes *, * Expression tester *, * Variables *, * Search* : Open the window in a new tab, in full screen.
- Scenario : Adding a search engine (to the left of the Run button).
- Scenario : Addition of the age function (gives the age of the value of the order).
- Scenario : *stateChanges () * now accepts the period * today * (from midnight to now), * yesterday * and * day * (for 1 day).
- Scenario : Functions * statistics (), average (), max (), min (), trend (), duration ()* : Bugfix for the period * yesterday *, and now accepts * day * (for 1 day).
- Scenario : Possibility to deactivate the automatic quote system (Settings → System → D'actualité : Orders).
- Scenario : Display of a * warning * if no trigger is configured.
- Scenario : Bugfix of select on copy / paste block.
- Scenario : Copy / paste of block between different scenarios.
- Scenario : The undo/redo functions are now available in the form of buttons (next to the block creation button).
- Scenario variables window : alphabetical sort at opening.
- Analysis / History : Ctrl Click on a legend to display only this history, Alt Click to display them all.
- Analysis / History : The options * grouping, type, variation, staircase * are active only with a single curve displayed.
- Analysis / History : We can now use the * Area * option with the * Staircase option*.
- View : possibility to put scenarios.
- History : Integration of the Timeline in DB for reliability reasons.
- History : Management of multiple timelines.
- History : Timeline graphic overhaul.
- Home automation summary : Plugin equipments deactivated and their controls no longer have the icons on the right (equipment configuration and advanced configuration).
- Home automation summary : Ability to search on equipment categories.
- Home automation summary : Possibility to move several pieces of equipment from one object to another.
- Home automation summary : Possibility to select all the equipment of an object.
- Task engine : On the * Daemon * tab, deactivated plugins no longer appear.
- D'actualité : The *Information* tab is now in the *General* tab*.
- D'actualité : The *Commands* tab is now in the *Equipments* tab*.
- Advanced equipment configuration window : Dynamic change of switchboard configuration.
- About window : Addition of shortcuts to Changelog and FAQ.
- WebApp : Integration of the new Summary page.
- WebApp : Scenarios page, a click on the scenario title displays its log.
- WebApp : We can now select / copy part of a log.
- WebApp : On the search in a log, addition of an x button to cancel the search.
- WebApp : Persistence of the theme toggle (8h).
- WebApp : On a design, a click with three fingers returns to the home page.
- WebApp : Display of scenarios by group.
- WebApp : Many bug-fix (UI, portrait / landscape iOS, etc.).

- Documentation : Adaptations in line with v4 and v4.1.
- Documentation : New page * Keyboard / mouse shortcuts * including a summary of all shortcuts in Jeedom. Accessible from the Dashboard doc or the FAQ.

- Bug fixes and optimizations.
- Lib: Update HighStock v7.1.2 to v8.0.4.


4.0.53
=====

- Bug fix.

4.0.52
=====

- Bug correction (update to be absolutely done if you are in 4.0.51).

4.0.51
=====

- Bugfix.
- Optimization of the next DNS system.

4.0.49
=====

- Possibility of choosing Jeedom's TTS engine and possibility of having plugins that offer a new TTS engine.
- Improved support for webview in the mobile application.
- Bugfix.
- Updating the doc.

4.0.47
=====

- Improvement of the expression tester.
- Updating the repository on smart.
- Bugfix.

4.0.44
=====

- Improved translations.
- Bugfix.
- Improved cloud backup restore.
- Cloud restoration now only get the local backup, leaving the choice to download or restore it.

4.0.43
=====

- Improved translations.
- Bug fixes on scenario templates.

4.0.0
=====
- Complete redesign of themes (Core 2019 Light / Dark / Legacy).
- Possibility to change the theme automatically according to the time.
- In mobile, the theme can change depending on the brightness (Requires activating * generic extra sensor * in chrome, chrome page://flags).<br/><br/>
- Improvement and reorganization of the main menu.
- Plugins menu : The list of categories and plugins is now sorted alphabetically.
- Tools menu : Addition of a button to access the expression tester.
- Tools menu : Addition of a button to access the variables.<br/><br/>
- Search fields now support accents.
- The search fields (Dashboard, scenarios, objects, widgets, interactions, plugins) are now active when the page opens, allowing you to type a search directly.
- Add an X button on the search fields to cancel the search.
- During a search, the * escape * key cancels the search.
- Dashboard : In edit mode, the search field and its buttons are disabled and become fixed.
- Dashboard : In edit mode, a click on an * expand * button to the right of the objects resizes the tiles of the object to the height of the highest. Ctrl + click reduces them to the height of the lowest.
- Dashboard : Order execution on a tile is now indicated by the * refresh button*. If there is none on the tile, it will appear during the execution.
- Dashboard : The tiles indicate an info command (history, which will open the History window) or action on hover.
- Dashboard : The history window now allows you to open this history in Analysis / History.
- Dashboard : History window retains its position / dimensions when another history reopens.
- Command D'actualité window: Ctrl + click on &quot;Save&quot; closes the window after.
- Equipment D'actualité window: Ctrl + click on &quot;Save&quot; closes the window after.
- Adding usage information when deleting equipment.
- Objects : Added option to use custom colors.
- Objects : Add context menu on tabs (quick object change).
- Interactions : Add context menu on tabs (quick interaction change).
- Plugins : Add context menu on tabs (quick change of equipment).
- Plugins : On the Plugins management page, an orange dot indicates non-stable plugins.
- Table improvements with filter and sort option.
- Ability to assign an icon to an interaction.
- Each Jeedom page now has a title in the interface language (browser tab).
- Prevention of auto-filling on fields&#39; Access code'.
- Management of functions * Previous page / Next page * of the browser.<br/><br/>
- Widget : Redesign of the widget system (Tools / Widget menu).
- Widget : Ability to replace a widget with another on all commands using it.
- Widget : Ability to assign a widget to multiple commands.
- Widget : Add horizontal info numeric widget.
- Widget : Adding an info numeric vertical widget.
- Widget : Addition of an info numeric compass / wind widget (thanks @thanaus).
- Widget : Adding an info numeric rain widget (thanks @thanaus)
- Widget : Display of the info / action shutter widget proportional to the value.<br/><br/>
- D'actualité : Improvement and reorganization of tabs.
- D'actualité : Added many * tooltips * (help).
- D'actualité : Adding a search engine.
- D'actualité : Adding a button to empty the widget cache (Cache tab).
- D'actualité : Added option to disable widget cache (Cache tab).
- D'actualité : Ability to center the content of the tiles vertically (Interface tab).
- D'actualité : Addition of a parameter for the global purging of the histories (Tab Commands).
- D'actualité : Change from # message # to # subject # in D'actualité / Logs / Messages to avoid duplication of the message.
- D'actualité : Possibility in the summaries to add an exclusion of the orders which have not been updated for more than XX minutes (example for the calculation of the temperature averages if a sensor has not raised anything for more than 30min it will be excluded from the calculation )<br/><br/>
- Scenario : The colorization of the blocks is no longer random, but by type of block.
- Scenario : Possibility by Ctrl + click on the button * execution * to save it, launch it, and display the log (if the log level is not on * None *).
- Scenario : Block deletion confirmation. Ctrl + click to avoid confirmation.
- Scenario : Addition of a search function in the Code blocks. Search : Ctrl + F then Enter, Next result : Ctrl + G, Previous result : Ctrl + Shift + G
- Scenario : Ability to condense blocks.
- Scenario : The &#39;Add block&#39; action switches to the Scenario tab if necessary.
- Scenario : New block copy / paste functions. Ctrl + click to cut / replace.
- Scenario : A new block is no longer added at the end of the scenario, but after the block where you were before clicking, determined by the last field in which you clicked.
- Scenario : Implementation of an Undo / Redo system (Ctrl + Shift + Z / Ctrl + Shift + Y).
- Scenario : Delete scenario sharing.
- Scenario : Improvement of the scenario templates management window.<br/><br/>
- Analysis / Equipment : Addition of a search engine (Batteries tab, search on names and parents).
- Analysis / Equipment : The calendar / days area of the equipment is now clickable to directly access the change of battery (s).
- Analysis / Equipment : Addition of a search field.<br/><br/>
- Update Center : Warning on the &#39;Core and plugins&#39; and / or &#39;Others&#39; tab if an update is available. Switch to &#39;Others&#39; if necessary.
- Update Center : differentiation by version (stable, beta, ...).
- Update Center : addition of a progress bar during the update.<br/><br/>
- Home automation summary : The deletion history is now available in a tab (Summary - History).
- Home automation summary : Complete overhaul, possibility of ordering objects, equipment, orders.
- Home automation summary : Addition of equipment and order IDs, in display and in search.
- Home automation summary : CSV export of parent object, id, equipment and their id, command.
- Home automation summary : Possibility of making visible or not one or more orders.<br/><br/>
- Design : Ability to specify the order (position) of * Designs * and * 3D Designs * (Edit, Configure Design).
- Design : Addition of a custom CSS field on the elements of * design*.
- Design : Displacement of display options in Design of the advanced configuration, in the display settings from * Design*. This in order to simplify the interface, and allow to have different parameters by * Design*.
- Design : Moving and resizing components on * Design * takes their size into account, with or without magnetization.<br/><br/>
- General reduction (css / inline styles, refactoring, etc.) and performance improvements.
- Remove Font Awesome 4 to keep only Font Awesome 5.
- Libs update : jquery 3.4.1, CodeMiror 5.46.0, tablesorter 2.31.1.
- Numerous bug fixes.
- Adding a mass configuration system (used on the Equipment page to configure the Communication Alert on these)

>**IMPORTANT**
>
>If after the update you have an error on the Dashboard try to restart your box so that it takes the new additions of components into account.

>**IMPORTANT**
>
>The widget plugin is not compatible with this version of Jeedom and will no longer be supported (because the functions have been taken over internally on the core). More information [here](https://www.Jeedom.com/blog/4368-les-widgets-en-v4).
