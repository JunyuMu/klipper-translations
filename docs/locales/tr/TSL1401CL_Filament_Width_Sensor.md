# TSL1401CL filament genişlik sensörü

This document describes Filament Width Sensor host module. Hardware used for developing this host module is based on TSL1401CL linear sensor array but it can work with any sensor array that has analog output. You can find designs at [Thingiverse](https://www.thingiverse.com/search?q=filament%20width%20sensor).

To use a sensor array as a filament width sensor, read [Config Reference](Config_Reference.md#tsl1401cl_filament_width_sensor) and [G-Code documentation](G-Codes.md#hall_filament_width_sensor).

## Nasıl çalışıyor?

Sensör, hesaplanan filaman genişliğine göre analog çıkış üretir. Çıkış voltajı her zaman algılanan filaman genişliğine eşittir (Örn. 1,65v, 1,70v, 3,0v). Ana modül voltaj değişikliklerini izler ve ekstrüzyon çarpanını ayarlar

## Note:

Sensor readings done with 10 mm intervals by default. If necessary you are free to change this setting by editing ***MEASUREMENT_INTERVAL_MM*** parameter in **filament_width_sensor.py** file.
