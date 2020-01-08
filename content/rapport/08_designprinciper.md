Designprinciper lab
=======================

Rapporten handlar om hur jag valt att jobba med designprinciper i temat [kmom06-designprinciper](rapport/designprinciper?style=kmom06-designprinciper).

Resonemang
-----------------------
Temat bygger vidare i minimalism och färg-andan. Jag inspirerades av den ux-designerns webbplats som var med i min rapport och ville också testa gul bakgrund.

Jag valde att jobba med kontraster och dominans/emfas som designprinciper. Även balans. Gul bakgrundsfärg med vita h1:or blev en bra början, men för att riktigt skaka om ökade jag storleken på rubrikerna rejält. Det ledde till en del ordbrytningsproblem och jag la därför till word-break: break-all;
word-break: break-word; hyphens: auto; i less-filen för temat under h1 för att komma till bukt med det.

För att ytterligare låta rubrikerna dominera fick all annan text och element en grå färg. Jag provade först med svart men då fick jag inte den effekten utan då tog den över.

Webbplatsen är nu väldigt tung åt vänster. För att lufta upp lite byggde jag lite utrymme mellan bilder och text på en 50px.

Efter det började jag jobba med huvudmenyn för att skapa en slags symmetri (även det designprincip under paraplyet "balans"). Den fick bli vertikal och högerställd och en extra tjocklek på 700. Här fick jag dock snabbt problem med dropdown-menyn som kommer under exempelvis redovisnings-menyvalet. Därför bytte jag spår och gav mig in på att hitta emfas genom att lägga till en textskugga. Den fick en rosa nyans och ganska högt sudd-värde. Detta bidrog också till kontrast även på space-planet eftersom det blir en 3D-känsla.


Referenser
-----------------------

[Wikipedia: Visual_design_elements_and_principles](https://en.wikipedia.org/wiki/Visual_design_elements_and_principles), 2020-01-08

https://css-tricks.com/snippets/css/prevent-long-urls-from-breaking-out-of-container/, 2020-01-08


Övrigt
-----------------------

Rapportförfattare: Julia Johansson.
