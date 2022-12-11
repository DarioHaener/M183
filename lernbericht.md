# Lern-Bericht
Haener Dario

## Einleitung

Zuerst habe ich mit XSS elemente in einer Webseite abgeändert, danach habe ich die Webseite so geändert dass man dagegen geschütz ist.

## Was habe ich gelernt?

Wie man mit hilfe von XSS elemente auf einer Webseite anpassen kann, sowohl auch wie man sich dagegen schützen kann.

## Beschreibung

Das Problem ist, dass die Webseite bei XSS nicht unterscheiden kann, ob es sich bei einer Eingabe um eine normale Eingabe handelt oder um einen Befehl, welche sie ausführen muss. Um sich dagegen zu schützen benötigt man escaping, was Eingaben sozusagen entschärft und immer als normale Eingaben verwendet.

Wenn man escaping explizit ausgestellt hat, kann man es mit `escape="true"` wieder einstellen.
```Java
<h:outputText value="#{value}" escape="true"/>
```

Dies kann man jedoch auch von hand machen, wie in dem unten stehenden Bild.
![image](https://user-images.githubusercontent.com/69902881/206922383-3c4f1d3b-1b50-476c-8fb1-3cc62f348d22.png)

```HTML
<h2>Escaping in Form Feldern (input="text")</h2>
<input style="width: 300px;" value="Sonderzeichen in Value: &quot; &amp; &#39;">
<input style="width: 300px;" value="&quot;onload=&quot; alert(&#39;Kein XSS2!&#39;)&quot;">
```

## Verifikation

Im Bild kann man sehen, dass ich 

# Reflektion zum Arbeitsprozess

👍 Ich konnte dank dem Online Unterricht an meinem Dektop PC arbeiten und war somit effizienter beim Arbeiten. 

👎 Ich musste auf meinem Desktop PC alles so einrichten, dass ich die aufgaben lösen konnte, was etwas aufändig war.

**VBV**: Vielleicht mehr Online Selbststudium Unterricht.
