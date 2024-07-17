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
export APP_HOST="0.0.0.0"
export APP_PORT=9013
export APP_KEY="test123"
export MODBUS_SERVER_TYPE="tcp"
export MODBUS_CLIENT_TYPE="tcp"
export LOGLEVEL="INFO"
export MODBUS_SERVER_HOST="0.0.0.0"
export MODBUS_SERVER_PORT=8013
export MODBUS_SERVER_MODE=3
export MODBUS_DISPENSE_MODULE="L"
export NET_INTERFACE="wlp1s0"
export MAC="04:7b:cb:bd:07:44"
```