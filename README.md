# Michal's Home Assistant Add-ons

A collection of custom Home Assistant add-ons for various home automation needs.

## 📦 Available Add-ons

### [NEC TV Control](hass-nec-control/)
Control your NEC TV via network commands. Turn your TV on and off remotely through Home Assistant.

**Features:**
- Power on/off control via network
- Configurable TV IP address and port
- REST API for Home Assistant integration
- Automatic device discovery

## 🚀 Installation

### Adding this repository

1. In your Home Assistant instance, go to **Settings** → **Add-ons** → **Add-on Store**
2. Click the three dots in the top right corner
3. Select **Repositories**
4. Add this repository URL: `https://github.com/MichalTorma/ha-repository`
5. Click **Add**

### Installing an add-on

1. Go to **Settings** → **Add-ons** → **Add-on Store**
2. Find the add-on you want to install
3. Click on it and then click **Install**
4. Configure the add-on settings
5. Start the add-on

## 📋 Requirements

- Home Assistant Core 2023.8.0 or newer
- Home Assistant OS or Supervised installation
- Network access to your devices

## 🔧 Configuration

Each add-on has its own configuration options. Please refer to the individual add-on documentation:

- [NEC TV Control Configuration](hass-nec-control/README.md)

## 🐛 Troubleshooting

### Common Issues

1. **Add-on won't install**
   - Ensure you're using a supported Home Assistant installation method
   - Check that the repository URL is correct
   - Verify your Home Assistant version meets the requirements

2. **Add-on won't start**
   - Check the add-on logs for error messages
   - Verify the configuration is correct
   - Ensure all required dependencies are available

3. **Network connectivity issues**
   - Verify your devices are on the same network
   - Check firewall settings
   - Ensure ports are not blocked

### Getting Help

If you encounter issues:

1. Check the add-on logs in Home Assistant
2. Review the add-on specific documentation
3. Create an issue in the repository with:
   - Home Assistant version
   - Add-on version
   - Error logs
   - Steps to reproduce the issue

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup

1. Fork this repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

### Add-on Development Guidelines

When creating new add-ons:

- Follow the [Home Assistant Add-on Development Guidelines](https://developers.home-assistant.io/docs/add-ons/)
- Include comprehensive documentation
- Add proper error handling
- Test on multiple architectures
- Include example configurations

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Home Assistant community for the excellent add-on framework
- Contributors and users who provide feedback and suggestions

## 📞 Support

For support and questions:

- Create an issue in this repository
- Check the [Home Assistant Community](https://community.home-assistant.io/)
- Review the [Home Assistant Documentation](https://www.home-assistant.io/docs/)

---

**Note:** This repository contains custom add-ons. Use at your own risk and always backup your Home Assistant configuration before installing new add-ons.