from gtts import gTTS

texto = input("Digite algo: ")

if texto == "oi":
    resposta = "Olá! Como posso te ajudar?"
elif texto == "tempo":
    resposta = "Hoje está um ótimo dia!"
else:
    resposta = "Não entendi, mas estou aprendendo!"

print(resposta)

tts = gTTS(resposta, lang='pt-br')
tts.save("resposta.mp3")
