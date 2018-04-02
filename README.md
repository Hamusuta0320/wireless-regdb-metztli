# wireless-regdb-metztli

This debian source builds updated wireless-regdb suitable for Debian Linux 4.15.15 (4.15.x?)
 as currently not even Unstable (Sid) provides the files needed to prevent error(s) such as:


is an updatedtform regulatory.0: firmware: failed to load regulatory.db (-2)
[   12.134223] firmware_class: See https://wiki.debian.org/Firmware for information about missing firmware
[   12.134281] platform regulatory.0: Direct firmware load for regulatory.db failed with error -2
[   12.134283] cfg80211: failed to load regulatory.db

Specifically, it provides updated files:

/lib/firmware/regulatory.db
/lib/firmware/regulatory.db.p7s
/usr/lib/crda/regulatory.bin

from https://wireless.wiki.kernel.org/en/developers/regulatory/wireless-regdb
