const TelegramBot = require('node-telegram-bot-api');

// Токен вашего бота
const token = '2084317227:AAEGWnpMfAL9qz9YmQNcIpgFXwykl6MF278';

// Создаем объект бота
const bot = new TelegramBot(token, { polling: true });

// Ответ на команду /start
bot.onText(/\/start/, (msg) => {
  const chatId = msg.chat.id;

  // Кнопка для открытия веб-приложения
  const webAppButton = {
    text: "Открыть веб-приложение",
    web_app: {
      url: "https://artemoska.ru"  // Ссылка на ваш сайт
    }
  };

  // Отправляем сообщение с кнопкой
  bot.sendMessage(chatId, "Привет! Нажми на кнопку ниже, чтобы открыть веб-приложение.", {
    reply_markup: {
      inline_keyboard: [[webAppButton]]
    }
  });
});
