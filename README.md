# camera.combined

A camera platform that give you a combined feed of your defined camera entities.

This will rotated the cameras showing a 10 second feed from each camera before moving along to the next.
  
To get started put `/custom_components/camera/combined.py` here:  
`<config directory>/custom_components/camera/combined.py`  
  
**Example configuration.yaml:**

```yaml
camera:
  platform: combined
  base_address: https://homeassistant.domain.com
  entities:
    - camera.camera1
    - camera.camera1
```

**Configuration variables:**  

key | description  
:--- | :---  
**platform (Required)** | The camera platform name.  
**base_address (Required)** | The base address for yor Home Assistant instanse.
**entities (Required)** | A list of camera entities.
**name (Optional)** | Give the camera a friendly name, defaults to `Combined`.
