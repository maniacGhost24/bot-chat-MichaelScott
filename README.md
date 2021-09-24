# bot-chat-MichaelScott

A GPT-3 Machine Learning model trained on the [Office dialogues dataset](https://www.kaggle.com/nasirkhalid24/the-office-us-complete-dialoguetranscript).

### How does it work?
Built a contextual dataset, which takes the previous seven dialogues before Michael's as context, train it on a small dataset (due to time issue, ideally you would train on a medium dataset, but it would take upwards of 5 hours seeing that Michael has around 11k lines in the whole show). 

The trained model is then hosted on the Hugging Face. [Repo Link](https://huggingface.co/maniacGhost24/MichaelScott-bot-push-small), to test the bot you can even try talking to it in the Hosted API interface in the same repo.

![API Chat Image]<./img/chat.png>

This model is then hosted on a python web server using [Repl](repl.it) which keeps the bot alive even after you close the code link. The code for the server can also be found in the repo.

It is then simply converted into a bot on discord using discord dev tools and is always kept alive using the server.