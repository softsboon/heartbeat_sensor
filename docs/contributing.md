Contributing.md

Link-uri pentru proiect

* Project home: https://github.com/softsboon
* Project main repository: https://github.com/softsboon/heartbeat_sensor
* Project wiki: https://github.com/softsboon/heartbeat_sensor/wiki

--- 
Cum se poate contribui la proiect:

**Linux/Console:**

1. Creezi un cont pe github daca nu ai unul.
2. Trimiti o cerere de access la proiect la adresa: sotsboon@gmail.com cu adresa de email folosita pentru contul de github
3. Dupa acceptarea cererii intri in contul de github si accesezi repositoriului de proiect https://github.com/softsboon/heartbeat_sensor
4. Creeaza un "Fork"
In pagina de Github a repositoriului de proiect se foloseste butonul "Fork" pentru a crea o copie a repositoriului in contul de Github al contributorului.
5. Creeaza o copie locala a proiectului: din pagina repositoriului nou creat, in contul personal de Github, se copiaza url-ul pentru clonarea repositoriului (in general se foloseste link-ul de ssh dar este ok si cel de http)
```sh
git clone git@github.com:USERNAME/FORKED-PROJECT.git
```
6. Adauga link la repo-ul original: din interiorul folderului in care am facut copia locala se adauga o referinta catre repo-ul original (cel din care am facut fork)
```
git remote add upstream https://github.com/UPSTREAM-USER/ORIGINAL-PROJECT.git
```
pentru a verifica daca s-a adaugat aceasta referinta putem folosi comanda
```
git remote -v
```
7. Actualizeaza repo-ul local cu modificarile de pe "upstream": Inainte de a incepe lucrul, trebuie aduse toate modificarile din repo-ul original pentru a lucra pe ultima varianta de cod (acest lucru se va face si inainte de a  trimite modificarile din repo-ul local in repo-ul fork-uit)
```
git fetch upstream 
git merge upstream/master
```
8. Add changes to the local repo
```
git add NUME_FISIER
```
sau 
```
git add . # adauga toate modificarile (staging)
```
9. Salveaza modificarile in repo-ul local
```
git commit -m "Fix issue #123" 
```
10. Actualizeaza repo-ul de pe server: trimite modificarile in repo-ul din contul personal de pe Github
```
git push 
```
11. Create a pull request
    - In pagina de repo din contul de github foloseste butonul de "New pull request"
    - completeti campul de descriere: "Fixed issue #123" si eventual adaugati o descrire a modificarilor.
    - Click pe butonul "Create pull request"
    - Click pe butonul "Merge pull request" (daca sunt conflicte nu va fi activ!)
---
**Windows/MacOS**

1. Creezi un cont pe github daca nu ai unul
2. Trimiti o cerere de access la proiect la adresa: sotsboon@gmail.com cu adresa de email folosita pentru contul de github
3. Dupa acceptarea cererii intri in contul de github si accesezi repositoriului de proiect https://github.com/softsboon/heartbeat_sensor
4. Creeaza un "Fork" In pagina de Github a repositoriului de proiect se foloseste butonul "Fork" pentru a crea o copie a repositoriului in contul de Github al contributorului.
5. Descarca aplicatia "Github Desktop" de [aici](https://desktop.github.com/)
6. Instaleaza aplicatia "Github Desktop". Dupa instalare se poate folosi optiunea "Create a tutorial repository..." care poate fi folosit pentru invatare/teste.
7. Foloseste butonul "Clone a repository from the Internet..." din pagina principala sau optiunea "Clone repository" din meniul "File".
8. In tab-ul "GitHub.com" selecteaza repositoriul de proiect "username/heartbeat_sensor" si apoi apasa butonul "Clone".
9. Nu mai trebuie adaugat link-ul catre repositoriul "upstream" deoarece aplicatia detecteaza daca este vorba de un fork si seteaza acest link automat.
10. Apasa butonul "Fetch origin" pentru a aduce toate modificarile din "softsboon/heartbeat_sensor" in repositoriul local.
11. Adauga fisiere/Modifica fisiere existente la proiect.
12. Deschideti GitHub Desktop si in partea din stanga sus vei gasi lista cu fisierele modificate/adaugate. In partea din stanga jos poti scrie descrierea scurta pentru commit si eventual si o detaliere a modificarilor facute. Apasa commit pentru a salva modificarile in repo-ul local.
13. Pentru a trimite modificarile catre repo-ul din contul tau de GitHub foloseste butonul "Push origin"
14. Foloseste optiunea "Create pull request" din meniul "Branch" care iti va deschide repositoriul de pe GitHub in browser.
15. Create a pull request
    - In pagina de repo din contul de github foloseste butonul de "Create pull request"
    - completeaza campul de descriere: "Fixed issue #123" si eventual adaugati o descrire detaliata a modificarilor.
    - Click pe butonul "Create pull request"
    - Click pe butonul "Merge pull request" (daca sunt conflicte nu va fi activ!)
 
---
Refs

* https://www.youtube.com/watch?v=8UguQzmswC4
* https://medium.com/@swinkler/git-workflow-explained-a-step-by-step-guide-83c1c9247f03
* https://reflectoring.io/github-fork-and-pull/
* https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow

