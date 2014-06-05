Animation_library
=================

**Instructions pour utiliser la librairie d'animations CSS "animation_lib_JON_MARTIN.css"**


----------------------------------------------------------


###IL Y A 5 ANIMATIONS EN TOUT:

	.jumpAway
	.inYourFace
	.shakeToFallOut
	.tornadoOut
	.backSuicideOut


----------------------------------------------------------


###POUR LES UTILISER DANS VOTRE PAGE WEB:
 
vous devez d'abord lier la feuille de style "animation_lib_JON_MARTIN.css" 
dans le header de votre page HTML.

Ex:
```html
	<head>
  	  <link rel="stylesheet" type="text/css" href="animation_lib_JON_MARTIN.css">
	</head>
```


----------------------------------------------------------



Vous pouvez ensuite ajoutez la classe de l'animation souhaitée 
(telle que nommée plus haut) à l'élément que vous souhaitez animer.

Ex:
```html
	<body>
	  <div class="jumpAway">
	  </div>
	</body>
```

Votre div sera ainsi animé!


----------------------------------------------------------


###POUR MODIFIER LES PARAMÈTRES D'UNE ANIMATION:

*Les informations suivantes sont aussi dans le fichier css "animation_lib_JON_MARTIN.css"*

Si vous souhaitez modifier des paramètres d'une animation 
(comme la durée, le délai, le nombre de répétitions, etc.), 
placez le code ci-dessous (entre les accollades du "#idOfYourElement") 
dans votre feuille de style CSS dans le id de l'élément que vous souhaitez animer.
(Si l'élément ne possède pas de "id", créez-en un).
Vous pourrez ensuite ajuster les paramètres au goût.


```css
#idOfYourElement{

	-webkit-animation-duration: 1s;		/* Xs or Xms */
	-webkit-animation-delay: 0s;		/* Xs or Xms */
	-webkit-animation-iteration-count: 1;	/* 0 to infinite*/
	-webkit-animation-fill-mode: both;	/* none, forwards, backwards or both */
	-webkit-animation-direction: normal;	/* normal, reverse, alternate, alternate-reverse */
	
	-moz-animation-duration: 1s;
	-moz-animation-delay: 0s;
	-moz-animation-iteration-count: 1;
	-moz-animation-fill-mode: both;
	-moz-animation-direction: normal;

	-ms-animation-duration: 1s;
	-ms-animation-delay: 0s;
	-ms-animation-iteration-count: 1;
	-ms-animation-fill-mode: both;
	-ms-animation-direction: normal;

	-o-animation-duration: 1s;
	-o-animation-delay: 0s;
	-o-animation-iteration-count: 1;
	-o-animation-fill-mode: both;
	-o-animation-direction: normal;

	animation-duration: 1s;
	animation-delay: 0s;
	animation-iteration-count: 1;
	animation-fill-mode: both;
	animation-direction: normal;
}
```


- *Cela ne peut fonctionner que si vous placez les modifications dans un id, car le id est plus fort que la classe.*

- *N'incluez seulement que les paramètres que vous voulez modifier.*

- *N'oubliez pas d'indiquez les préfixes des browsers (-webkit-, -moz-, etc.)*

