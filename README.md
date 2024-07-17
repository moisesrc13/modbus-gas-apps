# Modbus server apps

## Config Service
```bash
sudo cp modbus-client.service /etc/systemd/system/
sudo systemctl daemon-reload
sudo systemctl enable modbus-client.service
sudo systemctl status modbus-client.service
sudo systemctl start modbus-client.service
```

## Env vars
```bash
APP_HOST="0.0.0.0"
APP_PORT=9013
APP_KEY="test123"
MODBUS_SERVER_TYPE="tcp"
MODBUS_CLIENT_TYPE="tcp"
LOGLEVEL="INFO"
MODBUS_SERVER_HOST="0.0.0.0"
MODBUS_SERVER_PORT=8013
MODBUS_SERVER_MODE=3
MODBUS_DISPENSE_MODULE="L"
NET_INTERFACE="wlp1s0"
MODBUS_SERVER_MODE=3
MODBUS_DISPENSE_MODULE="H"
```

## Additional config for modbus

```bash
MODBUS_SERIAL_PORT="/dev/ptyp0"  # RJ485 WILL BE THE DEFAULT CONNECTION FOR MODBUS SERVER
MODBUS_SERIAL_BAUDRATE="19200"
MODBUS_SERIAL_DATA_BIT="8"
MODBUS_SERIAL_STOP_BIT="1"
MODBUS_SERIAL_PARITY="N"
MODBUS_TIMEOUT_SECONDS="15"
MODBUS_SERVER_MODE="2"  # 2, 3, 4
MODBUS_DISPENSE_MODULE="L"  # L, H
```