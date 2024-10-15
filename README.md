   # DePIN Alliance Farming Bot 
A Python-based automation scripts that uses no API Telegram for interacting with the DePIN Alliance

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/cucumber_scripts)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/cucumber-pickle/Cucumber)

## REGISTER FIRST : [https://t.me/DePIN_Alliance_Bot](https://t.me/DePIN_Alliance_Bot/play?startapp=pLQkN9zUDN)

# Feature 
  - Support for multiple proxy servers
  - Support for multiple telegram accounts
  - Display Menu : run the bot and set your configurations 
  - Instant Setup : save your setup and run easily 
  - Support Random User Agent 
  - Manage the items with the ability to sell items `ON` / `OFF`
  - Completion of Daily Checkin or Available Quest `ON` / `OFF`
  - Upgrade randomly selected skills `ON` / `OFF`
  - Open a cyber box that can be set to the maximum price `ON` / `OFF`
  - Purchase items in the shop that can be set to the maximum price. `ON` / `OFF`
  - Automatically use items that have higher Reward Points 
  - Show Device Equipment : bool `True/False`
  - Can run 24/7 using vps / rdp

## Installation
1. **Clone the Repository:**

   ```bash
   git clone https://github.com/cucumber-pickle/depinCum.git
   cd depinCum
   ```

2. **Create a virtual environment (optional but recommended)**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

   
3. **Install Dependencies:**

The bot uses Python 3 and requires some external libraries. You can install them using:

  ```bash
    pip install -r requirements.txt
  ```


## Configuration

1. **Create a `config.json` file**

    The `config.json` file should be in the root directory of the project. Here is a sample configuration:

    ```json
    {
        "show_device_equipment": false,
        "auto_open_box_max_price": 2000,
        "auto_buy_item_max_price": 2000,
        "sleep_before_start": 5,
        "account_delay": 3,
        "countdown_loop": 500
    }

    ```
    - `show_device_equipment`: set it to `true` to show device equipment 
    - `auto_open_box_max_price`: set a maximum price for the open cyber box
    - `auto_buy_item_max_price`: set a maximum price for the purchased item
    - `sleep_before_start`: the sleep time before running the bot 
    - `account_delay`: Delay between processing each account (in seconds).
    - `countdown_loop`: how long is the waiting time to return to the first account

## Query Setup:

Add your depinCum account tokens to a file named `data.txt` in the root directory. Each token should be on a new line.

Example:
   ```txt
query_id=AA....
user=%7B%22id%....
   ```

## Usage
Run the script with:

   ```bash
python main.py 
   ```

### Instant Setup:
- **Loading setup via CLI argument:** If the `--setup` argument is provided, the script will load the corresponding `.json` file and run the bot directly without displaying the menu.
- **Menu display:** If no `--setup` argument is provided, the script will display the menu as usual.
- **Setup saving:** The option to save setups has been included in the menu as option `8`.

This will allow you to run the script directly with a predefined setup like this:

```bash
python main.py --setup mysetup
```


## How to get tgWebAppData (query_id / user_id)

1. Login telegram via portable or web version
2. Launch the bot
3. Press `F12` on the keyboard 
4. Open console
5. Сopy this code in Console for getting tgWebAppData (user= / query=):

```javascript
copy(Telegram.WebApp.initData)
```

6. you will get data that looks like this

```
query_id=AA....
user=%7B%22id%....
```
7. add it to `data.txt` file or create it if you dont have one


## This bot helpfull?  Please support me by buying me a coffee: 
``` 0xc4bb02b8882c4c88891b4196a9d64a20ef8d7c36 ``` - BSC (BEP 20)

``` UQBiNbT2cqf5gLwjvfstTYvsScNj-nJZlN2NSmZ97rTcvKz0 ``` - TON

``` 0xc4bb02b8882c4c88891b4196a9d64a20ef8d7c36 ``` - Optimism

``` THaLf1cdEoaA73Kk5yiKmcRwUTuouXjM17 ``` - TRX (TRC 20)

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For questions or support, please contact [CUCUMBER TG CHAT](https://t.me/cucumber_scripts_chat)
