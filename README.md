# EuroDOCSIS3.0_Downstream_stats_checker

This is a spreadsheet for checking the stats of your downstream channels on a DOCSIS 3.0 modem. This is exclusively for EuroDOCSIS (Such as the UK and European countries) and not for the international standard of DOCSIS
which has different values all together. Once you put you stats into the chart it will color highlight them, showing if any are bad by a red color.

If values are red, you should likely contact your ISP.

This applies to all TG2492 telephony modems/routers, or if you have stumbed accross this because you have Virgin Media Broadband, your Virgin Media SuperHub 3.0.
You can find these stats at  http://192.168.0.1/?device_networkstatus&mid=NetworkStatus (this is the Router mode ip address, this is the default if you have not changed the operation mode on your hub) and clicking the Downstream Tab.
If you are using your Virgin Media Hub in Modem mode, you can find these numbers at http://192.168.100.1/?device_networkstatus&mid=NetworkStatus and the same relevant (Downstream) tab.

In the case of power (dBvM) being above the Median (which is the ideal value), you can easily buy a cheap but effective forward path attenuator with the value in dB written on it to get your values closest to the median. Here is an example of a 10dB forward path attenuator (https://www.amazon.co.uk/Apple-Component-Specialist-Forward-Attenuator-Burgaundy-silver/dp/B007FA1JCQ/ref=pd_ybh_a_4?_encoding=UTF8&psc=1&refRID=Y2F794FPAHMX9JH64557). Based on my template of the spreadsheet, I would want a 3db forward path attenuator because my average power (dBvM) is 4.1 dBvM above the ideal median of the range of acceptable volumes for my modulation type (QAM 256).

Keep in mind that as long as the power stats are within the range listed on the right for your modulation; you should not have any connection issues, and that the only reason you would want to try to move your average closer to the ideal median would be for complete optimisation of your internet connection. Also note that these stats are somewhat variable so if you do have dropouts or connection issues, check your router/modem webpage for changes in the values compared to what you put in the spreadsheet.

In the case of power (dBvM) being below the Median, you can buy an amplifier. But I do not recommend this as it has two consequences which is that it amplifies upstream dB as well as downstream dB, which may cause issues with the upstream, and that it also decreases the signal to noise ratio. Unless your downstream dBvM is red, I would recommend leaving this alone, and if it is red. Contact your ISP rather than buying an amplifier.

AN EXPLANATION OF SNR (SIGNAL TO NOISE RATIO): Signal to noise ratio is a measure of how much interferance (or NOISE) is measured in your connection between your modem/router to the node/CMTS (Cable Modulation Termination System). Depending on the modulation type, QAM 256 or QAM 64, the minimum acceptable SNR is listed on the right. If you had a SNR of 30dB, it means that the volume of signal (the good stuff) is 30dB higher than the volume of noise (the bad stuff).

If your SNR (Signal to noise ratio) is below the lowest value of your modems modulation type in the ideal section, you will suffer from packet loss and dropouts. This can be resolved by removing any splitters you may have in the line. But keep in mind if you have a TV box package as well as cable internet then removing a splitter will mean you have no TV box connection.
