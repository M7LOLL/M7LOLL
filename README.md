client.on('message', message => {
  if(message.content === '$afk') {
  message.member.setNickname(` AFK | ${message.author.username}`)
  message.reply('**I Set You AFK 😴**')
  console.table([{ Command: `$afk`, Server: `${message.guild.name}`, Channel: `${message.channel.name}` , Member: `${message.author.username}` }]);
  
}
})
