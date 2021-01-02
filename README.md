# ovehojs
<p align:center;>el repositorio oficial de Oveho.js 🎉</p>

**Discord.js** :pager:


- `index.js`
```js
const Discord = require('discord.js');
const client = new Discord.Client();

client.on('ready', () => {
  console.log(`Listo en ${client.user.tag}!`);
});

//comando de ejemplo (ping = pong)

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.reply('Pong!');
  }
});

client.login('TOKEN');
```

- en `TOKEN` pon la token de tu bot. si vas a hacerlo en Repl.it o en glitch.com pon un archivo .env y en `TOKEN`escribe `process.env.TOKEN` 

**Archivo** `.env`:
```
TOKEN=<token>
```

en `<token>` pon la token de tu bot


### instalar el paquete
para instalarlo:
`npm i discord.js`

