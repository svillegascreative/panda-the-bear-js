# Hacking Panda The Bear's Resume

Change profile picture
```javascript
$('.profile-image').attr('src', 'http://lorempixel.com/400/400/cats')
```

Replace sky picture
```javascript
$('#left-image img').attr('src', 'http://lorempixel.com/325/225/nature')
```

Change headline
```javascript
$('h1.highlight').text('Garfield')
```

Change "Employment" headline
```javascript
$('#employment .info-title').contents().last().replaceWith('&nbsp;Werks I did');
```

Remove Time Travel skills
```javascript
$('#time-travel').parent().remove()
```

Change background-color on <body>
```javascript
$('body').css('background-color', 'silver')
```

Change color of 'highlight' class
```javascript
$('.highlight').css('color', 'navy')
```

Change font family of h1 to 'monospace'
```javascript
$('h1').css('font-family', 'monospace')
```

Change background-color of round icons in sidebar
```javascript
$('.action-icon-bg').css('background-color', '#00adef')
```

Change placeholder text on name input
```javascript
$('#name').attr('placeholder', 'identify yourself')
```

Change placeholder text on message input
```javascript
$('#message').attr('placeholder', 'state your business')
```

Change value of name input
```javascript
$('#name').attr('value', 'your nemesis')
// or
$('#name').val('your nemesis')
```

Change value of email input
```javascript
$('#email').attr('value', 'koalathebear@gmail.com')
// or
$('#email').val('koalathebear@gmail.com')
```

Change value of submit button
```javascript
$('#submit').attr('value', 'En garde!')
// or
$('#submit').val('En garde!')
```

Disable submit button
```javascript
$('#submit').prop('disabled', true)
```
