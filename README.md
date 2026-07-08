# 🌟 Portfolio Technique — Stage Fin d'Année (EPSI Paris)

<p align="center">
  <img src="2026-06-27 - NDIAYE -Ndeye Mbasse - 2026-06-27T15_20_16.726Z - Photo_Pro_2.jpg" alt="Ndeye Mbasse Ndiaye" width="150" style="border-radius: 50%; border: 3px solid #8cb89f;"/>
</p>

<p align="center">
  <strong>Ndeye Mbasse Ndiaye</strong><br>
  Développeuse Web & Intégratrice ERP — EPSI Paris • Bachelor SIN B1 • 2025-2026
</p>

<p align="center">
  <a href="https://ndiayendeyembasse32-sys.github.io/netco-odoo-project/">🌐 Voir le Portfolio en ligne</a> •
  <a href="mailto:ndiayendeyembasse32@gmail.com">📧 Contact</a> •
  <a href="https://www.linkedin.com/in/ndeye-mbasse-ndiaye-a62281389">💼 LinkedIn</a>
</p>

---

## 🧑‍💻 À propos de moi

Je m'appelle **Ndeye Mbasse Ndiaye**, étudiante à l'**EPSI Paris** en Bachelor SIN (Sciences Informatiques et Numérique). Passionnée par l'architecture des systèmes, les réseaux et le développement applicatif, j'ai réalisé mon stage de fin d'année en tant que **Développeuse Web / Intégratrice ERP** chez NET-CO SERVICES.

---

## 🏢 Présentation du Stage

| | |
|---|---|
| **Entreprise** | NET-CO SERVICES — Nettoyage de copropriétés & services de proximité |
| **Période** | 4 mai → 30 juin 2026 (8 semaines) |
| **Tutrice** | Madame Liliane Lahlouh |
| **Adresse** | 60 rue François 1er, 75008 Paris |
| **SIRET** | 909 421 141 00021 |
| **Mission** | Transformation digitale complète : site vitrine + boutique e-commerce sur Odoo |

---

## ⭐ Appréciation de Stage

> *"Mbasse est une stagiaire sérieuse, autonome et pleinement impliquée. Elle a su prendre l'outil en main rapidement et a travaillé en grande autonomie. La qualité du résultat et sa capacité à avancer sans supervision constante méritent d'être soulignées."*
>
> **— Madame Liliane Lahlouh, Tutrice NET-CO SERVICES**

**Appréciation générale : ✅ Très Satisfaisant**

| Compétence | Niveau |
|---|---|
| A1 — Développement web | ⭐⭐⭐ Niveau 3 (max) |
| A2 — Infrastructure réseau | ⭐⭐⭐ Niveau 3 (max) |
| A4 — Nouvelles technologies | ⭐⭐⭐ Niveau 3 (max) |
| A5 — Veille & documentation | ⭐⭐⭐ Niveau 3 (max) |

---

## 🛠️ Réalisations Techniques

### 1. Site Vitrine — netcopro.com
- 7 pages + modules configurés (Accueil, Services, Recrutement, Blog, Devis, Réclamations, Tarifs)
- Bandeau RGPD & cookies
- Blog SEO avec articles métiers
- Formulaire de devis avec cases à cocher par prestation

### 2. Boutique E-commerce
- Catalogue produits (distributeurs, consommables, matériel)
- Fiches articles complètes avec photos
- Panier opérationnel
- Interconnexion avec le site vitrine

### 3. Personnalisations Front-end avancées

#### 🎨 Ruban Flottant Latéral Dynamique
Menu fixe en bord d'écran avec `clip-path` polygone, mode compact au scroll via JavaScript.

#### 📋 Formulaire de Devis Reskinné
Reskin CSS complet du formulaire Odoo : fond vert, champs pilule, cases prestations en pointillés.

#### 💌 Carte de Contact
Composant HTML/CSS autonome injecté dans l'éditeur Odoo avec liens cliquables.

### 4. Fonctionnalités Semaine 8
- 🎫 **Tickets d'assistance interne** — support IT/RH avec suivi par statut
- 💬 **Live Chat client** — module Odoo intégré sur le site
- 📁 **Gestion Google Drive** — arborescence par service + bibliothèque photos
- 📱 **Réseaux sociaux** — prospection LinkedIn, Facebook, Instagram pro

### 5. Création Graphique — Canva Pro
- **50+ supports graphiques** produits
- Flyers A4 (4 versions design)
- Brochures recto-verso professionnelles
- Stories Instagram (format 9:16)
- Flyer Signalements & Réclamations avec QR code dynamique

---

## 🛠️ Codes Sources Personnalisés

### Ruban Flottant — HTML
```html
<div id="ruban-flottant-netco">
  <a href="/contactus" class="ruban-btn ruban-theme-clair">
    <span class="fleche"></span>
    <span class="texte-btn">CONTACT</span>
  </a>
  <a href="/devis" class="ruban-btn ruban-vert">
    <span class="fleche"></span>
    <span class="texte-btn">DEVIS GRATUIT SOUS 24H</span>
  </a>
  <a href="/jobs" class="ruban-btn ruban-bleu">
    <span class="fleche"></span>
    <span class="texte-btn">REJOIGNEZ-NOUS</span>
  </a>
</div>
```

### Ruban Flottant — JavaScript (scroll listener)
```javascript
(function() {
  var ruban = document.getElementById('ruban-flottant-netco');
  if (ruban) {
    window.addEventListener('scroll', function() {
      if (window.pageYOffset > 40) {
        ruban.classList.add('compact');
      } else {
        ruban.classList.remove('compact');
      }
    });
  }
})();
```

### Formulaire de Devis — CSS
```css
section.s_website_form {
  background-color: #8cb89f !important;
  border-radius: 15px !important;
}
.s_website_form input.form-control {
  border-radius: 35px !important;
  color: #1b3b65 !important;
  font-weight: bold !important;
}
.s_website_form .btn-primary {
  background-color: #ffffff !important;
  color: #8cb89f !important;
  border-radius: 35px !important;
  font-weight: 900 !important;
}
```

---

## 🔗 Liens

- 🌐 **Portfolio** : [ndiayendeyembasse32-sys.github.io/netco-odoo-project](https://ndiayendeyembasse32-sys.github.io/netco-odoo-project/)
- 💼 **LinkedIn** : [Ndeye Mbasse Ndiaye](https://www.linkedin.com/in/ndeye-mbasse-ndiaye-a62281389)
- 📧 **Email** : ndiayendeyembasse32@gmail.com
- 📞 **Téléphone** : +33 7 44 73 85 38

---

*EPSI Paris — Bachelor SIN B1 — Stage 2026 — NET-CO SERVICES*
