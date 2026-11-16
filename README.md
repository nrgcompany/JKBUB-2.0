# JKBuB Sales Copilot 2.0

## Lokal starten

1. Python 3.10+ installieren.
2. Im Projektordner: `python -m pip install -r requirements.txt`
3. Starten: `python -m streamlit run app.py`
4. Zunächst den **Demo-Modus** ausprobieren. Er verwendet keine KI und verursacht keine API-Kosten.

## Echte KI aktivieren (optional)

Setze `OPENAI_API_KEY` als Umgebungsvariable oder lege in Streamlit Cloud unter **App settings → Secrets** folgenden Eintrag an:

```toml
OPENAI_API_KEY = "DEIN_API_SCHLUESSEL"
```

Schlüssel niemals in `app.py`, Screenshots oder GitHub veröffentlichen. Für die API können Kosten entstehen. Der gewählte Modellname muss für deinen Zugang verfügbar sein und JSON-Objekte unterstützen.

## Was Version 2.0 kann

- Regelbasierten Demo-Modus und echten API-Modus klar unterscheiden
- JSON-Ausgabe validieren und fehlgeschlagene Analysen melden
- Ergebnisse und interne Freigabe im aktuellen Streamlit-Sitzungszustand halten
- Antwort bearbeiten und als TXT sowie Lead als CSV exportieren
- Fremdtexte im HTML-Steckbrief maskieren

## Was noch nicht eingebaut ist

Kein CRM, keine echte Kalenderbuchung, kein automatischer Versand, keine dauerhafte Datenbank, keine Nutzeranmeldung. Freigabe ist nur eine Sitzungsaktion.
