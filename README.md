# chat_bot_c_sharp
GeekBrains
---

# Создание интеллектуальных чат ботов на C#

### Урок. Введение в практику создания интеллектуальных чат-ботов

'''cs
using Telegram.Bot;
using Telegram.Bot.Args;
using Telegram.Bot.Types;
using Telegram.Bot.Types.Enums;
class Program
{
	private static TelegramBotClient client;	
	static void Main(string[] args)
	{
// token, который вернул BotFather
		client = new TelegramBotClient(token);
		client.OnMessage += BotOnMessageReceived;
		client.OnMessageEdited += BotOnMessageReceived;
		client.StartReceiving();
		Console.ReadLine();
		client.StopReceiving(); 
	} 
private async void BotOnMessageReceived(object sender, MessageEventArgs messageEventArgs)
{
var message = messageEventArgs.Message;         
if (message?.Type == MessageType.TextMessage)
{
await client.SendTextMessageAsync(message.Chat.Id, message.Text);
}
} 
}
'''

![image](https://github.com/user-attachments/assets/3fc79a89-7c13-4eb5-88cb-5da0df7e846d)

![image](https://github.com/user-attachments/assets/8bd353eb-0aa2-44a3-bd07-25b61671291d)

![image](https://github.com/user-attachments/assets/32b565a0-8deb-4c8b-ab82-d5d93cc70868)

![image](https://github.com/user-attachments/assets/39c82111-4368-41e0-9e65-2862c56508c4)

![image](https://github.com/user-attachments/assets/86866b6f-e93d-4c91-8ff8-039746745ab5)

![image](https://github.com/user-attachments/assets/8b0ed17e-8960-4526-a052-71bd19525068)

![image](https://github.com/user-attachments/assets/f56f232c-287b-44ce-9181-c71f9271890e)

![image](https://github.com/user-attachments/assets/f4611377-640f-4b5d-b379-081f4552cb2c)

![image](https://github.com/user-attachments/assets/44e8da01-de34-40c3-b842-2067fc684733)

![image](https://github.com/user-attachments/assets/1e3184b8-2f43-404f-8a50-615a40b2bed6)

![image](https://github.com/user-attachments/assets/a2b90da2-c703-414a-a79b-18fc4af4ff1b)

![image](https://github.com/user-attachments/assets/f8558736-4f7e-4b9c-957b-d2f1611e2378)

![image](https://github.com/user-attachments/assets/e484464c-a833-43e5-ada4-21f4641b976b)

![image](https://github.com/user-attachments/assets/3e870213-8874-4a46-ad44-900e5bf5329c)

![image](https://github.com/user-attachments/assets/27eb50bd-6c80-4542-bae3-37aadcb9356f)

![image](https://github.com/user-attachments/assets/ab155884-0114-411e-aeb6-08ab44ad887a)

