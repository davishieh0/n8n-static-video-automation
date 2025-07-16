# n8n-static-video-automation
[Gravar a tela_20250716_142730.webm](https://github.com/user-attachments/assets/67ae8c1e-89ce-4566-906f-da5a6e61a631)

Este workflow n8n automatiza a criação de vídeos estáticos através de um bot do Telegram. O sistema combina imagens e áudios enviados pelos usuários para gerar vídeos de alta qualidade.

Fluxo Principal

Telegram Trigger - Monitora mensagens recebidas no bot
Switch de Classificação - Identifica se a mensagem contém foto, áudio ou outro tipo
Processamento de Mídia - Baixa e armazena os arquivos localmente
Controle de Estado - Usa Supabase para rastrear quais mídias cada usuário já enviou
Verificação de Completude - Checa se o usuário enviou tanto imagem quanto áudio
Geração de Vídeo - Usa FFmpeg para combinar imagem estática com áudio
Entrega - Envia o vídeo final via Telegram
Limpeza - Remove arquivos temporários e limpa o banco

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
