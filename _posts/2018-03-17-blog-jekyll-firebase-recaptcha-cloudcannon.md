Dans cet article nous allons apprendre &agrave; cr&eacute;er un blog avec Jekyll, nous ajouterons les commentaires &agrave; l'aide de Firebase et reCaptcha. Ensuite, nous le publierons sur github et pour finir nous le brancherons sur CloudCannon pour avoir un simple et efficace editeur d'article en ligne

Qu'est ce que Jekyll?

Installer et lancer Jekyll

Transformer site statique en site Jekyll

Ajouter le dossier \_layouts

Ajouter le dossier \_posts

Create our first template :

Copier coller le fichier index.html et le d&eacute;placer dans le dossier \_layouts. Le renomme en default.html

Retirer le contenu principal et ajouter la balise&nbsp; {{content}}

Retirer le contenu entre les balises et et ajouter les lignes suivantes

{code}

&nbsp; &nbsp; &nbsp; {% for post in site.posts %}<br>&nbsp; &nbsp; &nbsp; &lt;a href="{{ post.url }}" &nbsp;onclick="w3\_close()" class="w3-bar-item w3-button w3-hover-white"&gt;{{ post.title }}&lt;/a&gt;<br>&nbsp; &nbsp; &nbsp; {% endfor %}<br>{code}