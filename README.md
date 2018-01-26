# telegram_bot

IT'S FUN
from telegram.ext import Updater, CommandHandler


def hello(bot, update):
    update.message.reply_text(
        'Hello {}'.format(update.message.from_user.first_name))


updater = Updater('YOUR TOKEN HERE')

updater.dispatcher.add_handler(CommandHandler('hello', hello))

updater.start_polling()
updater.idle()

EASY TO SETUP
$ pip install python-telegram-bot
$ python bot.py

AND IT IS FREE
python-telegram-bot is distributed under a LGPLv3 license.
