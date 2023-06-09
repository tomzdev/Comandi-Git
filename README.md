Comandi Git
============

_Un elenco dei miei comandi Git comunemente usati_

--

### Configurazioni di base di git

| Comando | Descrizione |
| ------- | ----------- |
| `git config --global user.name 'Tuo Nome GitHub'` | Configura git con il tuo nome utente  |
| `git config --global user.email email@github.com` | Configura git con il tuo indirizzo mail |

### Creare o clonare progetti

| Comando | Descrizione |
| ------- | ----------- |
| `git init` | Inizializza un repository Git locale |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Crea una copia locale di un repository remoto |

### Snapshot di base

| Comando | Descrizione |
| ------- | ----------- |
| `git status` | Controllare lo stato |
| `git add [file-name.txt]` | Aggiungi un file all'area di staging |
| `git add -A` | Aggiungi tutti i file nuovi e modificati all'area di staging |
| `git commit -m "[commit message]"` | Confermare le modifiche |
| `git rm -r [file-name.txt]` | Rimuovi un file ( o cartella ) |

### Rami e fusione

| Comando | Descrizione |
| ------- | ----------- |
| `git branch` | Elenca i rami ( l'asterisco indica il ramo corrente ) |
| `git branch -a` | Elencare tutti i rami ( locale e remoto ) |
| `git branch [branch name]` | Crea un nuovo ramo |
| `git branch origin [branch name]` | Crea un nuovo ramo remoto |
| `git branch -d [branch name]` | Elimina un ramo |
| `git push origin --delete [branch name]` | Elimina un ramo remoto |
| `git checkout -b [branch name]` | Crea un nuovo ramo e passa ad esso |
| `git checkout -b [branch name] origin/[branch name]` | Clonare un ramo remoto e passare ad esso |
| `git branch -m [old branch name] [new branch name]` | Rinomina una ramo |
| `git checkout [branch name]` | Passa a un ramo |
| `git checkout -` | Passa al ramo verificato l'ultima volta |
| `git checkout -- [file-name.txt]` | Scartare le modifiche in un file |
| `git merge [branch name]` | Unisci un ramo nel ramo attivo |
| `git merge [source branch] [target branch]` | Unisci un ramo in un ramo di destinazione |
| `git stash` | Nascondi le modifiche in una directory di lavoro "sporca" |
| `git stash clear` | Rimuovi tutte le voci nascoste |

### Condivisione e aggiornamento di progetti

| Comando | Descrizione |
| ------- | ----------- |
| `git push origin [branch name]` | Invia un ramo al tuo repository remoto |
| `git push -u origin [branch name]` | Invia le modifiche al repository remoto (e ricorda il ramo) |
| `git push` | Invio delle modifiche al repository remoto (ramo ricordato) |
| `git push origin --delete [branch name]` | Elimina un ramo remoto |
| `git pull` | Aggiorna il repository locale al commit più recente |
| `git pull origin [branch name]` | Aggiorna le modifiche dal repository remoto |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Aggiungi un repository remoto |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Imposta il ramo di origine di un repository su SSH |

### Ispezione e confronto

| Comando | Descrizione |
| ------- | ----------- |
| `git log` | Visualizza le modifiche |
| `git log --summary` | Visualizza modifiche (dettagliate) |
| `git log --oneline` | Visualizza le modifiche (brevemente) |
| `git diff [source branch] [target branch]` | Anteprima delle modifiche prima dell'unione |
