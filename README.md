# python-venv-guide

### Creazione

Crea un ambiente virtuale isolato nella cartella corrente:

```bash
python3 -m venv <nome_env>
```

### Attivazione

Attiva l'ambiente per isolare le dipendenze:

```bash
source <nome_env>/bin/activate
```

*Per disattivare, eseguire il comando `deactivate`.*

### Gestione Dipendenze

* **Esportazione:** Crea un file con la lista delle librerie installate (`pip freeze` legge i pacchetti correnti):
```bash
pip freeze > requirements.txt
```


* **Installazione:** Installa automaticamente tutte le librerie elencate nel file:

```bash
    pip install -r requirements.txt
```

### Rimozione
Gli ambienti virtuali sono interamente contenuti nella propria cartella. Per rimuoverli, è sufficiente eliminare la cartella:
```bash
rm -rf <nome_env>
```

*Assicurarsi di aver eseguito `deactivate` prima di procedere alla cancellazione.*
