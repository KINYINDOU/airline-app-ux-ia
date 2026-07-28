# Projet — App Mobile Compagnie Aérienne : Conception UX/UI assistée par IA

## 📋 Description

Ce projet consiste à concevoir le parcours utilisateur d'une application mobile de compagnie aérienne, en s'appuyant sur des outils d'IA générative pour le wireframing/UI, tout en gardant un regard critique humain sur les résultats produits.

L'objectif pédagogique est double :
- Démontrer une méthodologie de prompting structurée et justifiée
- Montrer un esprit critique face aux limites de l'IA (le point le plus valorisé)

---

## 🎯 1. Personas voyageurs

| Persona | Profil | Besoin clé |
|---|---|---|
| **Amina** | Business, voyage fréquent | Rapidité : check-in en 30s, notifications retard en temps réel, salon d'attente |
| **Moussa** | Famille, 2 enfants | Simplicité : gestion bagages multiples, sièges groupés, aide visuelle claire |
| **Fatou** | Primo-voyageuse | Rassurance : guidage étape par étape, FAQ intégrée, chat support |

**Besoins transverses** : suivi vol en direct, embarquement mobile (QR code), gestion bagages, notifications proactives (retard/porte), accessibilité multilingue (important pour une compagnie africaine).

---

## 🧠 2. Stratégie de prompts

L'approche est construite en trois temps, correspondant à trois usages différents de l'IA.

### Prompt 1 — Cadrage métier
> "Tu es UX designer spécialisé aviation. Pour une appli mobile de compagnie aérienne destinée à [persona], liste les 8 écrans essentiels du parcours voyageur, du booking à l'arrivée, en justifiant l'ordre par la fréquence d'usage."

**Justification** : cadrer le métier avant de demander un visuel évite les propositions génériques (type e-commerce) mal adaptées aux contraintes spécifiques du transport aérien (embarquement, sécurité, retards).

### Prompt 2 — Génération de l'interface
> "Génère l'écran [X] pour [persona], priorité mobile-first, avec [contrainte, ex : mode hors-ligne pour la carte d'embarquement]."

**Justification** : découper la génération écran par écran plutôt que demander l'app entière permet un contrôle qualité à chaque étape et évite l'incohérence entre écrans.

### Prompt 3 — Critique croisée
> "Voici la proposition [décrire/coller]. Identifie 3 faiblesses UX pour un voyageur stressé en zone d'embarquement (lisibilité, rapidité, usage à une main)."

**Justification** : demander à l'IA de critiquer sa propre production révèle des angles morts (accessibilité, contexte d'usage réel) et alimente l'itération suivante.

---

## 📐 3. Structure du rapport

1. **Analyse métier** — personas + parcours utilisateur (jobs-to-be-done)
2. **Stratégie de prompts** — les 3 prompts ci-dessus + justification de l'ordre
3. **V1 générée** — screenshots + critique (2-3 points faibles argumentés)
4. **Itération** — prompt de correction + V2 + ce qui a changé et pourquoi
5. **Justification finale UX/UI** — pourquoi la V2 répond mieux aux besoins des personas
6. **Limites de l'IA constatées** — ce qui a dû être corrigé manuellement (recul critique)

> 💡 Le point 6 est souvent ce qui distingue une bonne copie : montrer un esprit critique face à l'IA, pas juste une génération rapide.

---

## 🔍 4. V1 générée — critique type

Format à suivre pour chaque point faible : **constat → pourquoi c'est un problème pour tel persona → impact concret**

Exemples de points faibles courants :
- Trop d'informations sur l'écran d'accueil → surcharge cognitive pour un voyageur pressé
- Bouton d'action principal (check-in) pas assez visible / mal positionné pour usage à une main
- Texte généré en anglais alors que le persona est francophone/multilingue

---

## 🔄 5. Itération (V1 → V2)

**Prompt de correction envoyé à l'IA :**
> "Simplifie l'écran d'accueil en gardant uniquement 3 actions prioritaires pour [persona], et mets en évidence le bouton [action] en haut de l'écran, atteignable au pouce."

**Changements apportés et pourquoi :**
- Réduction du nombre d'éléments visibles → moins de charge cognitive
- Repositionnement du CTA principal → cohérent avec l'usage réel (une main, en marchant)
- Ajout d'un indicateur de statut de vol en temps réel → répond au besoin transverse identifié en phase 1

---

## ✅ 6. Justification finale UX/UI

La V2 répond mieux aux besoins des personas sur trois axes :

- **Rapidité** : moins de clics pour atteindre l'action prioritaire (check-in, carte d'embarquement)
- **Accessibilité** : hiérarchie visuelle claire, lisible même en situation de stress (zone d'embarquement, luminosité variable)
- **Clarté** : un seul objectif par écran, conforme au principe UX "une action principale par vue"

---

## ⚠️ 7. Limites de l'IA constatées

- Propose des solutions esthétiquement correctes mais parfois **génériques**, sans réelle connaissance des contraintes métier aéroportuaires (procédures de sécurité, timing d'embarquement)
- Tendance à **surcharger l'interface** si le prompt n'est pas assez contraint
- Les propositions doivent être **systématiquement challengées** : l'IA valide rarement ses propres limites sans qu'on le lui demande explicitement (d'où l'intérêt du Prompt 3)
- Le jugement humain reste nécessaire pour trancher entre plusieurs propositions IA contradictoires

> Ce dernier point est celui qui montre au correcteur un usage de l'IA avec un vrai regard critique, et non en mode "copier-coller".

---

## 🛠️ À compléter pendant l'épreuve

- [ ] Captures d'écran réelles V1
- [ ] Captures d'écran réelles V2
- [ ] Détail des points faibles observés (avec captures à l'appui)
