# h264extractor
wireshark plugin to extract h264 stream from rtp packets, support Single NAL Unit Mode(RTP Packetization Mode 0),  FU-A and STAP-A

# How to use h264extractor
* Copy rtp_h264_extractor.lua to the directory where wireshark was installed
* edit init.lua,  make sure "disable_lua = false" and add "dofile(DATA_DIR.."rtp_h264_extractor.lua")"
* when open pcap file in wireshark,  decode as RTP and configure the H264 dynamic payload types.  
* Menu - Tools - Extract h264 stream from RTP

# TODO

# Reference
* https://wiki.wireshark.org/Lua
* https://tools.ietf.org/html/rfc6184
