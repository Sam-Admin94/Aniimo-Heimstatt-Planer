# Heimstatt-Planer – deutscher Projektstand

Dies ist der vollständige **Quellcode**, nicht die bereits ausführbare Website.

## Online-Build und Test (GitHub)
1. Neues öffentliches GitHub-Repository anlegen.
2. **Inhalt** dieses Projektordners (nicht den Ordner selbst) hochladen, inklusive `.github`.
3. In GitHub unter **Settings → Pages → Build and deployment** als Source **GitHub Actions** wählen.
4. Unter **Actions → Deutsche Website bauen und veröffentlichen → Run workflow** starten.
5. Nach erfolgreichem Build erscheint die Website-URL im Deployment.

Das Workflow-Skript kompiliert die originale Rust-Engine zu WebAssembly und führt die JavaScript-Tests aus.

## Stand und Einschränkungen
- Deutsche Übersetzungen: 301 von 830 Quelltexten; nicht übersetzte Einträge fallen auf Englisch zurück.
- Originale Engine und Produktionsdaten sind enthalten, aber **nicht kompiliert**.
- Eine vollständig lauffähige Website konnte in dieser Umgebung nicht nachgewiesen werden, da Rust-/WASM-Buildtools und ein Netzwerkzugriff fehlen.
- Bitte keine Fertigstellung oder getestete Funktionsgleichheit annehmen.

Originalprojekt: https://github.com/ae-bii/aniimax (MIT-Lizenz; LICENSE beibehalten).
