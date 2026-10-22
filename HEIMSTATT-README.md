# Heimstatt-Planer – deutsche Neugestaltung (Entwicklungsstand 3)

Basierend auf aniimax von aebii, MIT-Lizenz (siehe `LICENSE`).

## Bereits umgesetzt
- Responsives Design in `web/heimstatt.css`.
- Deutsch als Standardsprache, Sprachumschaltung bleibt erhalten.
- 264 der 830 englischen Übersetzungsschlüssel sind deutsch hinterlegt.
- Ursprüngliche Produktionsdaten, Rezepte und Berechnungslogik unverändert.
- Alle 26 vorhandenen JavaScript-Tests bestehen (Node.js).

## Noch nicht fertig
- Weitere Texte und Produktnamen müssen übersetzt und im Browser überprüft werden.
- `web/pkg/aniimax.js` und `web/pkg/aniimax_bg.wasm` fehlen: Ohne Rust-/wasm-pack-Kompilierung funktioniert die Optimierung nicht.
- Ein vollständiger Browser-End-to-End-Test ist noch nicht erfolgt.

## Starten nach Kompilierung
Rust und wasm-pack installieren, dann im Projektordner:

```bash
./build-wasm.sh
cd web
python3 -m http.server 8080
```

Danach `http://localhost:8080` öffnen. Direktes Öffnen der HTML-Datei über `file://` reicht nicht.

## Lizenz
Original: aebii, MIT. Lizenztext in `LICENSE`.
