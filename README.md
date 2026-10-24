# Caldeirão de Vozes

Modificador de voz no navegador: Bruxa, Fantasma, Darth Vader, Robô, Alienígena, Monstro, Demônio, Esquilo, Zumbi, Rádio antigo, Caverna, Narrador de trailer, Locutor FM, Estádio, Megafone, Mago, Gigante, Duende — e as vozes que você criar.

## Como usar

1. Abra https://lpouzada.github.io/caldeirao-de-vozes/ (celular ou computador), ou o `index.html` direto no Chrome, Edge ou Firefox.
2. Clique em **Microfone** e permita o acesso. Use fones para evitar microfonia.
3. Escolha uma voz. Troque à vontade enquanto fala.
4. Ajuste os controles e clique em **Salvar como nova voz** para guardar a sua (fica salva no navegador).
5. **Gravar** salva o áudio transformado (`.webm`) para baixar.

Também dá para **Carregar áudio** (MP3, WAV, OGG, M4A) ou usar a **Voz de teste**.

## Como funciona

Tudo roda localmente com a Web Audio API, sem servidor:

| Etapa | Efeito |
|---|---|
| Tom | Pitch shifter granular (AudioWorklet) com vibrato |
| Timbre | Distorção, filtros passa-alta/passa-baixa, ressonância de "máscara" (filtro pente) |
| Modulação | Modulador em anel (robótico) e tremolo |
| Espaço | Eco com realimentação e reverberação por convolução |

Cada voz é só um conjunto de valores desses controles (veja `BUILT_IN` em `index.html`), então criar uma voz nova é adicionar uma linha.
