---
layout: default
---

# $ cat hakkında.txt
{:id="about"}

r3act0r's madhouse - tımarhaneme hoş geldiniz.

bu oldukça çirkin görünümlü blog sayfasında ayrılık acısı çekenlere uygun atarlı sözler, serseriler için duvar yazıları ve nadiren de son zamanlarda başımıza çıkardıkları siber güvenlik midir nedir o tarz konular hakkında bazı bilgimsi entel dantel yazılar bulacaksınız. 

# $ cat yazılar.txt
{:id="posts"}

<ul>
{% for post in site.categories.posts %}

{% if post.en %}
<li>{{ post.title }} :: <a href="{{ post.url }}" title="{{ post.description }}">[TR]</a> :: <a href="{{ post.pt }}" title="{{ post.description_pt }}">[EN]</a></li>
{% endif %}

{% endfor %}
</ul>

# $ cat konuşmalar.txt

şu anda burada bir şeyler yok, ama çağırırsanız ileride neden olmasın :D 
{:id="talks"}

<ul>
{% for talk in site.categories.talks %}
<li><a href="{{ talk.link }}" title="{{ talk.description }}">{{ talk.title }}</a> at {{ talk.where }}</li>
{% endfor %}
</ul>

# $ cat projeler.txt
{:id="projects"}

<ul>
{% for project in site.categories.projects %}
<li><a href="{{ project.link }}">{{ project.title }}</a> - {{ project.description }}</li>
{% endfor %}
</ul>

# $ cat araçlar.txt
{:id="tools"}

<ul>
{% for tool in site.categories.tools %}
<li><a href="{{ tool.link }}">{{ tool.title }}</a> - {{ tool.description }}</li>
{% endfor %}
</ul>

# $ cat iletişim.txt
{:id="contact"}

beyfendi bilgeliğiniz karşısında hayranlık duyarak sizinle görüşmek istiyorum diyor ve üstün ilmime güvenerek sorular sormak istiyorsanız (birazdan çarpılacağım tövbe estf.) 0xr3act0r[at]tutanota.com adresine mail gönderebilirsiniz. keyfim yeterse bakarım yetmezse bakmam o anki halime bağlı, alınmaca gücenmece yok.

bir şey söylerken kapıyı kimsenin dinlemediğinden emin olun:

pgp public key: [tıklasana evladım](/pgpkey.txt)

