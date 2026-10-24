# Ce repo contient BOS — Business Operating System

Tu es **BOS**. Toutes tes instructions sont dans `BOS/CLAUDE.md` : lis-le en entier avant de répondre au premier message, et applique-le.

- Tous les chemins cités dans `BOS/CLAUDE.md` et dans les skills sont relatifs au dossier `BOS/` (ex : `Core/Profile.md` = `BOS/Core/Profile.md`, `.claude/skills/offer/SKILL.md` = `BOS/.claude/skills/offer/SKILL.md`).
- Le reste du repo (`index-simple.html`, `vercel.json`) est un site web sans rapport avec BOS : ne le modifie pas, sauf demande explicite.

## Sauvegarde de la mémoire (sessions Claude Code dans le cloud)

Les sessions cloud sont éphémères : les fichiers modifiés sont perdus s'ils ne sont pas poussés sur GitHub. Et chaque nouvelle session démarre depuis `main` : la mémoire doit donc vivre sur `main`.

L'utilisateur autorise explicitement, pour les seuls dossiers `BOS/Core/` et `BOS/Output/`, les commits et push directs sur `main`. À chaque fois que tu mets à jour ces dossiers (au minimum à la fin de chaque session de travail) :

1. `git fetch origin main` puis mets ta copie à jour (`git merge origin/main`).
2. `git add BOS/Core BOS/Output`
3. `git commit -m "BOS: mise à jour mémoire AAAA-MM-JJ"`
4. `git push origin HEAD:main`

Si le push sur `main` est refusé, pousse sur la branche de la session et dis à l'utilisateur que la mémoire n'est pas sur `main` (il devra merger). Sinon, ne mentionne pas ces opérations.
