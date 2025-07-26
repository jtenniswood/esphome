# ESPHome Configuration Templates

This repository provides a collection of modular ESPHome configuration templates for various microcontroller boards and sensors. The templates are designed to be easily customizable and maintainable using ESPHome's package system.

## Purpose

This repository serves as a centralized collection of:
- **Base configurations** for popular development boards (M5 Atom, M5 Echo, M5 Nano, Xiao C6)
- **Modular addons** for common sensors and features (Bluetooth, environment sensors, motion detection, etc.)
- **Interface configurations** for communication protocols (I2C)
- **Ready-to-use templates** that combine these components for specific use cases

## Quick Start

The templates in the `templates/` directory are ready to be used directly in ESPHome. Each template pulls configurations from this repository using ESPHome's package system, making updates and maintenance seamless.

### Available Templates

- **M5 Atom** (`templates/m5-atom.yaml`) - Environment and illuminance sensors
- **M5 Echo** (`templates/m5-echo.yaml`) - Echo/voice functionality  
- **M5 Nano** (`templates/m5-nano.yaml`) - Motion sensor
- **Xiao C6** (`templates/xiao-c6.yaml`) - Presence detection with mmWave sensor

### Using a Template

1. Copy any template from the `templates/` directory
2. Customize the `substitutions` section with your device details:
   ```yaml
   substitutions:
     name: "your-device-name"
     friendly_name: "Your Device Name"
     room: "Your Room"
   ```
3. Add your WiFi credentials to your ESPHome secrets
4. Flash to your device

## Repository Structure

```
├── base/           # Base board configurations
├── interface/      # Communication interface configs (I2C, etc.)
├── addon/          # Modular feature addons
└── templates/      # Ready-to-use device templates
```

### Modular Design

The configurations are split into modular components:

- **Base**: Core board setup (pins, basic functionality)
- **Interface**: Communication protocols and pin mappings
- **Addons**: Specific sensors and features that can be mixed and matched
- **Templates**: Pre-configured combinations for common use cases

## Customization

### Fork This Repository

We encourage you to **fork this repository** and customize it to your specific needs:

1. **Fork** this repository to your GitHub account
2. **Clone** your fork locally
3. **Modify** the configurations to match your hardware setup
4. **Update** the repository URLs in the templates to point to your fork
5. **Customize** addons and create new ones for your specific sensors

### Creating Custom Configurations

You can easily create new configurations by:

1. **Mixing addons**: Combine different addon modules in your packages
2. **Creating new addons**: Add new sensor configurations in the `addon/` directory
3. **Custom templates**: Create new templates for your specific board/sensor combinations
4. **Override settings**: Use ESPHome's package override functionality

## Benefits of This Approach

- **Maintainable**: Update configurations in one place, all devices benefit
- **Modular**: Mix and match features as needed
- **Version controlled**: Track changes and roll back if needed
- **Shareable**: Easy to share configurations with the community
- **Scalable**: Manage configurations for many devices efficiently

## Contributing

If you've created useful configurations or improvements:

1. Fork this repository
2. Create your custom configurations
3. Consider submitting a pull request to share with the community

## Getting Started with ESPHome

If you're new to ESPHome, check out the [official documentation](https://esphome.io/) to learn more about this powerful framework for microcontroller programming.

## Support

For ESPHome-specific questions, refer to the [ESPHome documentation](https://esphome.io/) and [community forums](https://community.home-assistant.io/c/esphome).

---

**Happy coding!** 🚀 Fork this repository and make it your own! 