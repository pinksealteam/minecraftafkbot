# MinecraftAFKBot

MinecraftAFKBot is a simple tool designed to prevent AFK detection systems from shutting down your free hosted Minecraft server. This bot is specifically configured for Minecraft version 1.16.4 but can be adapted to other versions via the `settings.json` file. 

## Features

- **Prevents AFK detection**: Ensures your server remains active by preventing AFK kicks.
- **Customizable settings**: Change the bot's username, the server IP, and more through the `settings.json` file.
- **Periodic messaging**: Option to send periodic messages at your chosen interval.
- **Version flexibility**: Adaptable to different Minecraft versions with ViaVersion and ViaBackwards plugins.

## Getting Started

### Prerequisites

- Minecraft server (preferably free hosted)
- Java and Node.js installed on your machine
- ViaVersion and ViaBackwards plugins (if connecting to versions other than 1.16.4)

### Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/Cajger/MinecraftAFKBot.git
    cd MinecraftAFKBot
    ```

2. **Configure settings**:
    - Open the `settings.json` file and adjust the parameters to suit your needs:
        ```json
        {
            "username": "BotUsername",
            "server_ip": "your.server.ip:port",
            "version": "1.16.4",
            "message_interval": 300,
            "messages": [
                "Hello, I'm still here!",
                "I'm human!"
            ]
        }
        ```
    - `username`: The bot's username.
    - `server_ip`: The IP address and port of your Minecraft server.
    - `version`: The Minecraft version to connect to.
    - `message_interval`: Interval in seconds for sending periodic messages.
    - `messages`: Array of messages to send periodically.

3. **Run the bot**:
    ```sh
    java -jar MinecraftAFKBot.jar
    ```

    OR

    ``` 
    node bot.js
    ```

## Troubleshooting

### Connection Issues

If the bot cannot connect due to version issues, try installing the ViaVersion and ViaBackwards plugins on your server. These plugins allow connections from different Minecraft versions:

- **ViaVersion**: Allows newer Minecraft clients to connect to older server versions.
- **ViaBackwards**: Allows older Minecraft clients to connect to newer server versions.

### Plugin Installation

1. **Download ViaVersion and ViaBackwards**:
    - [ViaVersion](https://www.spigotmc.org/resources/viaversion.19254/)
    - [ViaBackwards](https://www.spigotmc.org/resources/viabackwards.27448/)

2. **Install the plugins**:
    - Place the downloaded `.jar` files into your server's `plugins` directory.
    - Restart your server.

## Contributing

Contributions are welcome! If you have any ideas, issues, or improvements, feel free to open an issue or submit a pull request.

## Credits

- **Author**: Cajger
- **Team**: PinkSealTeam

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Enjoy your uninterrupted Minecraft sessions!

