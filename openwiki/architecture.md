# Guia de Deploy (Easypanel) e Assistente de Voz Nativo (Assist)

## 1. Deploy no Easypanel (VPS)
Se você utiliza o **Easypanel** na sua VPS, pode subir o Home Assistant em menos de 1 minuto:

### Como fazer:
1. Abra o painel do seu **Easypanel**.
2. Crie um novo projeto (ex: `Home Assistant`).
3. Clique em **+ Service** ➔ escolha a opção **Docker Compose** (ou **App Templates** se disponível).
4. Cole o conteúdo do seu [`docker-compose.yml`](../docker-compose.yml).
5. Defina a pasta de montagem de volume (Mapear `/config` para persistir dados).
6. Clique em **Deploy**.
7. O Easypanel gerenciará a porta `8123` e criará o certificado SSL (HTTPS) automaticamente via Traefik!

---

## 2. Usar o Computador/Celular como "Alexa" (Assistente de Voz Nativo: HA Assist)

O Home Assistant possui o seu próprio assistente de voz offline e privado chamado **HA Assist** (Year of the Voice).

### Como transformar seu Computador/Navegador/Celular em uma "Alexa":

1. **Pelo Navegador (Computador/Notebook)**:
   - Abra o Home Assistant no navegador.
   - No canto superior direito, clique no ícone de **Microfone / Bolinha de Conversa**.
   - Fale diretamente pelo microfone do PC: *"Ligar lâmpada do quarto"*, *"Qual a temperatura?"*, *"Desligar a tomada"*.

2. **Pelo Celular (App Home Assistant Companion)**:
   - Baixe o app **Home Assistant** na Play Store / App Store.
   - Conecte ao seu servidor.
   - Você pode colocar um **Widget de voz** na tela inicial do celular ou definir o Home Assistant como o assistente padrão do Android (substituindo o Google Assistente).

3. **Caixa de Som / Microfone Dedicado (Home Assistant Assist Hardware)**:
   - Se quiser um dispositivo físico na mesa (como uma caixa da Alexa que fica sempre escutando a palavra de ativação *"OK Nabu"* ou *"Hey Jarvis"*), você pode usar uma plaquinha **ESP32-S3-BOX** ou **Atom Echo** (custa cerca de R$ 40 - R$ 150) configurada com o ESPhome.
