# ESPHome quick start

## Create and activate the virtual environment

From the repository root:

```powershell
python -m venv ..\venv
..\venv\Scripts\Activate.ps1
python -m pip install esphome
```

## Go to the ESPHome configuration directory

```powershell
cd components\iq2020-envoy
```

## Check the configuration

```powershell
esphome config .\JacuzziESP32s3dev.yaml
```

## Build

```powershell
esphome compile .\JacuzziESP32s3dev.yaml
```

## Upload to the device

```powershell
esphome upload .\JacuzziESP32s3dev.yaml --device 192.168.1.20
```

To set an upload timeout, add `--timeout 60`.

## Build and upload

```powershell
esphome run .\JacuzziESP32s3dev.yaml --device 192.168.1.20
```

To set a timeout, add `--timeout 60`.
