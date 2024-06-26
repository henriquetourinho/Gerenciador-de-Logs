# Gerenciador de Logs

Este é um script em shell para gerenciar logs de sistema. Ele realiza as seguintes tarefas:

1. Move logs antigos para um diretório de arquivo.
2. Compacta logs antigos para economizar espaço.
3. Remove logs antigos após um período de tempo especificado.
4. Envia relatórios de status por email.

## Configuração

### Diretórios e Arquivos

- `LOG_DIR`: Diretório onde os logs estão armazenados.
- `ARCHIVE_DIR`: Diretório para onde os logs antigos serão movidos.
- `LOG_FILE`: Arquivo onde os logs do processo de gerenciamento serão armazenados.

### Variáveis de Configuração

- `EMAIL`: Endereço de email para enviar o relatório.
- `RETENTION_DAYS`: Número de dias após os quais os logs são considerados antigos.

## Como Usar

1. **Baixe o script:**

   Salve o script em um arquivo chamado `gerenciador_de_logs.sh`.

2. **Dependências**

Certifique-se de ter o comando mail configurado corretamente no seu sistema para enviar emails.
Você pode instalar o mail em sistemas baseados em Debian com:<br>
sudo apt-get install mailutils

4. **Torne o script executável:**

   ```bash
   chmod +x gerenciador_de_logs.sh

