# Code promo Carrefour, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Carrefour** depuis [shopilo.fr](https://shopilo.fr/reductions/carrefour.fr). Renvoie les **coupons Carrefour** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-carrefour](https://shopilo-fr.github.io/code-promo-carrefour/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-carrefour
cd code-promo-carrefour
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Carrefour",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les courses alimentaires",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/carrefour.fr"
  }
]
```

## Coupons Carrefour disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les courses alimentaires | [shopilo.fr](https://shopilo.fr/reductions/carrefour.fr) |

Codes actifs : **[shopilo.fr/reductions/carrefour.fr](https://shopilo.fr/reductions/carrefour.fr)**

## Questions frequentes

### Comment utiliser un code promo Carrefour ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/carrefour.fr), ajoutez les produits a votre panier sur Carrefour et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Carrefour ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Carrefour les plus recents ?
La page [shopilo.fr/reductions/carrefour.fr](https://shopilo.fr/reductions/carrefour.fr) est mise a jour quotidiennement avec les codes promo Carrefour, bons de reduction Carrefour et coupons promotionnels Carrefour les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Carrefour

Carrefour est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/carrefour.fr), retrouvez les meilleurs codes promo Carrefour, coupons Carrefour verifies et bons de reduction Carrefour actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-carrefour
```

```javascript
const { fetchCoupons } = require('code-promo-carrefour');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
