# UGC API

An *in progress* guide on how to use the UGC API.

In order to use the UGC API you must obtain an API key from a UGC Admin. This key is not to be shared, as it will be tied to your name/organization. If we find out that the API key is being passed around, then the key will be deleted and technical relations will be terminated.

# API Calls

### Exists
This will return a simple true/false with a given input.  
  
  *example*  
www.ugcleague.com/api/api.php?key=*key_here*&exists=76561198013595660  
will return
```
{"exists":true}
```
---

### Player
Will return a given UGC player's team history and information.

  *example*
www.ugcleague.com/api/api.php?key=*key_here*&player=76561198013595660
will return  
```
{
    "ugc_page": "http://www.ugcleague.com/players_page.cfm?player_id=76561198013595660",
    "team": [{
        "name": "Throwing Harder Than Cy Young",
        "tag": "THTCY",
        "format": "6v6",
        "division": "NA Platinum",
        "status": "HP",
        "last_updated": "2014-07-21 00:00:57",
        "joined": "2013-08-20 04:51:12",
        "active": "true"
    }, {
        "name": "It's in Mumble",
        "tag": "gotem",
        "format": "9v9",
        "division": "NA Silver ",
        "status": "A",
        "last_updated": "2015-05-29 11:52:04",
        "joined": "2015-05-23 08:02:12",
        "active": "true"
    }, {
        "name": "Clan Veni Vidi Vici",
        "tag": "|*V*V*V*|",
        "format": "9v9",
        "division": "NA Steel",
        "status": "I",
        "last_updated": "2014-04-11 02:15:22",
        "joined": "2012-09-04 05:28:00",
        "active": "false"
    }, {
        "name": "Prison Treatment",
        "tag": "?PT?",
        "format": "9v9",
        "division": "NA Silver ",
        "status": "I",
        "last_updated": "2014-04-14 03:45:00",
        "joined": "2013-05-14 23:19:17",
        "active": "false"
    }, {
        "name": "The Nikumaru Counter!",
        "tag": "290'",
        "format": "6v6",
        "division": "NA Steel",
        "status": "I",
        "last_updated": "2013-08-05 01:36:09",
        "joined": "2013-06-02 23:36:38",
        "active": "false"
    }, {
        "name": "Highlander Players",
        "tag": ".hl",
        "format": "9v9",
        "division": "NA Platinum",
        "status": "I",
        "last_updated": "2015-04-27 17:52:51",
        "joined": "2013-04-28 04:45:19",
        "active": "false"
    }, {
        "name": "The Cult of Bill Cosby 2.0: The Squeakwel",
        "tag": "cosB",
        "format": "6v6",
        "division": "NA Gold",
        "status": "HP",
        "last_updated": "2015-02-19 05:43:28",
        "joined": "2013-08-07 03:21:38",
        "active": "false"
    }, {
        "name": "Misfit Mercenaries",
        "tag": "MM",
        "format": "9v9",
        "division": "NA Gold",
        "status": "HP",
        "last_updated": "2014-04-23 01:20:39",
        "joined": "2012-12-17 18:39:21",
        "active": "false"
    }, {
        "name": "The Ringers",
        "tag": "ringer.",
        "format": "9v9",
        "division": "NA Silver ",
        "status": "HP",
        "last_updated": "2014-08-29 20:03:17",
        "joined": "2013-12-23 14:29:50",
        "active": "false"
    }, {
        "name": "Take Five!",
        "tag": "Take Five, !",
        "format": "4v4",
        "division": "Silver N.Amer",
        "status": "I",
        "last_updated": "2014-08-20 02:57:59",
        "joined": "2013-12-23 15:12:38",
        "active": "false"
    }, {
        "name": "The Cult of Bill Cosby 2.0: The Squeakwel",
        "tag": "cosB",
        "format": "6v6",
        "division": "NA Gold",
        "status": "HP",
        "last_updated": "2015-02-19 05:43:28",
        "joined": "2013-08-07 03:21:38",
        "active": "false"
    }, {
        "name": "Pregame Tryhards",
        "tag": "TH",
        "format": "9v9",
        "division": "NA Platinum",
        "status": "DR",
        "last_updated": "2015-05-16 22:24:46",
        "joined": "2011-07-08 08:24:31",
        "active": "false"
    }, {
        "name": "Kawaii Truck",
        "tag": "oo---oo-Bo",
        "format": "6v6",
        "division": "NA Silver",
        "status": "HP",
        "last_updated": "2014-06-08 19:40:10",
        "joined": "2014-04-12 18:13:37",
        "active": "false"
    }, {
        "name": "Take Five!",
        "tag": "Take Five, !",
        "format": "4v4",
        "division": "Silver N.Amer",
        "status": "I",
        "last_updated": "2014-08-20 02:57:59",
        "joined": "2013-12-23 15:12:38",
        "active": "false"
    }, {
        "name": "Orange Juice",
        "tag": "-oj-",
        "format": "9v9",
        "division": "NA Steel",
        "status": "I",
        "last_updated": "2014-08-31 20:57:43",
        "joined": "2014-04-14 17:19:55",
        "active": "false"
    }, {
        "name": "gib Rex",
        "tag": "gR|",
        "format": "9v9",
        "division": "NA Gold",
        "status": "A",
        "last_updated": "2015-05-23 23:42:34",
        "joined": "2013-08-15 23:31:54",
        "active": "false"
    }, {
        "name": "test team 333",
        "tag": "333",
        "format": "9v9",
        "division": "*N.A. New Teams",
        "status": "A",
        "last_updated": "2015-04-28 10:37:06",
        "joined": "2013-12-15 15:48:18",
        "active": "false"
    }]
}
```

Let's break this down. The first element that will be returned is the player's UGC page information. After that, an array of teams that the player was on will be sent. The list is sorted based on whether or not they are active.

Team name:
```
"name": "Throwing Harder Than Cy Young"
```

Team's clan tag:
```
"tag": "THTCY"
```

Format (2v2, 4v4, 6v6, 7v7, 8v8, 9v9)
```
"format": "6v6"
```

Division:
```
"division": "NA Platinum"
```

Status:
```
"status": "HP"
```
Note:
```
A = Active
S = Suspended
NRF = Not Ready due to Forfeit
NR = Not Ready
NC = New Team (Not setup)
HP = Invited From Prior Season
DR = Dropped
I = Inactive
W = Waiting For Next Season
```
Last time the player accessed the UGC page. (Updated their profile, joined, dropped, who knows) [Maybe convert this to epoch?]  
NOTE: This will possibly be removed due to lack of consistancy.
```
"last_updated": "2014-07-21 00:00:57"
```

Time joined: (Maybe convert this to epoch?)  
NOTE: This will possibly be removed due to lack of consistancy.
```
"joined": "2013-08-20 04:51:12"
```

Currently rostered on this team:
```
"active": "true"
```
---
### Current Player
Will return a given UGC player's current team and information. (Note, teams may either be inactive or waiting)

  *example*
www.ugcleague.com/api/api.php?key=*key_here*&current_player=76561198013595660
will return  
```
{
    "ugc_page": "http://www.ugcleague.com/players_page.cfm?player_id=76561198013595660",
    "team": [{
        "name": "Throwing Harder Than Cy Young",
        "tag": "THTCY",
        "format": "6v6",
        "division": "NA Platinum",
        "status": "HP",
        "last_updated": "2014-07-21 00:00:57",
        "joined": "2013-08-20 04:51:12",
        "active": "true"
    }, {
        "name": "It's in Mumble",
        "tag": "gotem",
        "format": "9v9",
        "division": "NA Silver ",
        "status": "A",
        "last_updated": "2015-05-29 11:52:04",
        "joined": "2015-05-23 08:02:12",
        "active": "true"
    }]
}
```
All information from Current Player can be described by Player.

---
### Active Player
Will return a given UGC player's current team and information. (Note, only ACTIVE and CURRENT teams will be listed.)
  *example*
www.ugcleague.com/api/api.php?key=*key_here*&active_player=76561198013595660
will return
```
{
    "ugc_page": "http://www.ugcleague.com/players_page.cfm?player_id=76561198013595660",
    "team": [{
        "name": "It's in Mumble",
        "tag": "gotem",
        "format": "9v9",
        "division": "NA Silver ",
        "status": "A",
        "last_updated": "2015-05-29 11:52:04",
        "joined": "2015-05-23 08:02:12",
        "active": "true"
    }]
}
```
All information from Active Player can be described by Player.

---

### Note  
Feedback is always welcome and appreciated. If you have any requests, please open them as github issues here so we can track them.  
If you would like an API key, please contact me on steam via http://steamcommunity.com/id/BlindSightSniper/ or add another UGC Admin. A list of admins can be found at http://www.ugcleague.com/staff.cfm
