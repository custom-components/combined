This will rotate the camera feeds, showing a 10 second feed from each camera before displaying the next one.

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
**base_address (Required)** | The base address for yor Home Assistant instance.
**entities (Required)** | A list of camera entities.
**name (Optional)** | Give the camera a friendly name, defaults to `Combined`.
