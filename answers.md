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

Remove personal info from sidebar
```javascript
$('.bio-info').empty()
```

## Adding Elements to the DOM
Clone Pikachu and insert at bottom
```javascript
$('#right-image img').clone().insertAfter('form')
// or
$('#right-image img').clone().appendTo('section')
```

Repeat last step 10x
```javascript
for ( i=0; i < 10; i++ ) { $('#right-image img').clone().appendTo('section') }
```

Add 'last updated' to sidebar
```javascript
// list item
var listItem = document.createElement('li');
// left span
var leftSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
listItem.appendChild(leftSpan);
// right span
var rightSpan = document.createElement('span');
var date = document.createTextNode(new Date);
rightSpan.appendChild(date);
listItem.appendChild(rightSpan);
// add to ul
var list = document.getElementsByClassName('bio-info')[0]
list.appendChild(listItem)
```
