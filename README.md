# uni5-BA-agent

Agent Business Analyst autonome pour Claude Code.
Lit un cahier des charges et prépare le backlog complet sur GitHub.

## Ce que fait l agent
1. Analyse le CDC en texte libre
2. Détecte le stack automatiquement
3. Pose uniquement les questions bloquantes
4. Présente le backlog pour validation
5. Crée les issues GitHub + board Projects
6. Prépare le handoff vers uni5-dev-agent

## Installation

### Prérequis
- Claude Code (Pro ou Max)
- GitHub CLI authentifié : gh auth login
- MCP GitHub configuré

### Installer le MCP GitHub
```powershell
claude mcp add-json github '{\"type\":\"http\",\"url\":\"https://api.githubcopilot.com/mcp\",\"headers\":{\"Authorization\":\"Bearer TON_TOKEN\"}}'
```

### Cloner et lancer
```powershell
git clone https://github.com/toujaninoura/uni5-BA-agent
code uni5-BA-agent
```
Ouvrir l extension Claude Code (✱) et coller le CDC.

## Utilisation avec uni5-dev-agent
1. Lancer uni5-BA-agent → backlog créé sur GitHub
2. Lancer uni5-dev-agent → développement automatique depuis les issues

## Licence
MIT © toujaninoura
