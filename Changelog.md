The Changelog
===

1.4.1
===

August 29, 2021

##### Fixes

* Fixes issue for Kucoin DCA exit.

##### Known Issues

Dashboard: Open positions has been removed and will return in a future release (ui only, does not affect engine).

Trading details: The trades list can sometimes not display the latest order made. A page reload should fix this temporarily. This will be fixed in the next 1.4.1 release (ui only, does not affect engine).

General: High numbers of orders may slow down the loading of the bot. This will be fixed in the next 1.4.1 release (ui only, does not affect engine).

Documentation: We're still building this out and it is in progress as of 1.4.x series.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.

1.4.0
===

August 27, 2021

Welcome Kucoin!
We have added Kucoin as our fourth exchange. A lot of work went into this and our thanks goes out to Thómas, our new developer. The bot currently does not support KCS discount fees yet, but we will be adding that support in a point release.

##### New Additions

* Private API - You can no specify in the settings the ability to not use the private api calls and only public calls. Certain members have asked for this as they have worked on some interesting ways to make the bot do things no one else does. This helps them do that.
* Manual buy/sell confirmation - You can not turn on or off a confirmation dialog for every manual buy sell you do.
* More meta data - the Exchange section of the Settings now shows all the pairs meta data for minimum and max amounts. Handy info since the exchanges won't give this to you up front.
* More quotes have been turned on for all the exchanges.

##### Fixes

* Updates to some of the trades calculations in the engines to make sure fees are applied correctly.

##### Known Issues

Dashboard: Open positions has been removed and will return in a future release (ui only, does not affect engine).

Trading details: The trades list can sometimes not display the latest order made. A page reload should fix this temporarily. This will be fixed in the next 1.4.1 release (ui only, does not affect engine).

General: High numbers of orders may slow down the loading of the bot. This will be fixed in the next 1.4.1 release (ui only, does not affect engine).

Documentation: We're still building this out and it is in progress as of 1.4.x series.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.


1.3.3
===

April 16, 2021

This is crtical hotfix for Binance.us.

##### Fixes

* Fixed websocket error Binance.us users were seeing on bot startup.

##### Known Issues

Dashboard: Open positions has been removed and will return in the next release (ui only, does not affect engine).

Trading details: The trades list can sometimes not display the latest order made. A page reload should fix this temporarily. This will be fixed in the next release (ui only, does not affect engine).

General: High numbers of orders may slow down the loading of the bot. This will be fixed in the next release (ui only, does not affect engine).

Documentation: We're still building this out and it is in progress as of 1.3.x series.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.

1.3.2
===

Mar 12, 2021

This is a minor point fix.

##### Fixes

* Fixed 429 errors on startup.

* Fixed problem on setup where an invalid exchange api key was entered and could not be corrected.

##### Known Issues

Dashboard: Open positions has been removed and will return in the next release (ui only, does not affect engine).

Trading details: The trades list can sometimes not display the latest order made. A page reload should fix this temporarily. This will be fixed in the next release (ui only, does not affect engine).

General: High numbers of orders may slow down the loading of the bot. This will be fixed in the next release (ui only, does not affect engine).

Documentation: We're still building this out and it is in progress as of 1.3.x series.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.

1.3.1
===

Feb 21, 2021

This is a minor point fix to address two critical issues with Binance/.us and Coinbase Pro exchanges.

##### Fixes

* Fixed binance/u.s. issue for bot not entering on enough min notional. Manual and automated buys and sells should be good going forward.

* Added 2 new sections to the Settings -> Reset.
  1. Paper Trade Orders reset. This allows you to clear out all your existing paper trade orders for a clean slate. Handy so you don't have to completely reset the whole db and lose your paper trades.
  2. Live Trade Orders reset. Works like paper trade reset. Since the binance issue mentioned above, there might now be a way to exit out because qty is too low. Now you can clear all your live trade orders (for all pairs), and exit your positions on the exchange. Again, better than resetting your entire db.

* Fixed high cpu load for Coinbase Pro.

* Added USDC and BUSD quotes for bianance.com.

##### Known Issues

Dashboard: Open positions has been removed and will return in the next release (ui only, does not affect engine).

Trading details: The trades list can sometimes not display the latest order made. A page reload should fix this temporarily. This will be fixed in the next release (ui only, does not affect engine).

General: High numbers of orders may slow down the loading of the bot. This will be fixed in the next release (ui only, does not affect engine).

Documentation: We're still building this out and it is in progress as of this release.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.

1.3.0
===

Feb 16, 20201

Binance.us has been added and the exchange section of the bot has had a major overhaul.

##### Fixes

* Binance.com websockets are fixed and will work as expected.

* All three exchanges now have updates to the rate limiting to make it more precise.

* Manual buy / sell buttons for live trading should now be fixed. Added better messaging as well in case of any kind of failure.


##### Known Issues

Dashboard: Open positions has been removed and will return in the next release (ui only, does not affect engine).

Trading details: The trades list can sometimes not display the latest order made. A page reload should fix this temporarily. This will be fixed in the next release (ui only, does not affect engine).

General: High numbers of orders may slow down the loading of the bot. This will be fixed in the next release (ui only, does not affect engine).

Documentation: We're still building this out and it is in progress as of this release.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.

1.2.3
===

Jan 26, 20201

Minor but critical updates.

##### Fixes

* Binance paper trading fees are now saved correctly. Prior to this the trade lines on the details page gave incorrectly formatted results.

* Manual buy / sell buttons has a bug that prevented buys or sells from being made. This is now fixed.

* Tickers feeds are now purely websocket based and api is only used on boot for warmup. This should reduce api requests.

* Backtesting candle fetch has been updated. A new candle set should only be fetched if the current time is greater than the latest candle for the pair/period in the db. This should significantly speeds on subsequent backtests using the same pair and period timeframe.

##### Known Issues

Dashboard: May still show open positions when they are closed on the trade details.

Exchange orders: FOK Limit orders my not go through as expected due to the local order book moving. We are researching this issue and should have a solution in the coming release(s).

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.


1.2.2
===

Jan 19, 20201

Lot's of updates and fixes. We'd like to thank Eric, Paul, Rai and everyone else that helped us pound on this. I made a huge difference!

##### Fixes

* As volume spiked, Coinbase Pro decided to not upgrade their infrastructure and let some api requests return 404 not found errors. Not surprised. This forced us to refactor some of the exchange code to deal with this. Extensive testing went into this over many days. If you saw any weird order errors with CB Pro, this is probably why and it is fixed.

* Fixed a dust issue on CB Pro and made sure that the api is always using the right side of the pair when doing quantity conversions. This should also fix an min amount errors people maybe have been seeing with CB Pro.

* Fixed Binance LOT_SIZE issue.

* Refactored all the accounting (big thanks to Eric for this) and dialed in the numbers more. This includes paper trading as well.

* Fixed a bug that prevented manual buy / sells from going through.

* Fixed bug for users that did not provide a last name on eval setup :facepalm: and were then prevented later from inputting a license to unlock the eval.

* Fixed a bug in the Settings > Account where account information could not be updated (like first and last name).

* TRUNCATE DATABASE is back in on Settings! This will truncate all candles past 30 days. If your db feels sluggish or too big, give this a shot.

* RESET DATABASE is back in the Settings as well. Resetting the db removes all data EXCEPT account, exchange configuration, and saved backtesting settings. You will need to manually reset all your paper trading account balances.

* Removed the button to flip a trade panel to the back panel. This will be re-introduced later if warranted.

* File locations are now placed under a port number folder if not using the default port. So, for instance, if the port flag has been set to ```port=4000```, the db and logs will live under ```HOME/acuitas/4000```. This now allows multiple bots running under different ports on the same machine and have all the file locations segmented correctly. If you are using the default port, then you will see the logs and database files in ```HOME/acuitas``` and no port path will be specified.

* New startup flag has been added to place the database wherever you want! Using the ```dbpath=``` flag, you can specify ***any*** directory/folder on your machine and the database will be placed there. This will override and work with the ```port=``` flag as expected. If you specified ```dbpath=G:\db1 port=4000```, the bot will place the logs in ```HOME\acuitas\4000``` and the db full path will be ```G:\db1\acuitas.sqlite```. Finally, the file paths will be displayed in the console window as the bot starts up.

##### Known Issues

Dashboard: May still show open positions when they are closed on the trade details.

Backtesting: For some runs, the backtesting engine may re-fetch data when not needed. This will be fixed in 1.2.3.

Paper / Live Trading: Sometimes when an order is placed, it may not update as expected in the trades table. Quick fix will be a reload and this will be addressed in 1.2.3 or 1.2.4.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.


1.2.1
===

Sorry, lots going on around the Dec holidays and we didn't get a chance to provide the release notes. :( See 1.2.2 above.

1.2.0
===

Dec 4, 2020

It's here, **DCA has been added**!

We have rounded out an insane year with an awesome feature **many** people have requested - Dollar Cost Averaging. We have made this as simple as possible too. Everything is gui up front and you can choose between a DCA buy signal of a fixed percentage drop OR a buy signal of the strategy iteself.

For fixed percent signal you can specify how much percent down the price will go for each buy (ie, 2% will buy when the price drops 2% from the last entry) as well as how many times to buy (ie, buy a max of 5 times). We have also included a few configs to specify they buy drop type. So if you have 1% and want a little more tweaking you can make that 1% applied to either a Log2 or Fibonacci calculation. This will allow for steeper curves that could potentially be more 'aggressive' in how sharp the price drop is.



Lastly, you can specify the strategy itself as the entry signal for the buy drops. This setting does not rely on any fixed or calculated percentage drop and runs solely off the strategy itself, so, you could get interesting results. Depending on how you have your strategy tuned, you could buy bigger drops and possibly exit at bigger profits. We will be expanding on this more in the future, so stay tuned!


NOTE: The Windows installer does not yet do the auto-update, so Windows users will still need to uninstall / install to get this version going.

##### Fixes

All the bugs can be referenced on the Acuitas Issues site: https://github.com/aqs-base/acuitas-issues

* Minor ui fixes on the trading details screens.

##### Known Issues

* Pair details screen does not stream complete volume to the chart. This is a non-critical issue since we are not using an volume based indicators at the moment. Navigating away from pair details and back will force the chart to reload, which will pull the proper volume from the local database. This will be fixed in a later point release.

* The hook to try to recover from your computer sleeping is still not working as we want. To be clear, this bot is not meant to be installed on anything other than a dedicated desktop/server, or vps. Powersaving, napping, etc, are not friendly to up to the second data flowing into the system. We've added some code to try to make the engine 'reset' when it detects a sleep/wake cycle, but this is still ongoing and experimental.

* Translation updates are coming. We had to pull the bulk of the translation code out when we switched the UI frameworks and will be adding this back in in a later point release. Apologies in advance to our non-U.S. English speaking friends.

* Possible issues with local currency conversion for display. We haven't tested every locale yet, but for the group we did, everything converted into local currency for display correctly. If yours isn't, please let us know.

* The Live and Paper trade dashboard Open Positions sometimes display the incorrect P/L amounts. This will be fixed in an upcoming point release and does not affect trading.

##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.

1.1.2
===

Sep 2, 2020

This release is mainly a performance and bug fix release.

NOTE: The Windows installer does not yet do the auto-update, so Windows users will still need to uninstall / install to get this version going.

##### Fixes

All the bugs can be referenced on the Acuitas Issues site: https://github.com/aqs-base/acuitas-issues

* Issue #1: BINANCE: Updated the sell calculations so that the bot will take into account if not enough BNB is available for fees. If this is the case, the fees are then taken from the appropriate side.
* Issue #2: Exchange data feeds have been throttled back to only listen for pairs that are in Paper or Live trading.
* Issue #3: You can now Markey BUY/SELL when a pair is off. This will work both on Paper and Live trading.
* Issue #4: Delisted pairs are now handled correctly and will not block the ui. Delisted pairs will also not try to trade and the only option now in the UI is to delete them.
* Issue #6: Performance bug fixed that was causing slow load times on the client UI; this impacted load by 2-4 seconds.
* Issue #8: Minor UI fixes.

##### Known Issues

* Pair details screen does not stream complete volume to the chart. This is a non-critical issue since we are not using an volume based indicators at the moment. Navigating away from pair details and back will force the chart to reload, which will pull the proper volume from the local database. This will be fixed in a later point release.

* The hook to try to recover from your computer sleeping is still not working as we want. To be clear, this bot is not meant to be installed on anything other than a dedicated desktop/server, or vps. Powersaving, napping, etc, are not friendly to up to the second data flowing into the system. We've added some code to try to make the engine 'reset' when it detects a sleep/wake cycle, but this is still ongoing and experimental.

* Translation updates are coming. We had to pull the bulk of the translation code out when we switched the UI frameworks and will be adding this back in in a later point release. Apologies in advance to our non-U.S. English speaking friends.

* Possible issues with local currency conversion for display. We haven't tested every locale yet, but for the group we did, everything converted into local currency for display correctly. If yours isn't, please let us know.


##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.


1.1.1
===

May 29, 2020

There have been some good fixes to trailing, Binance min notional, and from of the UI issues a few people were seeing. So, we wanted to get this out before the weekend.

NOTE: The Windows installer does not yet do the auto-update, so Windows users will still need to uninstall / install to get this version going.

##### Fixes

All the bugs can be referenced on the Acuitas Issues site: https://github.com/aqs-base/acuitas-issues

* Issue #1: Can't create live trade from paper trade.
* Issue #2: Live and paper trade stats row was missing the trade count in the P/L today box.
* Issue #3: Trailing is still off.
* Issue #4: Binance MIN_NOTIONAL is still causing issues.
* Issue #6: Table headers in trades table for pair details not rendering as expected on first order.
* Issue #8: UI does not load when bot is behind an nginx proxy because of host and port issues.

##### Known Issues

* Pair details screen does not stream complete volume to the chart. This is a non-critical issue since we are not using an volume based indicators at the moment. Navigating away from pair details and back will force the chart to reload, which will pull the proper volume from the local database. This will be fixed in a later point release.

* The hook to try to recover from your computer sleeping is still not working as we want. To be clear, this bot is not meant to be installed on anything other than a dedicated desktop/server, or vps. Powersaving, napping, etc, are not friendly to up to the second data flowing into the system. We've added some code to try to make the engine 'reset' when it detects a sleep/wake cycle, but this is still ongoing and experimental.

* Translation updates are coming. We had to pull the bulk of the translation code out when we switched the UI frameworks and will be adding this back in in a later point release. Apologies in advance to our non-U.S. English speaking friends.

* Possible issues with local currency conversion for display. We haven't tested every locale yet, but for the group we did, everything converted into local currency for display correctly. If yours isn't, please let us know.


##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.


1.1.0 - FINAL!!
===

May 27, 2020

The world is mad right now. Viruses, lockdowns, contact tracing and snitching, small businesses collapsing, massive unemployment numbers, exploding deficits that we didn't think were possible - in 30 days time. Dogs and cats living together, mass hysteria!

Some of us though, have been bracing for these things. All of us are here in crypto because it was never a stretch to think that all these houses of cards can only stay up so long before they start falling apart.

So, what better time to rewrite a major part of the bot?! From the beginning, we've been a gui-first piece of software. Writing for three platforms where you can install locally or remotely is extremely hard. Making it look good and work well is even harder. But, from the start, this was one of our goals - no text file configs or settings, everything gui first.

Why did we pick now to do this project?

Mostly because we have things comin down the pipe that just wouldn't work with the old UI code. That code was originally meant to 'git er done'. It was known not to be perfect and was there to put the first version out. We learned a lot about what we could improve on and what we didn't care for. So we spent all of March and April cranking out a completely new UI. This UI maintains most of the original look and feel, but removes some of the unnecessary chrome, condenses down some areas, and it's faster too. There are also a lot of things under the hood that make it about 100x easier and much faster for us to surface new functionality.

Some of the things that are in the new UI for this final 1.1.0 release.

* There is a new, completely rewritten setup flow with only the most minimal required info.
* You can edit paper / live trades fully with all changeable strategy properties, including switching time periods.
* Revamped the dashboard to track assets that your account has on the exchange. You can get to any pair details via a link since we have included open positions.
* There is a new Tutorials section that lists our curated list of videos so you don't have to go digging for them.

Some of you know this, but we've also included a new native installer for Windows folks. This installer will provide notifcations as well when updates are available. It also includes ALL the runtime requirements so you don't need to install Java anymore on your own - it comes with it.

The bot and ui have been in testing for a few months now by a lot of friends. Going forwards we're focusing on stability and feature expansion. We've got some good things on tap for the rest of this year that we think everyone will like.

##### Fixes

* Binance: LOT_SIZE should now behave as expected. Some users were reporting errors with this and we went back in an refactored a bunch of code as well as covered those changes with more tests.

* Binance: MIN_NOTIONAL is now handled better. This is the trickest of the Binance filters as it deals with cost. Since asset prices fluctuate all the time, we felt the best way to deal with MIN_NOTIONAL errors is to provide you with the _why_ of the error. We therefore provide the amount submitted along with the amount calculated via the MIN_NOTIONAL calcs on the Binance api docs. We decided against making any adjustments for you as it would possibly require the bot to increaase the amount you set and we feel that this is something you need to be in control of. Providing better messaging for the Order Events Log will inform you on the adjustments you will need to make in order to get the order done.

* Trailing has been rewitten and simplified in the engine. We think it is more accurate now as well.

* Tweaks to the paper trading accounting to tighten up the amounts.


##### Known Issues

* Pair details screen does not stream complete volume to the chart. This is a non-critical issue since we are not using an volume based indicators at the moment. Navigating away from pair details and back will force the chart to reload, which will pull the proper volume from the local database. This will be fixed in a later point release.

* The hook to try to recover from your computer sleeping is still not working as we want. To be clear, this bot is not meant to be installed on anything other than a dedicated desktop/server, or vps. Powersaving, napping, etc, are not friendly to up to the second data flowing into the system. We've added some code to try to make the engine 'reset' when it detects a sleep/wake cycle, but this is still ongoing and experimental.

* Translation updates are coming. We had to pull the bulk of the translation code out when we switched the UI frameworks and will be adding this back in in a later point release. Apologies in advance to our non-U.S. English speaking friends.

* Possible issues with local currency conversion for display. We haven't tested every locale yet, but for the group we did, everything converted into local currency for display correctly. If yours isn't, please let us know.


##### Filing issues:

All issues can be filed and tracked here: https://github.com/aqs-base/acuitas-issues/issues

Please provide:

* Your OS, version, basic comp specs (memory, etc).
* The bot version.
* Enough of a description to give us an idea of what's going on.
* Any and all screenshots you can provide.

DO NOT INCLUDE SENSITIVE DATA SUCH AS FULL NAMES, EMAIL, LICENSE KEYS, ETC.


1.1.0-beta15
===

Feb 8, 2020

#### Changes

* We're now using our cloud datastore as our source of truth for all candles. This allows us now to remove the burden of talking to the exchange for this data and therefore allows us to reduce the number of api requests we make to the exchange. This allows us to speed up the app and in our testing, Coinbase Pro speed is now on par with Binance.
* We have standardized on candle interval lengths. These lengths are: 1m, 5m, 15m, 30m, 1hr, 4hr, 1d. We feel that these intervals should provide enough options for candles sizes for everyone. We will automatically migrate any Binance 3m pairs to 5m pairs. Other intervals will be disabled. You will have to exit your positions manually on the exchange and delete those pairs in the bot.
* On the details panel the amount information updates on a regular interval. Some users complained that their 5% was not accurate over time - this was true on the UI since that amount was fixed from the point in time the price was calculated (the trading engine does not have this limitation). Using an update interval, you can now see more accurate, up to date information.
* We have removed the Desktop/GUI launcher as this was just creating too many problems for users. There were some weird dependencies that caused issues with the backtesting and our build/distribution process was just too complicated. We are now using the Windows installer/launcher for Windows users and Mac & Linux users can use the command line scripts. See your local *-guide.txt file for more info on how to run on your platform.

####Fixes

* Base/Quote conversion display on the trading pairs front panel was not updating correctly. It is now in sync with the back and details panels.
* Manual entry/exits were not using the correct event type for each side in the order event log. This is now fixed.
* Binance engine percentage code now correctly uses the fills qty/price from an entry order to exit.
* More database fine tuning for performance and file size.

##### Known Issues

* None.

This is the last release before the final 1.1.0. Please report any issues you see. Thanks!


1.1.0-beta14
===

Jan 21, 2020

#### Changes

* We're back to SQLite - from scratch this time. Efforts to try to migrate this before didn't go as planned and since trying to stabilize on a new db engine, we're just wiping the slate clean. Our goal is to NOT have to deal with any of these types of issues post final release. So we're doing them now. This means you will need to get out of your positions on the exchange and go through the setup process again.
* Removed the step of the setup that asks you to input the timezone and locale. We can get these from the host os now and so this whole step has been removed.
* Updated the token icon set.

####Fixes

* Base/Quote conversion fixes on the edit pair modal for percentage. This prevented some people from editing this value.

##### Known Issues

* It appears that 1m candles on Coinbase Pro are not working as expected. This means that backtests using 1m candles on Coinbase Pro never complete. We're looking into this and hope to have a fix by final.

We *really* trying to get the beta wrapped up, so please report any issues you see so we can get these resolved.



1.1.0-beta13
===

Jan 18, 2020

** THIS IS STILL A PRELIMINARY BETA AS TESTING HAS NOT CONCLUDED ON COINBASE PRO **

If you have any CB Pro issues, stop the bot and go back to beta 11.

####Fixes

* Database rollback back to the version beta 11 used. There were issues with the SQLite and there isn't the bandwidth right now to dive into that more. So, this will use the previous mv.db file.
* You can now truncate the database. Hopefully this will help speed things up. Go to Settings -> Maintenance tab to use this feature.
* Reworking of the trading engine and use to better handle trade and candle streams. This is part of the ongoing work to reduce code cruft and speed execution up.

As always, please report any issues you see so we can get these resolved.



1.1.0-beta12 (2112)
===

Jan 10, 2020

## 🥁🥁🥁 Neil Peart, R.I.P. 🥁🥁🥁

 > We've taken care of everything
 > The words you read, the songs you sing
 > The pictures that bring laughter to your eye
 > It's one for all and all for one
 > We work together, common son
 > Never need to wonder how or why

This week, one of my few heroes has died. Neil Peart entered my life when I was young, at the beginning of my teenage years. At first, he set the standard for me as to what a master drummer could be. I grew up thinking that how he played drums naturally made sense and all drummers should and would aspire to play like him. Through my teens and twenties as I weaved my way through various bands, I sadly learned that the opposite was true. No one played like him.

No one thought like him either. 

As I grew up with Rush, I found Neil's other, even more underrated masterful ability - his lyrics. Neil wrote almost all the lyrics for the second Rush album on. He wrote of fairly typical topics on the early recoards until their breakout: 2112. That album to me, was where his lyrics hit high gear and never looked back. There was intent and purpose in everything he wrote. I appreciate that even more in modern times because I think it is sorely lacking in today's music and art.

I mention all this because I have dropped all kinds of easter eggs into the code of the bot (the majority you'll never see) based off his words and ideas. The first song on 2112 still holds relevance for me today. Actually, even more so. Not just for Bitcoin/Crypto and giving people control of how they transact with *their* money , but also because it spoke of the power of collectivism and totalitarian state against the individual. I'd encourage anyone interested in these topics to load up 2112, get the lyrics next to them, and spend the 20-30 mins listening and thinking. Yah, it's 70's rock, not the music of today, but its words, music, and songwriting are timeless.

Rush, and Neil in particular shaped a lot of my youth and I constantly go back to lyrical passages when I'm reflecting on life, family, friends, and the world in general. I can recommend the years 1975-1982 from their catalog. Those were their most prolific for me. If you do decide to take a listen, I hope you enjoy and dig a little deeper under the surface.

 > Each of us, a cell of awareness. 
 > Imperfect and incomplete. 
 > Genetic blends with uncertain ends.
 > On a fortune hunt that's far too fleet.
 
 
Nibaru
 
===

##### DATABASE MIGRATION

Beta 12 has a new database! We've switched from an encrypted embedded database to SQLite. Some users have had speed issues and it was laborious for me to deal with it. SQLite supports multi-terabyte databases (not that you'll ever have one that big) and I am more confident in its ability to speed things up as well as be a more efficient store.

There is a path through all this, so please read on.

Before you do anything, shut down your bot and backup you mv.db file. Worst case if something catastrophic happens, you can run beta 11 against the old database and then we can chat in the support channel what the problem is. 

There are two scripts that will put beta12 into migration mode:
```
Desktop-Migrate.ps1
desktop-migrate.sh
```

Windows users need to right click on ```Desktop-Migrate.ps1``` and select Run. This will start up the bot with the migrate flag, which shows a modified ui. 

Mac/Linux users, open up a shell, cd to the directory where beta 12 was unzipped (search for how to ```cd``` in a terminal/shell if you don't know how to). Sorry, there's no other way to make this easier right now. Once you are in that directory type:
```./desktop-migrate.sh```

Once the gui is up, you will see a modified ui. There is only one thing to do on this ui and that's to run the migration process. 

Click the ```Migrate``` button to begin this process. DO NOT EXIT or do anything else. I've run this many times and it is stable, so you shouldn't have any problems. The bot will give feedback in the text panel on the migration progress. Depending on how big your database is, it could take from a few mins to about 45 mins. I did a 21GB database migration and it took about 45 mins for me. On a smaller database, it was done in under 5 mins. 

Once the data base been migrated, the gui and bot will exit automatically. You can then run it as you normally do by double clicking on the beta12 jar or via one of the script/bat file methods.

Lastly, because none of the database is encrypted now, it's up to YOU to secure it. If you put this on a VPS, make sure you have it secured! And if you don't know how to do that, ask around on the channel and someone will help. This is YOUR database, so, treat it as such.

(Migration instructions end)

#### Fixes

* On pair details screen, the trades list now reflects the qty of a buy order. Before it would not show this.
* Manual buy/sells can now be done with the pair turned off. This is nice and allows you to buy/sell without having to worry that your trying to time things with the bot engine.
* I think the exit bug is fixed. This was due to, of course, a rounding error that would cause the exit qty to round up based on the quote price scale. Now, it rounds down correctly.

As always, please report any issues you see so we can get these resolved.



1.1.0-beta11
===

Dec 24, 2019

🎄🎄🎄 MERRY CHRISTMAS! 🎄🎄🎄

##### IMPORTANT: We are now distributing TWO jar files. They first has the name Desktop in it and the second has the name Server in it.

##### Desktop now runs a gui control panel where you can set the bot port and start / stop the bot. This should make it much easier to launch and control for all Desktop users. You should be able to just double-click on the jar file to run.

##### Server will run in text console mode (like all builds did before) and is meant to run on a vps/local server.

This release does not address running multiple bots on different ports. For any bot after your first, you will need to run separately via the Server with whatever custom start script you have.

---

* As noted above, the releases have been split into different jars and there is now a gui launcher. This gui launcher should run on all platforms by just double-clicking the Desktop jar file.
* This release is still Java 8 only, but work has been done internally to free us of that. Upcoming releases will not be bound to this.  
* This release mostly targeted bugs and performance. The local trades database is now pruned which should help prevent memory from getting out of control.
* All exceptions are logged into a separate exceptions.log file.

Known issues
---

* Some users have experienced an issue where the bot does not exit at the expected stop loss percentage. This work is still ongoing and the exceptions log should now help diagnose this issue so it can be fixed in the next build.

As always, please report any issues you see so we can get these resolved.


1.1.0-beta10
===

Dec 14, 2019

* WINDOWS USERS: Please use the Powershell launcher now. This has much better cpu and performance utilization. Right click on the Start-Acuitas file and select 'Run with PowerShell'. You will see significant performace gains using this. The old start.bat file will be removed in beta11.
* Coinbase Pro: All markets have been enabled.
* Binance: Enabled PAX and TUSD markets.
* All fiat based values should now be converted for display correctly. Testing this mostly involved our GBP and EUR friends.
* Paper and Live Trades now present a confirmation dialog when deleting.
* Fixes for some issues people were seeing with prices not displaying correctly on the Paper/Live Trade edit modals.
* Internal improvements to better manage memory and better utilize concurrency.


1.1.0-beta9
===

Dec 6, 2019

* Paper trading fixed values are now zeroed out when newly created. Before, the fixed amount value was carried over from the backtest and this didn't need to adhere to the paper trading balance for that quote asset. Paper trades are now turned off by default on new create and cannot be turned on until a valid quote amount is entered on the edit modal.
* Better validation for Paper and Live trade edit screens. Minimum order sizes are now better enforced so that you cannot enter a quote amount on the edit screen lower than what the exchange specifies as a minimum.
* Fixes to the manual buy/sell to make sure that the appropriate time for order creation is the current 'now' time.
* Introduced a 'db' flag that will allow you to specify what you want your database to be named. This will create a directory of the same name user your user's home directory. This will also allow multiple bot instances to be run on the same machine with a different port number.
* Added some more output in the bot startup to display the full path to the database being used as well as what exchange the bot is licensed for. Handy info to help us help you with any troubleshooting you may need.
* Introduced a new 'delete-db.bat' script for windows users. This will delete the database for you in your database directory. This was provided by Craigs Cryptos (thank you!).
* Upgraded our core exchange library. This version included various optimizations and additions to both Coinbase Pro and Binance api clients.
* More fine tuning on setup. Some users were bouncing out when their setup didn't properly complete. This should be fixed.
* Setup step one error checking and reporting improvements. License keys are checked more rigorously by the local bot api.

Known issues
---

* Binance: Some users are still reporting that they cannot see MATIC and a few other currencies. This is ongoing as it has not yet been reproduceable.
* Sometimes, some of the trading view charts might not render correctly. This seems to be a low percentage of the time, but it is being investigated.

As always, you can help out by reporting any issues you see to the proper online channels so that we can get them into our ticketing system.

1.1.0-beta8
===

Dec 2, 2019

Fast releases usually mean important bug fixes.

* ALL: Fixed a regression in the pairs not showing up. ([Ticket #3] cant get Pairs to wotrk for Windows 10.)
* Coinbase Pro: Fixed regression in websocket where candlesticks were not processing correctly.
* Switched over from text changelog to markdown version. Not a huge difference here, just some adjustment to the formatting.

Known issues
---

* Binance: There are still some entry/exit errors for MIN_NOTIONAL and LOT_SIZE. This can prevent a lot of orders from going through, but some still can. Beta9 will focus on dialing these in better.
* Binance: Some users are still reporting that they cannot see MATIC and a few other currencies. This is ongoing as it has not yet been reproduceable.
* Sometimes, some of the trading view charts might not render correctly. This seems to be a low percentage of the time, but it is being investigated.


1.1.0-beta7
===

Nov 30, 2019

* Fixed an issue in the engine where the manual buy/sell was using the wrong timestamp sometimes to record the trade (this was only a local issue and did not affect the order on the exchange itself).
* The percent and fixed amounts should now reflect correctly on the UI and for any orders placed.
* Dashboard and ui cleanup.
* Added a debug section that displays all the pairs that the bot is currently using. This is the start of some user diagnostic tools to help reporting any issues they may see.

As always, report any issues you see to the online conduits.

Known issues:

* Some people are reporting some ui issues with price conversions - these are still ongoing since they're only affecting a small amount of users.

* Some users are also reporting that a few pairs are missing. This is still an ongoing investigation to figure out why this is happending. It's so far only affected a small amount of users.

---

Nov 28, 2019
1.1.0-beta6
=========================

For our U.S. users, Happy Thanksgiving!

Meat's back on the menu boys!... (There's a movie reference there..)

* Binance is back! And it's fast! Backtesting works. Paper trading works. Live trading, mostly works. (See known issues below). We have enabled USDT, ETH, BNB, and BTC markets. More to come in later releases.
* There are more little UI fixes on backtesting and the trading screens.
* Backtesting pair selection box now supports search again! Start typing a pair and it will autocomplete the list (again).

This release is primarily for users to start using their Binance accounts again. It is sill beta and while we have made some successful live trades, there are still some minor issues we're ironing out. Other than that, we're getting close to our final 1.1.0 release.

As always, report any issues you see to the online conduits.

Known issues:

* Binance sometimes doesn't calculate the correct qty of quote asset and therefore misses a trade. Because of this, no entry will be made - we're categorizing this as a minor, non-critical issue.

* Market buy/sell now has not been fully tested on Binance yet for Live trading. If you do decide to try it, use at your own risk. We'll have it tested more thoroughly in the next release. It's possible it does work as the code was already abstracted out and working in prior Coinbase Pro releases.


Nov 26, 2019
1.1.0-beta5
=========================

Lots of tweaks and bug fixes!

* SYSTEM PASSWORD IS REQUIRED! We now force you to set a system password on start/install of the bot. Subsequent page loads will require the password to be added. Upon setting a new password or providing it via an access request, the system will save it as a cookie on the browser so you don't have to keep re-entering it. This overall will help with security (the http connection is still clear text) and users have been asking about this for a while.

NOTE: To reset the password (in case you lose it), add the --reset-password=true flag to the end of the start.sh/.bat command. Start the bot, let it boot. There will be a message saying the password has been reset. Stop the bot. Remove the reset-password flag. Restart the bot. You will then be prompted to enter your new password.

* Dashboard daily profit now tracks the current week correctly.
* Edit Paper / Live trades now should work as expected. There were a few bugs that wouldn't allow switching from a fixed/percent price as well as form fields that would duplicate each time edit was clicked. These have been fixed and the functionality should be stable.
* Details screem now shows better info on your fixed/percent amount along with fiat equivalent.
* There was an issue where failed orders kept hitting the exchange too quickly. These are now handled correctly and as part of this, the order events logs the exchange spefific error.
* Out of memory/Websocket errors - these should all be cleaned up and handled correctly now.
* Collapsing / Expanding Paper/Live trades now persists locally. This means if you collapse your pairs view, go to another screen, come back - the pairs will show in the collapsed view.
* Fixed an issue with the Trading View charts where they could get all weird and the trades bunch up on the right side of the screen.
* Live Trading is still considered ready for use now. As always, if you see any issues, don't hesistate to grab someone in the group.

Known issues:

* Binance has been disabled, but will return soon.

WARNING: DO NOT (YET) PUT THIS ON YOUR BINANCE PAIRS. THERE HAS BEEN SIGNIFICANT CHANGES TO THE TRADING ENGINE AND WE HAVE NOT THOUROUGHLY TESTED BINANCE (that should be available in beta 4). RUN THIS ON A COMPLETELY SEPARATE VM/VPS/MACHINE UNLESS YOU WANT TO TAKE THAT RISK. IT COULD WORK, BUT WE JUST DON'T FULLY KNOW YET. WE WILL HAVE THIS RESOLVED BY THE 1.1.0 FINAL.



Nov 15, 2019
1.1.0-beta4
=========================

Ooops, we skipped beta3.

* MANUAL BUY & SELL ARE IN! You can now execute manual market orders with a click of the button. See the pair details screen for the new Buy and Sell buttons.
* Dashboard now behaves as expected with the multiple quote currencies.
* Lots more tightening and bug fixing of the engine code. Lots.
* UI's for paper trading and live trading are now consistent and feature complete.
* Tons of UI cleanup on all the screens.
* Bug fixes for some people seeing issues where the bot would never start up properly.

* Live Trading is still considered in final testing phases and while it's 'working' and should be ok, you might want to use small ammounts for now.

Known issues:

* Binance has been disabled, but will return soon.

* Editing Live and Paper trades is still in beta - there might be minor bugs.

* Still seeing intermittent sync issues on fetching amounts for conversion on the various forms (non-critical).

WARNING: DO NOT (YET) PUT THIS ON YOUR BINANCE PAIRS. THERE HAS BEEN SIGNIFICANT CHANGES TO THE TRADING ENGINE AND WE HAVE NOT THOUROUGHLY TESTED BINANCE (that should be available in beta 4). RUN THIS ON A COMPLETELY SEPARATE VM/VPS/MACHINE UNLESS YOU WANT TO TAKE THAT RISK. IT COULD WORK, BUT WE JUST DON'T FULLY KNOW YET. WE WILL HAVE THIS RESOLVED BY THE 1.1.0 FINAL.


Oct 8, 2019
1.1.0-beta2
=========================

* More updates to the trading engine to tighten up the api restrictions the exchanges require.
* Lots of internal additions to make Coinbase Pro work more like a modern exchange...
* More tweaks to the setup screens so that the Next button enables when the forms are valid. This helps to solve the force clicking out of a field to get the button to update.
* Paper trades are no longer deleted when the Live Trade is created.
* More minor ui updates to the trading details screen.

* Live Trading is still considered in final testing phases and while it's more stable than the previous beta, use at your own risk - for now.

Known issues:

* Editing trades has some issues on how the form is configured. Trying to edit a trade multiple times without refreshing the page, will cause the form to not work as expected. The work around is to reload the page after each save done on the edit modal.

* When a pair details is displayed, some of the pricing & p/l values are not correct. This is because Coinbase Pro does not provide updates every second as Binance does. After the first trade has been received from Coinbase Pro, these numbers will update correctly.

* Dashboard BTC Markets section is still using Binance - this will be updated to use the selected exchange in the coming betas.

* Binance is still not tested - see warning below.

WARNING: DO NOT (YET) PUT THIS ON YOUR BINANCE PAIRS. THERE HAS BEEN SIGNIFICANT CHANGES TO THE TRADING ENGINE AND WE HAVE NOT THOUROUGHLY TESTED BINANCE (that should be available in beta 4). RUN THIS ON A COMPLETELY SEPARATE VM/VPS/MACHINE UNLESS YOU WANT TO TAKE THAT RISK. IT COULD WORK, BUT WE JUST DON'T FULLY KNOW YET. WE WILL HAVE THIS RESOLVED BY THE 1.1.0 FINAL.


Sept 21, 2019
1.1.0-beta1
=========================

* Fixed a bug in the edit Paper Trade form where the rsi fields weren't working correctly.
* Added support to start the bot on a different port. Just append port=8080 (or whatever high number you want) and the bot will start and bind to that port.

* Live Trading is still considered in testing phase so don't rush in just yet. We'll announce when it's safe.

WARNING: DO NOT (YET) PUT THIS ON YOUR BINANCE PAIRS. THERE HAS BEEN SIGNIFICANT CHANGES TO THE TRADING ENGINE AND BECAUSE WE'RE AMERICANS AND BINANCE KICKED US OUT, WE HAVE NOT THOUROUGHLY TESTS EVERYTHING. RUN THIS ON A COMPLETELY SEPARATE VM/VPS/MACHINE UNLESS YOU WANT TO TAKE THAT RISK. IT COULD WORK, BUT WE JUST DON'T FULLY KNOW YET. WE WILL HAVE THIS RESOLVED BY THE 1.1.0 FINAL.


Sept 18, 2019
1.0.6-244
=========================

* Fixed a bug in the CoinbasePro candles that wasn't respecting candle close time. Eeeek! This caused all kinds of probs and the chart looks solid once again.
* Fixed the negative current capital for paper trading.
* Fixed the Step 2 process on setup. The exchage credentials now correctly handle any typos or errors the exchange returns.
* Live Trading is still considered in testing phase so don't rush in just yet. We'll announce when it's safe (it's close tho!).


Sept 17, 2019
1.0.6-216
=========================

* Updates to the Coinbase Pro data sync services. We are processing trades more proactively now to deliver better updates to the trading engine and TradingView chart(s).


Sept 8, 2019
1.0.6-213
=========================

* Data sync service attempts to 'heal' gaps in candle pricing for exchanges that have flaky or not enough trades in their system. This is done to minimize anomolies in candles that the strategies run over.
* Editing live trades is in, but still needs more testing - use at your own risk (for now)!


Sept 7, 2019
1.0.6-212
=========================

* Added in proper system architecture to reduce api calls and use the database directly again. We are back to fast refreshes on charts, backtesting, and trading.


Sept 2, 2019
1.0.6-209
=========================

* Bug fixes for settings screen.
* Bug fixes for setup flow not saving Coinbase Pro password correctly.
* Fixes for some of the Coinbase Pro ticker fetches.


Sept 1, 2019
1.0.6-207
=========================

* More bug fixes and updates for paper trading edit
* Tightening up of CoinbasePro api rate limiting


Aug 31, 2019
1.0.6-205
=========================

* Bug fixes for paper trading.
* You can now edit most paper trade settings on the fly.


Aug 20, 2019
1.0.6-203
=========================

* Coinbase works with backtesting.
* Coinbase works with papertrading.


June, 2019
1.0.6-197
=========================


First release!
