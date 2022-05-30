# Branch Workflow

## Descrizione
La metodologia di gestione del repository che useremo è una derivazione del **Feature branch Workflow**.
In questa fase del progetto in cui il lavoro implica la stesura di testi e non l'implementazione di feature, useremo 5 branch per gestire il lavoro:

1. master
2. nicolò
3. salvatore
4. andrea
5. gianluigi

Nel branch master risiedera la code base principale del nostro progetto.
Ognuno dei membri del team invece svilupperà il progetto lavorando nel proprio branch.
Quando un branch e pronto ad essere mergiato nella codebase principale l'utente che lo ha sviluppato solleverà una pull request.
Alla pull request seguirà la revisione del codice da parte di almeno un'altro membro del team che darà l'approvazione.
una volta mergiato il branch personale nel master si procederà a cancellare il proprio branch e ricrearlo partendo dal branch master.

## Linee guida

Quelle che seguono sono delle linee guida per l'utilizzo di questo workflow.
1. posizioniamo sul branch master
```
git checkout master
```
2. prima di iniziare a lavorare ci si assicura che il master locale coincida con il master remoto
```
git fetch origin //preleva da dal remote origin i nuovi commit
git reset --hard origin/master //cancella i commit dopo origin/master e posizione il master locale sul master remoto
```
3. creiamo il nostro nuovo branch
```
git checkout -b nome_del_mambro_del_team
```
4. lavoriamo sul nostro codice come di consueto ma pushando sul server remoto i vari commit del nostro branch in modo da renderli disponibili agli altri membri del team
```
git status
git add
git commit -m "commento del commit"
git push origin nome_del_mambro_del_team
```
5. quando crediamo che il nostro lavoro si pronto per essere mergiato nel master andiamo su github e creiamo una pull request.  
   //TODO descirvere la pull request

6. riposizionimoci sul master e cancelliamo il vecchio branch
```
git checkout master
git branch -d nome_del_mambro_del_team
```
7. ricominciamo dal punto 1