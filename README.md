<p align="center">
	<img src="https://github.com/EngajamentoFlow/n8n/blob/main/n8n.png" alt="N8N-logo" width="100" />	
	<p align="center">Crie automações complexas 10 vezes mais rápido, sem brigar com APIs</p>
</p>
<hr />
<p align="left">
	<img src="https://telegram.org/favicon.ico" alt="Telegram-logo" width="32" />
	<span>Grupo e Canal Telegram: </span>
	<a href="https://t.me/n8nbr" target="_blank">Grupo</a>
</p>
<hr />
<p align="left">
	<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
	<span>Grupo WhatsaAPP: </span>
	<a href="https://telinkei.com/gp-n8n-zap" target="_blank">Grupo</a>
</p>
----------------------------------------------------------------------------
</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```

----------------------------------------------------------------------------
----------------------------------------------------------------------------

**Manual de Instalação N8N**


</p>
sudo apt update && sudo apt upgrade y
</p>
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
</p>
sudo apt-get install -y nodejs
</p>
node -v
</p>
sudo npm install n8n -g
</p>
npm update -g n8n
</p>
sudo apt install npm
</p>
npm install pm2 -g
</p>
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
</p>
sudo apt install ./google-chrome-stable_current_amd64.deb
</p>
sudo apt install nginx
</p>
sudo nano /etc/nginx/sites-available/n8n
</p>
</p>
</p>

```
server {

  server_name n8n.dominio.com.br;

  location / {

    proxy_pass http://127.0.0.1:5678;

    proxy_http_version 1.1;

    proxy_set_header Upgrade $http_upgrade;

    proxy_set_header Connection 'upgrade';

    proxy_set_header Host $host;

    proxy_set_header X-Real-IP $remote_addr;

    proxy_set_header X-Forwarded-Proto $scheme;

    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;

    proxy_cache_bypass $http_upgrade;

    proxy_buffering off;

    proxy_cache off;

  }

  }
  ```

</p>
</p>
</p>
sudo ln -s /etc/nginx/sites-available/n8n /etc/nginx/sites-enabled
</p>
sudo apt-get install snapd
</p>
sudo snap install notes
</p>
sudo snap install --classic certbot
</p>
systemctl stop apache2.service
</p>
sudo certbot --nginx
</p>
sudo service nginx restart
</p>
pm2 start n8n --cron-restart="0 0 * * *" -- start
</p>
pm2 startup ubuntu -u root & pm2 startup ubuntu -u root --hp /root & pm2 save
</p>
cd 
</p>
export N8N_EDITOR_BASE_URL=https://seudominio.com.br
</p>
</p>
export WEBHOOK_URL=https://seudominio.com.br
</p>
pm2 restart all --update-env
</p>



</p>
export N8N_EDITOR_BASE_URL=https://n8n.socialatendimento.com.br
</p>
export WEBHOOK_URL=https://n8n.socialatendimento.com.br
</p>
pm2 restart all --update-env
</p>


----------------------------------------------------------------------------
----------------------------------------------------------------------------

**Pronto tudo Funcionando**

----------------------------------------------------------------------------
----------------------------------------------------------------------------

</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>


**PIX CNPJ**

```
45959142000119	
```

----------------------------------------------------------------------------
