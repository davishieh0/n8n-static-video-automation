# n8n-static-video-automation
[Gravar a tela_20250716_142730.webm](https://github.com/user-attachments/assets/84ee4931-ff8b-4c40-8ee3-ff184d868bcb)

Este workflow n8n automatiza a criação de vídeos estáticos através de um bot do Telegram. O sistema combina imagens e áudios enviados pelos usuários para gerar vídeos de alta qualidade.

🛠️ Componentes Técnicos

Telegram Bot API - Interface de comunicação
Supabase - Banco de dados para controle de estado da fila de mídia
FFmpeg - Processamento de vídeo e áudio
Sistema de Arquivos - Armazenamento temporário dos arquivos

💬 Interação do Usuário

Usuário envia imagem → "Imagem Adicionada"
Usuário envia áudio → "Áudio Enviado"
Sistema possui ambos → Processamento automático
Vídeo final é entregue
Arquivos são limpos automaticamente
