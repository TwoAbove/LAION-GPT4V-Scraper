# LAION-GPT4V-Scraper 
Pipeline to scrape prompt + image url pairs from LAION `share-gpt4v-images` discord channel

This is currently syncing to huggingface here: [https://huggingface.co/datasets/TwoAbove/LAION-discord-gpt4v](https://huggingface.co/datasets/TwoAbove/LAION-discord-gpt4v)

### Environment Setup

#### Environment Variables (add to your github repo secrets)
- `DISCORD_TOKEN` - Discord bot token with read access and "MESSAGE CONTENT INTENT" toggled on
- `HF_DATASET_NAME` - Name of the dataset to sync to on huggingface
- `HF_TOKEN` - Huggingface token with write access to the dataset

#### config.json
- `channel_id` - ID of the discord channel to scrape
- `limit` - Number of messages to scrape per request
- `hf_dataset_name` - Falback dataset name incase ENV is not set

