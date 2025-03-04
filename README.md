# Home Assistant Chrome Extension

This Chrome extension provides easy and fast access to your Home Assistant dashboard by displaying it in a popup window. It allows you to quickly open your Home Assistant dashboard, making it convenient to monitor and control your smart home devices.

![HA Extension](doc/01-teaser.png)

# Installation

### Download and extract the extension

Download the chrome extension from github:

https://github.com/uwinkler/chrome-ha/archive/refs/heads/main.zip

### Adjust URL

Edit `popup.html` and change the URL of the iframe. It should point to your Home Assistant server.

![Edit popup.htl](doc/02-url.png)

### Configure HA

In Home Assistance, add this following line to your `configuration.yml`:

```yml
http:
  use_x_frame_options: false
```

Otherwise HA will not be shown in the iframe. Restart your HA server

### Load and unpack the extension

1. Go to `chrome://extensions`

2. Enable development mode

![Enabled dev mode](doc/03-enabled-dev.png)

3. Click "Load unpacked"

![Load unpacked](doc/03-load-extension.png)

4. Find you extension and pin it

   ![Pin extension](doc/04-pin.png)

### That's it 🥳
