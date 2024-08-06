# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[IGRAJ!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Prije što počnemo, kako *vi* biste željeli čitati?

`publish("show_options_bottom")`

# intro-start-2

n3: Sada, započnimo našu priču...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: OVO JE ČOVJEK

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: I TO JE TJESKOBA ČOVJEKA

n: _TI_ SI TJESKOBI

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ne. Ne, ne, ne slušam. Provjerit ću svoj telefon.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: VAŠ POSAO JE DA ZAŠTITITE SVOG ČOVJEKA OD *OPASNOSTI*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Hej! Pomicate svoj život na Twitteru! Opet!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Da, pitam se zašto samo češće ne sjedim i slušam svoje misli.

`hong({eyes:"neutral"});`

n: BRZO, UPOZORI IH NA *OPASNOST!*

```
bb({eyes:"look"});
```

[O ne, pogledajte tu užasnu vijest!](#act1d_news)

[O ne, je li taj tweet tajno o *nama?*](#act1d_subtweet)

[Hej, GIF mačke koja pije mlijeko](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: He, da, to je slatko, ja--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MAČKE NE MOGU PROBAVITI MLIJEKO, A MI SMO UŽASNI LJUDI KOJI UŽIVAJU U ZLOSTAVLJANJU ŽIVOTINJA

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



