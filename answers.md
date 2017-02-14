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

4.
