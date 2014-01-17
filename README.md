PoEBot
======

Path of Exile event IRC bot

This is a very simple IRC bot, meant to join a channel and assist with tracking PoE races.

!next will display the currently running race, if any, and the next upcoming event, with appropriate timers for time remaining and time until

!help will display the help (currently just !next and how it works)

!track <account> (admin only) will set the account to be tracked

!place/!rank will tell the rank of the tracked account in the current race, if one is active, and if they are on the ladder.

!about will give me credit :D

The bot will also act as a timer: at one hour to an event, and five minutes before, it will say into the channel that an event is upcoming, along with details.

-Python 3.3
-pytz
-datetime
-requests

The packages were not included by default on my install, so they may not be on yours either.

Within PoEBot.py, you should also edit the server, channel, and botnick to appropriate values. I have not yet added an authentication feature yet. If you are not in USE, you should change the TZ as appropriate. Administrators is a list of Bot admins. rate_limit controls how often the bot can respond to non admin commands put into chat. defLeague is the default league setting, which is a fallback for !place if no race is running.

Enjoy some MIT License
-Skyl3lazer


Copyright (c) 2014 by Skyl3lazer

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
