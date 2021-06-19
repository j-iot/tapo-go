# Tapo Golang
Library for communicating with Tapo devices

## Example usage:
```go
plug := tapo.New("192.168.1.11", "user@example.com", "your password")

if err := device.Handshake(); err != nil {
  log.Panic(err)
}

if err := device.Login(); err != nil {
  log.Panic(err)
}

device.Switch(false)

deviceInfo, err := device.GetDeviceInfo()
```
