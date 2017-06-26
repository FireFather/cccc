# cccc
computer chess tournament broadcast system

CCCC is a complete system for broadcasting chess engine games, matches, or tournaments live on the web.

It consists of two components:  web server (cccc.zip) and tournament broadcast (cccc-live.zip).

Some documentation (a short guide) is also included (cccc-guide.zip).

The web server component uses a customized version of
pgn4web
by Paolo Casaschi
copyright (C) 2009-2016 
http://pgn4web.casaschi.net

The tournament manager component use a customized version of
cutechess-cli
by Ilari Pihlajisto and Arto Jonsson
Copyright (C) 2007-2012 
http://cutechess.com/

Pgn and data files are ftp'd to the web server using
AutoVer 2.2.1
by Hunter Beanland
© 2002-2015 www.beanland.net.au
http://beanland.net.au/AutoVer/

pgn files are processed with a variety of tools and utilites including:

Elostat 1.3
by Frank Schubert

Bayeselo
https://www.remi-coulom.fr/Bayesian-Elo/
by Rémi Coulom

40H-PGN Tools & Utilities
by Norm Pollock
https://40h.000webhostapp.com/

Palview
by Andrew Templeton
http://www.enpassant.dk/chess/palview/

The system aldo includes extensive use of powershell scripts and windows command-line scripts to create, manage, and format comma-delimed text files (results.dat, ratings.dat, etc.).

To set it up:
1. download the web server (cccc.zip), tournament broadcast (cccc-live.zip), and guide (cccc-guide.zip) packages
2. unpack and ftp the web server files to the root subdirecory (/cccc) on any web server
3. unpack the tournament manager files to a root subdirecory (for ex: d:/cccc-live) on any modern Windows PC or server
4. unpack the documentation files to a subdirecory (for ex: d:/cccc-guide) on your Windows PC
5. download Autover, install it, and configure it according to the screenshots located in the d:/cccc-guide/autover subdirectory
6. verify and customize any scripts and paths according to your specific needs

To start a broadcast:

1. edit the cutechess engines.json file as need be (verify the drive letters and paths are correct for your system)
2. edit start.bat to change configure any cutechess tournament parameters
(see cutechess-cli.6.html for details)
3. start autover
4. run the 2 powershell scripts: watch_game.ps1 and watch_games.ps1 (right-click and Run with Powershell)
5. double-click on start.bat

Norman Schmidt
firefather@telenet.be
6/26/2017

