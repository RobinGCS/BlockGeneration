BlockGeneration
A powerful and efficient block regeneration system for Minecraft servers.

BlockGeneration is a robust Spigot/Paper plugin designed for server administrators to manage custom block regeneration in defined regions. Whether you're running a Skyblock, Prison, or custom RPG server, this plugin allows you to define specific areas where broken blocks automatically respawn after a set time, providing a seamless gameplay experience.

🚀 Features
Custom Region Definition: Easily mark regions using a simple selection wand.

Intelligent Regeneration: Automatically restores broken blocks within defined areas after a configured delay.

Inventory Integration: Option to collect broken blocks directly into the player's inventory.

Admin-friendly: Intuitive command structure for managing regions, generators, and configuration.

Performance Focused: Built with asynchronous processing to ensure your server stays lag-free even with many active generators.

Visual Feedback: Particle effects to help admins mark and identify active regions.

⚙️ Installation
Download the latest version of BlockGeneration.jar from the Releases page.

Drop the file into your server's /plugins folder.

Restart your server to generate the default configuration files.

Customize your config.yml and messages.yml to your liking.

Use /bg wand to start defining your regeneration regions!

📋 Configuration & Advanced Features
The config.yml file allows you to fully customize how your generators behave. Below are the key configuration options:

1. Custom Block Transformation
You can define which blocks are transformed when a generator regenerates. By default, the plugin uses COBBLESTONE, but you can change this to any material you prefer.

2. Weighted Drop Percentages
You can add a probability percentage to each block type. This allows you to create custom mining experiences (e.g., higher chances for common blocks, lower for rare ores).

Example config.yml snippet:

generators:
  1:
    blocks:
      - COAL_ORE [90]  # 90% chance to spawn
      - IRON_ORE [20]  # 20% chance to spawn
      - LAPIS_ORE [60] # 60% chance to spawn
    respawn-time: 5    # Time in seconds for the block to regenerate

3. Chest Regeneration
The plugin supports automatic chest contents regeneration. Once a chest is placed within a generator region, it will automatically refill its contents based on your defined loot tables after the specified respawn interval.

📖 How it works
Define: Use the /bg wand to select the corners of your regeneration zone.

Register: Execute /bg add and type the desired generator set ID in the chat.

Enjoy: Once registered, players can break blocks within that area; the plugin will handle the rest, ensuring blocks reappear exactly as they should.

📋 Requirements
Minecraft Version: 1.20+ (Paper/Spigot recommended)

API: Adventure API (Included)

🤝 Support & Contributions
Found a bug or have a feature request? Please feel free to open an Issue here on GitHub or submit a Pull Request.

Built with ❤️ for the Minecraft community.
