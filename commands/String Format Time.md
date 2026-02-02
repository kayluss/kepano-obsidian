---
created: 2026-01-22T22:16:00
tags:
  - note
  - journal
---
:put =strftime(‘%Y-%m-%d) 

---

Format String              Example output
-------------              --------------
%c                         Thu 27 Sep 2007 07:37:42 AM EDT (depends on locale)
%a %d %b %Y                Thu 27 Sep 2007
%b %d, %Y                  Sep 27, 2007
%d/%m/%y %H:%M:%S          27/09/07 07:36:32
%H:%M:%S                   07:36:44
%T                         07:38:09
%m/%d/%y                   09/27/07
%y%m%d                     070927
%x %X (%Z)                 09/27/2007 08:00:59 AM (EDT)
%Y-%m-%d                   2016-11-23
%F                         2016-11-23 (works on some systems)

RFC822 format:
%a, %d %b %Y %H:%M:%S %z   Wed, 29 Aug 2007 02:37:15 -0400

ISO8601/W3C format (http://www.w3.org/TR/NOTE-datetime):
%FT%T%z                    2007-08-29T02:37:13-0400