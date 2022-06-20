# pcap-share
temporary github for pcap share.

* `modbus.pcapng` is orginal capture file filtered on modbus traffic.
* `modbus.log`, `modbus_detailed.log` are zeek logs of the capture file. modbus.log is the standard log produced by zeek
modbus_detailed is the log produced by a zeek plugin: https://github.com/cisagov/icsnpp-s7comm
* `modbus.csv`, `modbus_detail.csv` are the zeek logs converted to csv format for convenience.
* `wireshark_modbus.csv` is a csv export using wireshark.

All timestamps are in unix format in unit of seconds.
The accuracy of the timestamps is up to 6 decimals, meaning 10e-6 seconds or µs.
f.e. unix time => `1593264449.419685`

The number of lines of wireshark_modbus.csv does not correspond with the zeek logs modbus.csv or modbus_detailed.csv.
The timestamps can be used to check which packets (don't) correspond with eachother.
