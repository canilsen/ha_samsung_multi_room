# Samsung Multiroom support for HomeAssistant

Control volume, and source of your multiroom device like [Samsung Soundbar K650](https://www.samsung.com/us/televisions-home-theater/home-theater/sound-bars/samsung-hw-k650-soundbar-w-wireless-subwoofer-hw-k650-za/) or [Samsung Soundbar HW-MS650](https://www.samsung.com/us/televisions-home-theater/home-theater/sound-bars/sound--premium-soundbar-hw-ms650-za/) using [HomeAssistant](https://home-assistant.io/)

# Installation

Copy `samsung_multi_room/media_player.py`,`samsung_multi_room/__init__.py` and `samsung_multi_room/manisfest.json` to `<config>/custom_components/samsung_multi_room/` directory. Then add this to your configuration.yaml

``` YAML
media_player:
  - platform: samsung_multi_room
    name: "Soundbar" # name, otherwise it will use name of your soundbar
    host: 192.168.1.227 # ip of your soundbar
    max_volume: 20 # on this level glass breaks, and there are 80 levels more on K650...
```

# Sources

* soundshare - this is tv
* bt - bluetooth
* aux
* optical
* hdmi

# Api support
Based on information gathered from: https://github.com/bacl/WAM_API_DOC/blob/master/API_Methods.md
