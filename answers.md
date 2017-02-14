# Hacking Panda The Bear's Resume

1. Change profile picture
```javascript
$('.profile-image').attr('src', 'http://lorempixel.com/400/400/catss')
```

*numbering on Alexa interrupted and reset*

1. Replace sky picture
```javascript
$('#left-image img').attr('src', 'http://lorempixel.com/325/225/nature')
```

2. Change headline
```javascript
$('h1.highlight').text('Garfield')
```

3. Change "Employment" headline
```javascript
$('#employment .info-title').contents().last().replaceWith('&nbsp;Werks I did');
```

4. Remove Time Travel skills
```javascript
$('#time-travel').parent().remove()
```

5. Change background color on <body>
```javascript
$('body').css('background-color', 'silver')
```

6. Change colour of 'highlight' class
```javascript
$('.highlight').css('color', 'navy')
```

7. Change font family of h1 to 'monospace'
```javascript
$('h1').css('font-family', 'monospace')
```
