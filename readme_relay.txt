pi relay control
google doc "readme pi irrigation"

------------9/25/21 basic control -----------
configure i2c use raspi-config tool
test:
	turn on channel 1
	i2cset -y 1 0x10 0x01 0xFF
	turn off channel 1
	i2cset -y 1 0x10 0x01 0x00
	turn on channel 4
	i2cset -y 1 0x10 0x04 0xFF
