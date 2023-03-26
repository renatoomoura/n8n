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

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```

**Manual de Instalação API Quepasa**

git clone https://github.com/sufficit/sufficit-quepasa /opt/quepasa-source
</p>
bash /opt/quepasa-source/helpers/install.sh
</p>
sudo apt-get install nginx
</p>
cd /etc/nginx/sites-enabled
</p>
sudo nano /etc/nginx/sites-available/quepasa

</p>

```
server {

  server_name quepasa.dominio.com.br;

  location / {

    proxy_pass http://127.0.0.1:31000;

    proxy_http_version 1.1;

    proxy_set_header Upgrade $http_upgrade;

    proxy_set_header Connection 'upgrade';

    proxy_set_header Host $host;

    proxy_set_header X-Real-IP $remote_addr;

    proxy_set_header X-Forwarded-Proto $scheme;

    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
    
    proxy_cache_bypass $http_upgrade;

  }

  }
```

sudo ln -s /etc/nginx/sites-available/quepasa /etc/nginx/sites-enabled
</p>
</p>
sudo apt-get install snapd
</p>
sudo snap install --classic certbot
</p>
sudo certbot --nginx
</p>
Coloque Email:
</p>
Y
</p>
Y
</p>
sudo certbot --nginx
</p>
sudo service nginx restart
</p>

----------------------------------------------------------------------------

**Ativando SSL da API Quepasa**

nano /opt/quepasa-source/src/.env
</p>
Alterar linha 1
</p>
WEBSOCKETSSL=false
</p>
para
</p>
WEBSOCKETSSL=true
</p>
systemctl restart quepasa
</p>

----------------------------------------------------------------------------

**Instalação Finalizadas**

</p>
quepa.dominio.com.br/setup
</p>
Faça os cadastros em todos eles
</p>
----------------------------------------------------------------------------
</p>
----------------------------------------------------------------------------

**Instalar NO no N8N**

n8n-nodes-chatwoot
</p>
n8n-nodes-quepasa
</p>
Baixar Workflow
</p>
Disponiveis nesse Github
</p>
----------------------------------------------------------------------------
</p>

**Configue os Worflows no N8N**

**Worflow QuepasaQrcode**

</p>
Acesse seuchatwoot/super_admin e crie um token na opção Platform Apps
</p>
Segundo NO “COLOCANDO DADOS" URL N8N, URL DO QUEPASA, URL CHATWOOT, TOKEN TOKEN PLATFORM APPS
</p>
Coloque suas credenciais NOS PostgreSQL, elas estarão em seu .env na pasta /home/chatwoot/chatwoot
</p>
Ligue seu Workflow e divirta-se 

</p>
----------------------------------------------------------------------------
</p>

**Worflows ChatwootToQuepasa QuepasaToChatwoot**

</p>
Adicione numeros NOS Trigger com numeros correspondente a Workflow
</p>
----------------------------------------------------------------------------

**Criando Seu Bot Agente**

Acesse: chatwoot.dominio.com.br/superadmin
</p>
Crie seu Token Platform Apps
</p>
----------------------------------------------------------------------------

**Crie uma Automação conforme a imagem abaixo**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Automa%C3%A7%C3%A3o.png" alt="Automação" width="1000" />
</p>
----------------------------------------------------------------------------

**Criando sua Caixa de Entrada**

Criar um contato no Chatwoot
</p>
Quepasa Control
</p>
control@quepasa.io
</p>
Envia uma mensagem para Contato Criado
</p>
Quepasa Control
</p>
/qrcode
</p>
Leia QRCODE
</p>
----------------------------------------------------------------------------

**Pronto tudo Funcionando**

----------------------------------------------------------------------------

**Comando atualizar API Quepasa**

su - quepasa
</p>
git pull
</p>
exit
</p>
systemctl daemon-reload
</p>

----------------------------------------------------------------------------
----------------------------------------------------------------------------

**Versão Docker**

**Manual de Instalação ChatWoot via Docker**


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
