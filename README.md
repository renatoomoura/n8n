<p align="center">
	<img src="https://github.com/sufficit/sufficit-quepasa/raw/main/src/assets/favicon.png" alt="Quepasa-logo" width="100" />	
	<p align="center">Quepasa é um software de código aberto, totalmente gratuito, para troca de mensagens com a plataforma Whatsapp</p>
</p>
<hr />
<p align="left">
	<img src="https://telegram.org/favicon.ico" alt="Telegram-logo" width="32" />
	<span>Grupo e Canal Telegram: </span>
	<a href="https://t.me/quepasa_api" target="_blank">Grupo</a>
	<span> || </span>
	<a href="https://t.me/quepasa_channel" target="_blank">Canal</a>
</p>
<hr />
<p align="left">
	<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
	<span>Grupo WhatsaAPP: </span>
	<a href="https://chat.whatsapp.com/Cv5WfmujRzE09yQ6hagYim" target="_blank">Grupo</a>
</p>
----------------------------------------------------------------------------
</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://d33wubrfki0l68.cloudfront.net/b8db213a4d85ebec7b82272cacb727a05a9a1475/96e9f/_images/n8n-docs-icon.svg" alt="Quepasa-logo" width="200" />
</p>

**Manual de Instalação Chatwoot+N8N+Quepasa**

----------------------------------------------------------------------------

**Manual de Instalação N8N**

sudo apt update && apt upgrade -y
</p>
sudo apt-get install -y libgbm-dev wget unzip fontconfig locales gconf-service libasound2 libatk1.0-0 libc6 libcairo2 libcups2 libdbus-1-3 libexpat1 libfontconfig1 libgcc1 libgconf-2-4 libgdk-pixbuf2.0-0 libglib2.0-0 libgtk-3-0 libnspr4 libpango-1.0-0 libpangocairo-1.0-0 libstdc++6 libx11-6 libx11-xcb1 libxcb1 libxcomposite1 libxcursor1 libxdamage1 libxext6 libxfixes3 libxi6 libxrandr2 libxrender1 libxss1 libxtst6 ca-certificates fonts-liberation libappindicator1 libnss3 lsb-release xdg-utils
</p>
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
</p>
sudo apt-get install -y nodejs
</p>
sudo npm install n8n -g
</p>
npm update -g n8n
</p>
npm install pm2 -g
</p>
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
</p>
sudo apt install ./google-chrome-stable_current_amd64.deb
</p>
sudo nano /etc/nginx/sites-available/n8n
</p>
server {
</p>
  server_name n8n.dominio.com.br;
</p>
  location / {
</p>
    proxy_pass http://127.0.0.1:5678;
</p>
    proxy_http_version 1.1;
</p>
    proxy_set_header Upgrade $http_upgrade;
</p>
    proxy_set_header Connection 'upgrade';
</p>
    proxy_set_header Host $host;
</p>
    proxy_set_header X-Real-IP $remote_addr;
</p>
    proxy_set_header X-Forwarded-Proto $scheme;
</p>
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
</p>
    proxy_cache_bypass $http_upgrade;
</p>
    proxy_buffering off;
</p>
    proxy_cache off;
</p>
  }
</p>
  }
</p>
sudo ln -s /etc/nginx/sites-available/n8n /etc/nginx/sites-enabled
</p>
sudo certbot --nginx
</p>
sudo service nginx restart
</p>
pm2 start n8n --cron-restart="0 0 * * *" -- start
</p>

----------------------------------------------------------------------------


----------------------------------------------------------------------------

</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>
----------------------------------------------------------------------------
