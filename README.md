# ha-amcrest
Clone of the HomeAssistant core amcrest integration

## How to install on a local Home Assistant instance
Inside your home assistant's `config` directory:
```
cd custom_components
git clone git@github.com:pleasereset/ha-amcrest.git amcrestdev
```

Then use `amcrestdev` instead of HomeAssistant's `amcrest` in your `configuration.yaml`
Example:
```
amcrestdev:
  - name: 'Entrance'
    host: 192.168.2.2
    username: USER_NAME
    password: PASSWORD
    channel: 1
    stream_source: rtsp
    binary_sensors:
      - motion_detected
      - online
  - name: 'Backyard'
    host: 192.168.2.2
    username: USER_NAME
    password: PASSWORD
    channel: 2
    stream_source: rtsp
    binary_sensors:
      - motion_detected
      - online
```