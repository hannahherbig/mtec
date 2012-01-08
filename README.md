make an `opts.co` file (well, anything that can be `require('./opts)`'d)

    module.exports =
      main: \#main
      ops: \#ops
      server: 'irc.example.net'
      nick: \bot
      modules: <[ topic factoids ]>
      pass: \nickservpassword

here's the compiled javascript in case you hate coco

    module.exports = {
      main: '#main',
      ops: '#ops',
      server: 'irc.example.net',
      nick: 'bot',
      modules: ['topic', 'factoids'],
      pass: 'nickservpassword'
    };