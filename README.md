# MenteLibera - Rilasci

Eseguibili pronti all'uso di **MenteLibera** (Brain Art generativo per
bambini con disabilita'):

- **Windows**: `MenteLibera-Setup-x.y.z.exe` / `MenteLibera-x.y.z-win64.zip`
- **Android / tablet / Android TV**: `MenteLibera-x.y.z.apk`

I sorgenti sono in un repository privato separato. Questo repo pubblico
contiene **solo i binari** pubblicati tramite [GitHub Releases](../../releases)
e l'app desktop/Android li controlla automaticamente per l'auto-update.

## Come funziona l'auto-update

All'avvio, l'app interroga l'endpoint pubblico delle release di questo
repository:

```
GET https://api.github.com/repos/bdbais/mentelibera-releases/releases/latest
```

Confronta il campo `tag_name` (es. `v1.2.0`) con la propria versione
interna; se piu' recente, propone all'utente di scaricare e installare
l'aggiornamento (asset `.exe`/`.apk` dell'ultima release). Nessun
aggiornamento viene installato automaticamente senza conferma dell'utente.

## Installazione

- **Windows**: scarica l'ultimo `.exe`/`.zip` da [Releases](../../releases) ed eseguilo.
- **Android/tablet/TV**: scarica l'`.apk` da [Releases](../../releases);
  potrebbe essere necessario abilitare "Installa da fonti sconosciute" la
  prima volta (lo store ufficiale verra' valutato in seguito).
