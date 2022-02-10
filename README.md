# html-boilerplate

## Cand se modifica codul, rulati:

`git add .` adaugam toate fisierele in commit

`git commit -m "mesaj commit" ` salvam stadiul codului cu mesajul "mesaj commit"

`git push ` urcam continutul commitului pe server (origin)

## Daca descarcam prima data codul:

`git clone https://...` creaza o copie a repo-ului de pe github

Aceasta copie are tot istoricul de pe github pentru acest repo.

O data clonat, se poate urca normal, ca la procesul de mai sus

## Daca lucram pe acelasi proiect, pe mai multe device-uri:

Se presupune ca repo-ul a fost clonat pe toate device-urile.

- situatia 1: pe laptop1 s-au modificat fisiere:

Se urca in mod normal pe github cu comenzile de `add`, `commit`, `push`

Pe laptop2 trebuie sincronizat codul. Se va rula:

`git pull` va aduce in local toate schimbarile de pe github

- situatia 2: pe laptop2 s-au modificat si urcat schimbari:

Se urmeaza instructiunile de `add`si `commit`

Inainte de a da `push` se va da un `git pull` pentru a sincroniza ce e local cu ce e pe github

Se poate rula `git push` care va contine modificarile locale si cele de pe github

## Pentru a crea un branch nou:

`git checkout -b nume-branch-fara-space` va crea un branch nou cu numele nume-branch-fara-spaces

Acest branch exista doar local si trebuie creat pe github.

`git push --set-upstream origin nume-branch-fara-spaces` va crea pe github acest branch si va urca pe el schimbarile din local

Din acest moment se poate da `git push` normal
