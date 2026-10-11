# minecraft-docker

Servidor PaperMC 1.21 (`itzg/minecraft-server`) + túnel Playit.gg con Docker Compose.

## Uso

1. `cp .env.example .env` y pon tu `PLAYIT_SECRET_KEY` (playit.gg → Agents → Add agent → Docker).
2. `docker compose up -d`
3. En playit.gg crea un túnel *Minecraft Java* hacia `127.0.0.1:25565`.

- Logs: `docker compose logs -f`
- Consola: `docker attach mc_paper_server` (salir con Ctrl+P, Ctrl+Q)
- Detener: `docker compose down`

El mundo (`data/`) no se versiona; haz copia aparte.
