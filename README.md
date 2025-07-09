# Lavalink Server Setup

This workspace contains configuration for running a Lavalink audio node.

## Files

- [`application.yml`](application.yml): Main configuration file for Lavalink.
- `Lavalink.jar`: Lavalink server executable.

## Getting Started

1. **Install Java**  
   Lavalink requires Java 11 or higher. Download and install it from [Adoptium](https://adoptium.net/).

2. **Configure Lavalink**  
   Edit [`application.yml`](application.yml) to set your desired server port and password:
   ```yaml
   server:
     port: '2333' # Replace with your port
   lavalink:
     server:
       password: "yourpassword" # Replace with your password
   ```

3. **Run Lavalink**  
   Open a terminal in this directory and run:
   ```sh
   java -jar Lavalink.jar
   ```

4. **Connect Your Bot**  
   Use the port and password you set in your bot's Lavalink client configuration.

## Configuration Options

- **Sources**: Enable or disable music sources (YouTube, SoundCloud, etc.).
- **Rate Limiting**: Configure IP blocks and retry limits.
- **Metrics**: Prometheus metrics endpoint (disabled by default).
- **Sentry**: Error tracking configuration.

For more details, see the [Lavalink documentation](https://github.com/freyacodes/Lavalink).

## License

See the [Lavalink repository](https://github.com/freyacodes/Lavalink) for license information.
