# ovehojs
el repositorio oficial de Oveho.js 🎉

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

---

## Embed
Quieres hacer un mensaje `embed`?

Código de guía:

```js
const exampleEmbed = new Discord.MessageEmbed()
	.setColor('#0099ff') //<-- color (embed)
	.setTitle('Some title') //<-- título del embed
	.setAuthor('Some name', 'https://i.imgur.com/wSTFkRM.png', 'https://discord.js.org') //<-- author, author icon y author link (opcional)
	.setDescription('Some description here') //<-- descripción
	.setThumbnail('https://i.imgur.com/wSTFkRM.png') //<-- imagen del thumbnail

	.setImage('https://i.imgur.com/wSTFkRM.png') //<-- imagen del embed
	.setFooter('Texto del footer', 'https://i.imgur.com/wSTFkRM.png'); //<-- icono del footer

channel.send(exampleEmbed);
```
