# UPSCALE • PixelProd

Application web d’upscaling vidéo (navigateur) pour tests et intégration dans l’écosystème PixelProd.

| Section | Contenu |
|---|---|
| Objectif | • Importer une vidéo<br>• Lancer un traitement d’upscaling côté client (selon l’implémentation du projet)<br>• Exporter la vidéo traitée |
| Prérequis | • Node.js + npm (ou yarn) |
| Installation | ```bash<br>npm install<br>``` |
| Lancer en développement | ```bash<br>npm run dev<br>``` |
| Build (production) | ```bash<br>npm run build<br>npm run start<br>``` |
| Déploiement | Déployable sur Vercel (ou autre hébergeur compatible Node).<br>Si un fichier `vercel.json` est présent, il pilote la configuration. |
| Structure (indicative) | • `src/` : code application<br>• `public/` : assets statiques (si présent)<br>• `package.json` : scripts et dépendances |
| Installation Instructions (références) | Les points ci-dessous sont des pistes d’intégration/lecture (players + shaders) à adapter selon ta stack réelle.<br>Si tu veux annoncer “supporté officiellement”, il faut valider dans le code ce qui est réellement implémenté. |
| Windows | • (GLSL/MPV)<br>• (GLSL/Plex) |
| Linux | • (GLSL/MPV)<br>• (GLSL/Plex) |
| Mac | • (GLSL/MPV)<br>• (GLSL/IINA)<br>• (GLSL/Plex) |
| Expérimentations (basse résolution) | **v4.1 Low resolution experiment**<br>Résultats issus de tests “SRGAN shaders” pour du 360p → 4K (zoomer pour voir les détails).<br><br>Notes performance (à titre indicatif) :<br>• Les tests peuvent être triés par vitesse d’algorithme, “bicubic” étant généralement le plus rapide.<br>• FSRCNNX et Anime4K peuvent être temps réel selon machine/configuration.<br>• waifu2x et Real-ESRGAN ne sont généralement pas temps réel. |
| Roadmap PixelProd | • Branding UI PixelProd (logo, couleurs, typo)<br>• Page d’accueil + onboarding simple<br>• Paramètres d’upscaling (qualité, vitesse, preset)<br>• Historique des traitements (local)<br>• Export optimisé (format / bitrate) |
