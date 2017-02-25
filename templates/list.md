{% if data  is defined %}
{% for item in data %}
- {{item.tid}} {{item.tname}} {{item.tsize}} {{item.tstatus}} {{item.tdownloaded}}
{% endfor %}
{% if data|length == 0 %}
No torrents scheduled! Please add some!
{% endif %}
{% else %}
Couldn't connect to the transmission server, is it running? 
{% endif %}
