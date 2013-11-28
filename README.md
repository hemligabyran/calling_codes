Calling codes
=============

All international calling codes connected to country / territory

Information about country and area codes taken from http://en.wikipedia.org/wiki/List_of_country_calling_codes and http://en.wikipedia.org/wiki/Telephone_numbers_in_Canada.

Information about territory codes taken from http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2

SQL to get the right territory
------------------------------

    SELECT territory FROM calling_codes WHERE
      prefix = 1284461 OR
      prefix = 128446 OR
      prefix = 12844 OR
      prefix = 1284 OR
      prefix = 128 OR
      prefix = 12 OR
      prefix = 1
    ORDER BY prefix DESC
    LIMIT 1;

The above will return "VG" (Virgin Islands), even though the country code is US/Canada/etc

Updates and/or corrections of this data is very welcome!
