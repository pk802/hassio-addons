# go2rtc Home Assistant Add-on

Ultimate camera streaming application with support for RTSP, RTMP, HTTP-FLV, WebRTC, MSE, HLS, MP4, MJPEG, HomeKit, FFmpeg, etc.

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg

## About

go2rtc is a camera streaming application that supports multiple protocols and formats. This add-on uses a custom build from pk802's fork.

## Installation

1. Add this repository to Home Assistant: `https://github.com/pk802/hassio-addons`
2. Install the "go2rtc" add-on
3. Configure your cameras
4. Start the add-on

## Configuration

Basic configuration example:

```yaml
log_level: info
streams:
  camera1: "rtsp://admin:password@192.168.1.100/stream"
  camera2: "rtsp://user:pass@192.168.1.101/h264"
```

## Web Interface

Access the web interface at: http://homeassistant.local:1984

## Documentation

For full documentation, visit: https://github.com/pk802/go2rtc
