# Wolfuxs
Config files for my GitHub profile.
def main():
    print("Bot started...")  # ← Eklendi
    updater = Updater(token=os.environ['TELEGRAM_TOKEN'], use_context=True)
    dp = updater.dispatcher

    dp.add_handler(CommandHandler('start', start))

    updater.start_polling()
    updater.idle()
