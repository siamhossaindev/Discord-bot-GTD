# Discord-bot-GTD

A Discord bot that calculates item values in Garden Tower Defense from unit price changes, built with discord.py and pandas.

![Demo](images/demo.png)

## Features

- `!val` starts an interactive conversation in Discord to value a unit
- Calculates a value from the increase or decrease of a unit's [price/demand/rarity]
- Uses pandas to [load and process the unit data]
- [Any other feature, e.g. handles invalid input, supports multiple units]

### How values are calculated

[One or two sentences, or a short formula. For example: "The bot compares the unit's current price to its previous price and adjusts the base value by the percentage change."]

## Installation

```bash
git clone https://github.com/siamhossaindev/Discord-bot-GTD.git
cd Discord-bot-GTD
pip install -r requirements.txt
```

## Configuration

1. Create a bot in the [Discord Developer Portal](https://discord.com/developers/applications) and copy its token.
2. Copy `.env.example` to `.env`:
   ```bash
   cp .env.example .env
   ```
3. Open `.env` and set your token:
   ```
   DISCORD_TOKEN=your_token_here
   ```

## Usage

Run the bot:

```bash
python bot.py
```

Then, in your Discord server:

| Command | Description |
|---------|-------------|
| `!val`  | Starts a conversation where the bot asks for a unit and its price change, then replies with its value |

**Example**

```
You: !val
Bot: [first question the bot asks]
You: [your answer]
Bot: [the value it returns]
```

## Tech Stack

- Python
- discord.py
- pandas
- python-dotenv
