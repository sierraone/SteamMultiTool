Welcome to the repository for the SteamMultiTool.

As of right now, only opportunity buys are supported.

Current features and functions:

1. Pressing *R* starts the script. 
2. Pressing *E* initiates the buy procedure on an open buy dialog 
it's simply a faster way of agreeing to the Steam Subscriber Agreement and hitting Accept. 
This functionality has been built-in to the main script since 0.3, and is therefore deprecated.)
3. Pressing *S* stops the script.

a. The script itself trolls new listings and looks for items (only CS:GO supported at the moment) that are underpriced.
The formula used takes into account market and Steam fees. Parameters can be set using the variables at the beginning of the script.
b. A exponential timer increase has been added to help with HTTP Response 429 - Too many requests. Even so, ~300 queries per day seems to be the maximum.

Planned Features:
1. Incorporate 429 check with actual refresh, cutting queries by half. This should help with 429 errors.
2. Add support for DOTA2.
3. Add support for targeted trawling check (scan through a database of items and alert if any contain underpriced items). **LONGTERM**
