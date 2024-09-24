```
Hardware used: 
microcontroller board [Adafruit M4 CAN ](https://www.adafruit.com/product/4759), should also work with Adafruit STM32F4 board and a CAN Transceiver. 
lamp: Supernova M99 Pro with Higo 6 pin cable connector.


Test-run:


AN Driver waking up from standby.
CAN power supply booster enabled.
>Sent: COB_ID:0x66f len:4 data:[0x60 0x00 0x00 0x00 ] Func:getname1
Bus state changed to canio.BusState.ACTIVE
<Recv: COB_ID:0x5ef len:8 data:[0x00 0x53 0x55 0x50 0x45 0x52 0x4e 0x4f ] chars: [.SUPERNO]
>Sent: COB_ID:0x66f len:4 data:[0x70 0x00 0x00 0x00 ] Func:getname2
<Recv: COB_ID:0x5ef len:8 data:[0x17 0x56 0x41 0x2d 0x4d 0x39 0x39 0x30 ] chars: [.VA-M990]
>Sent: COB_ID:0x66f len:8 data:[0x40 0x00 0x10 0x00 0x00 0x00 0x00 0x00 ] Func:getdevtype
<Recv: COB_ID:0x5ef len:8 data:[0x43 0x00 0x10 0x00 0x4d 0x39 0x39 0x20 ] chars: [C...M99 ]
>Sent: COB_ID:0x66f len:8 data:[0x40 0x08 0x10 0x00 0x00 0x00 0x00 0x00 ] Func:getfwver
<Recv: COB_ID:0x5ef len:8 data:[0x41 0x08 0x10 0x00 0x0e 0x00 0x00 0x00 ] chars: [A.......]
>Sent: COB_ID:0x0 len:2 data:[0x81 0x00 ] Func:nmtresetall
>Sent: COB_ID:0x0 len:2 data:[0x81 0x6f ] Func:nmtreset
>Sent: COB_ID:0x0 len:2 data:[0x80 0x00 ] Func:nmtpreopall
>Sent: COB_ID:0x0 len:2 data:[0x80 0x6f ] Func:nmtpreop
>Sent: COB_ID:0x0 len:2 data:[0x01 0x00 ] Func:nmtstartall
>Sent: COB_ID:0x0 len:2 data:[0x01 0x6f ] Func:nmtstart
>Sent: COB_ID:0x66f len:8 data:[0x40 0x00 0x22 0x00 0x00 0x00 0x00 0x00 ] Func:get0x2200
<Recv: COB_ID:0x5ef len:8 data:[0x4f 0x00 0x22 0x00 0x06 0x00 0x00 0x00 ] chars: [O.".....]
>Sent: COB_ID:0x66f len:8 data:[0x2b 0x00 0x22 0x00 0x02 0x04 0x00 0x00 ] Func:lbon
<Recv: COB_ID:0x5ef len:8 data:[0x80 0x00 0x22 0x00 0x00 0x00 0x00 0x08 ] chars: [..".....]
>Sent: COB_ID:0x66f len:8 data:[0x2b 0x00 0x22 0x00 0x03 0x00 0x00 0x00 ] Func:hbon
<Recv: COB_ID:0x5ef len:8 data:[0x80 0x00 0x22 0x00 0x00 0x00 0x00 0x08 ] chars: [..".....]
>Sent: COB_ID:0x66f len:8 data:[0x2b 0x00 0x22 0x00 0x02 0x00 0x00 0x00 ] Func:lboff
<Recv: COB_ID:0x5ef len:8 data:[0x80 0x00 0x22 0x00 0x00 0x00 0x00 0x08 ] chars: [..".....]
>Sent: COB_ID:0x66f len:8 data:[0x2b 0x00 0x22 0x00 0x03 0x00 0x00 0x00 ] Func:hboff
<Recv: COB_ID:0x5ef len:8 data:[0x80 0x00 0x22 0x00 0x00 0x00 0x00 0x08 ] chars: [..".....]
```
