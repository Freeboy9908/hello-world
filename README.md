# ping
const Discord = require('discord.js');
const client = new Discord.Client();

client.on('ready', () => {
  console.log(`Logged in as ${client.user.tag}!`);
});

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.reply('pong');
  }
});

client.login('NzgwMjM3OTU4NjQ4NDMwNjQ0.X7sLOQ.wsRuXsTvppXZFanKjP4wk0F8d4w');
