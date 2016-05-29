# QuerySolutions

### Starter Theme Structure

<table>
  <tr>
    <th>Folder</th>
    <th>What inside</th>
  </tr>
  <tr>
    <td>inc</td>
    <td>all <code>get_template_part()</code> goes here</td>
  </tr>
  <tr>
    <td>admin</td>
    <td>all "admin side stuff" goes here</td>
  </tr>
  <tr>
    <td>css</td>
    <td>css goes here</td>
  </tr>
  <tr>
    <td>js</td>
    <td>js goes here</td>
  </tr>
  <tr>
    <td>images</td>
    <td>images goes here</td>
  </tr> 
  <tr>
    <td>functions</td>
    <td>theme "plugins" and snippets</td>
  </tr>   
</table>

### Wordpress Security

1) <a href="http://www.groovypost.com/howto/howto/improve-wordpress-securitty-wp-config-php-location/" target="_blank">Moving wp-config.php to secret place</a>

2) <a href="https://paulund.co.uk/move-wp-content-folder-to-different-location" target="_blank">Moving wp-content</a>

### PX to REM
http://codepen.io/liorbabi/pen/QEWOWr


### Magnific popup video + image mixed gallery
```js
	jQuery('.large_slide_thumb a').magnificPopup({
	  type:'image',
	  gallery:{enabled:true},
	  callbacks: {
		elementParse: function(item) {
			//selector with class is_image or is_video
			if(jQuery(item.el).parent().hasClass('is_image') ) {
			 item.type = 'image';
			} else {
			 item.type = 'iframe';
			}
		}
	  }
	});
```
