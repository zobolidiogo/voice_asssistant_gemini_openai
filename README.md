# Voice Assistant com Gemini, Whisper e gTTS

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge\&logo=google\&logoColor=white)
![Whisper](https://img.shields.io/badge/Whisper-OpenAI-412991?style=for-the-badge)
![gTTS](https://img.shields.io/badge/gTTS-Text%20to%20Speech-brightgreen?style=for-the-badge)

Projeto de assistente do bootcamp GenAI & Dados por voz desenvolvido em Python no Google Colab, integrando tecnologias de Speech-to-Text, geração de respostas com IA e Text-to-Speech para criar uma conversa completa por áudio.

---

## O Desafio

Este projeto foi desenvolvido como parte de um laboratório prático da DIO.
O objetivo era construir um sistema capaz de:

* Gravar áudio do usuário
* Transcrever a fala para texto
* Enviar a pergunta para um modelo de linguagem
* Receber a resposta da IA
* Converter essa resposta novamente em áudio

O tutorial original utilizava a API da OpenAI (ChatGPT) para responder às transcrições de áudio para texto. Entretanto, devido à indisponibilidade de acesso gratuito (e como parte exploratória), adaptei o projeto para utilizar o **Google Gemini/Gemma**, mantendo toda a proposta funcional com ferramentas acessíveis.

---

## A Solução

Foi implementado um pipeline completo de conversação por voz:

1. Captura de áudio no Colab (Python + pequeno trecho em JavaScript)
2. Transcrição utilizando o modelo **Whisper** da OpenAI
3. Geração de resposta com o modelo **Google Gemini/Gemma**
4. Síntese de voz com **gTTS**
5. Reprodução automática do áudio gerado

Fluxo do sistema:

Áudio → Texto (Whisper) → Resposta IA (Gemini) → Áudio (gTTS)

---

## Funcionalidades

* Conversação por voz totalmente funcional
* Suporte a português
* Respostas naturais geradas por IA
* Conversão automática de texto para fala
* Execução simples via Google Colab
* Substituição da OpenAI por Gemini para uso gratuito

---

## Arquivo do Projeto

* assistente_voz_whisper_openai.ipynb – Implementação completa no Google Colab

---

## Como reproduzir o projeto

1. Baixe o arquivo .ipynb
2. Confira se o Colab está conectado em seu Google Drive
   Para fazer isso:
   - Abra o Drive
   - Vá em **+ Novo**
   - Clique em **Mais**
   - Procure por Google Colaboratory
   Caso não esteja instalado:
   - No mesmo local que clicou em **Mais**, clique em **+ Conectar mais apps**
   - Procure por Colaboratory
     Ou
   - Visite o site para instalar o Colaboratory em:
     [workspace.google.com/u/0/marketplace/app/colaboratory/1014160490159?flow_type=2](https://workspace.google.com/u/0/marketplace/app/colaboratory/1014160490159?flow_type=2)
   - Clique em instalar e escolha sua conta @gmail.com
3. Faça upload do arquivo .ipynb no Drive
4. Abra o arquivo com Google Colaboratory
   Com o arquivo aberto:
5. Escolha o idioma no primeiro bloco de comando utilizando o código ISO da linguagem ('pt' = portugês)
6. Siga a sequência de instruções presentes nos códigos
7. Gere sua chave do Google Gemini
   Para gerar sua chave API:
   - Visite o site:
   [https://aistudio.google.com](https://aistudio.google.com)
   - Clique em **Get API key**
   - E então em **Criar chave de API**
8. Com a chave criada em Nível gratuito, guarde o código dela, pois você necessitará para executar algumas células do Colab
9. No Colab, siga as instruções presentes em cada bloco e execute as células na ordem para:

* Escolher idioma
* Gravar áudio
* Transcrever com Whisper
* Gerar resposta com Gemini
* Ouvir retorno em voz com gTTS

---

## Tecnologias Utilizadas

* Python
* Google Colab
* Whisper (Speech-to-Text)
* Google Gemini/Gemma (LLM)
* gTTS (Text-to-Speech)
* JavaScript para captura de áudio

---

## Contato

Diogo Zoboli

Email: [zobolidiogo@gmail.com](mailto:zobolidiogo@gmail.com)

LinkedIn: [linkedin.com/in/zobolidiogo](https://www.linkedin.com/in/zobolidiogo)

---

Se este projeto foi útil, considere dar uma estrela no repositório ⭐
