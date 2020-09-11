# EuroDOCSIS3.0_Downstream_stats_checker

This is a spreadsheet for checking the stats of your downstream channels on a DOCSIS 3.0 modem. This is exclusively for EuroDOCSIS (Such as the UK and European countries) and not for the international standard of DOCSIS
which has different values all together. Once you put you stats into the chart it will color highlight them, showing if any are bad by a red color.

If values are red, you should likely contact your ISP.

In the case of dBvM being above the Median (which is the ideal value), you can easily buy a cheap but effective downstream attenuator with the value in dB written on it to get your values closest to the median.

In the case of dBvM being below the Median, you can buy an amplifier. But I do not recommend this as it has two consequences which is that it amplifies upstream dB as well as downstream dB, which may cause issues, and that it also decreases the signal to noise ratio if your SNR is below 50 (which it will be in most cases). Unless your downstream dBvM is red, I would recommend leaving this alone, and if it is red. Contact your ISP rather than buying an amplifier.

If your SNR (Signal to noise ratio) is below the lowest value of your modems modulation type in the ideal section, you will suffer from packet loss and dropouts. This can be resolved by removing any splitters you may have in the line. But keep in mind if you have a TV box package as well as cable internet then removing a splitter will mean you have no TV box connection.
