# 🌟 Portfolio Technique — Stage Fin d'Année (EPSI Paris)

<p align="center">
  <img src="2026-06-27 - NDIAYE -Ndeye Mbasse - 2026-06-27T15_20_16.726Z - Photo_Pro_2.jpg" alt="Ndeye Mbasse Ndiaye" width="150" style="border-radius: 50%; border: 3px solid #8cb89f;"/>
</p>

## 🧑‍💻 À propos de moi
Je m'appelle **Ndeye Mbasse Ndiaye**, étudiante à l'**EPSI Paris**. Passionnée par l'architecture des systèmes, les réseaux et le développement applicatif, j'ai réalisé mon stage de fin d'année en tant que **Développeuse Web / Intégratrice ERP**.

---

## 🏢 Présentation du Stage
* **Entreprise d'accueil :** NET-CO SERVICES (Expertise en nettoyage de copropriétés et services de proximité)
* **Période :** 4 mai au 30 juin 2026
* **Objectif :** Mener à bien la transformation digitale de l'entreprise en concevant un écosystème web unifié (Site vitrine + Boutique e-commerce) entièrement centralisé sur l'ERP **Odoo**, complété par le développement de scripts de personnalisation front-end.

---

## 🛠️ Réalisations Techniques & Codes Sources Personnalisés

Dans cette section, vous trouverez l'ensemble des blocs de code (HTML, CSS et JavaScript) que j'ai conçus et injectés au sein de l'éditeur avancé d'Odoo afin de modifier en profondeur l'expérience utilisateur et l'esthétique graphique de la plateforme.

### 1. Ruban Flottant Latéral Dynamique (Menu d'Action Rapide)
* **Description technique :** Ce module crée un menu flottant sur le bord droit de l'écran (`image_57bd24.png`). Il intègre des formes personnalisées en polygones grâce à la propriété CSS `clip-path`. Un script JavaScript écoute le défilement de la page (scroll) : dès que l'utilisateur descend de plus de 40px, le menu bascule automatiquement en mode **compact** pour libérer de l'espace visuel, puis se redéploie dynamiquement au survol de la souris.

#### 🌐 Structure HTML
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
/* Positionnement global */
#ruban-flottant-netco {
position: fixed !important;
top: 50% !important;
right: 0 !important;
transform: translateY(-50%) !important;
z-index: 99999 !important;
display: flex !important;
flex-direction: column !important;
gap: 10px !important;
}

/* Style de base des boutons */
#ruban-flottant-netco .ruban-btn {
display: flex !important;
align-items: center !important;
justify-content: flex-start !important;
padding: 12px 20px 12px 15px !important;
height: 45px !important;
font-family: 'Inter', sans-serif !important;
font-weight: bold !important;
font-size: 13px !important;
white-space: nowrap !important;
cursor: pointer !important;
text-decoration: none !important;
width: 230px !important;
clip-path: polygon(15px 0%, 100% 0%, 100% 100%, 15px 100%, 0% 50%) !important;
transition: width 0.3s ease, padding 0.3s ease !important;
}

/* Flèches */
#ruban-flottant-netco .fleche {
width: 0 !important;
height: 0 !important;
border-top: 7px solid transparent !important;
border-bottom: 7px solid transparent !important;
margin-right: 12px !important;
display: inline-block !important;
flex-shrink: 0 !important;
}

/* Effet de soulignement dynamique */
#ruban-flottant-netco .texte-btn {
position: relative !important;
}

#ruban-flottant-netco .ruban-btn:hover .texte-btn::after {
content: '' !important;
position: absolute !important;
left: 0 !important;
bottom: -4px !important;
width: 100% !important;
height: 2px !important;
background-color: currentColor !important;
animation: souligner 0.3s forwards !important;
}

@keyframes souligner {
from { width: 0; }
to { width: 100%; }
}

/* Couleurs */
#ruban-flottant-netco .ruban-theme-clair { background-color: #ffe7ce !important; color: #1b3b65 !important; }
#ruban-flottant-netco .ruban-theme-clair .fleche { border-right: 11px solid #1b3b65 !important; }

#ruban-flottant-netco .ruban-vert { background-color: #8cb89f !important; color: #ffffff !important; }
#ruban-flottant-netco .ruban-vert .fleche { border-right: 11px solid #ffffff !important; }

#ruban-flottant-netco .ruban-bleu { background-color: #5d737e !important; color: #ffffff !important; }
#ruban-flottant-netco .ruban-bleu .fleche { border-right: 11px solid #ffffff !important; }

/* Mode compact scroll */
#ruban-flottant-netco.compact .ruban-btn { width: 45px !important; padding: 12px 0px 12px 14px !important; }
#ruban-flottant-netco.compact .texte-btn { display: none !important; }
#ruban-flottant-netco.compact:hover .ruban-btn { width: 230px !important; }
#ruban-flottant-netco.compact:hover .texte-btn { display: inline-block !important; }
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
/* 1. LE FOND VERT DU FORMULAIRE */
section.s_website_form, .s_website_form {
background-color: #8cb89f !important; /* Ton vert */
padding: 40px !important;
border-radius: 15px !important;
}

/* 2. LES TEXTES ET TITRES (BLANCS ET CENTRÉS) */
.s_website_form .col-form-label,
.s_website_form label {
color: #ffffff !important;
font-weight: bold !important;
font-family: Arial, sans-serif !important;
}

/* Forcer le centrage des titres principaux */
.s_website_form .s_website_form_field:not(:has(input[type="checkbox"])):not(:has(input[type="radio"])) .col-form-label {
text-align: center !important;
display: block !important;
width: 100% !important;
font-size: 16px !important;
}

/* 3. L'ENCADREMENT TRANSPARENT DES PRESTATIONS */
.s_website_form .s_website_form_field:has(input[type="checkbox"]) {
border: 2px dashed rgba(255, 255, 255, 0.4) !important;
border-radius: 15px !important;
padding: 20px !important;
background-color: rgba(255, 255, 255, 0.1) !important;
margin-top: 15px !important;
margin-bottom: 20px !important;
}

/* Aligner les petites cases à cocher et ronds à gauche */
.s_website_form .form-check-label {
text-align: left !important;
display: inline-block !important;
}

/* 4. LES CASES DE SAISIE (BLANCHES ET ARRONDIES) */
.s_website_form input.form-control,
.s_website_form textarea.form-control {
background-color: #ffffff !important;
border: none !important;
border-radius: 35px !important; /* Forme pilule */
padding: 12px 20px !important;
color: #1b3b65 !important; /* Écriture bleu marine */
font-weight: bold !important;
}

/* Moins d'arrondi pour la grande zone de texte */
.s_website_form textarea.form-control {
border-radius: 20px !important;
}

/* 5. LE BOUTON DE SOUMISSION (BLANC ET TEXTE VERT) */
.s_website_form .btn-primary,
.s_website_form button,
.s_website_form .s_website_form_send {
background-color: #ffffff !important;
color: #8cb89f !important;
border: none !important;
border-radius: 35px !important;
font-weight: 900 !important;
padding: 15px 40px !important;
box-shadow: 0 4px 15px rgba(0,0,0,0.1) !important;
text-transform: uppercase !important;
}

/* 6. LES DEUX ASTUCES DE CACHAGE / SÉCURITÉ ANTI-SPAM */
/* Masquer la case blanche avec le mot CACHEMOI */
input[placeholder="CACHEMOI"] {
display: none !important;
}

/* Masquer le petit mot "Texte" orange au-dessus du bouton */
.s_website_form .s_website_form_submit label {
display: none !important;
}
<div class="netco-container">
<div class="netco-card">
<div class="icon-circle">
<i class="fa fa-comment"></i>
</div>

<h2 class="title">Parlons de votre projet :<br>obtenez un devis gratuit</h2>
<p class="subtitle">Notre équipe commerciale vous répond rapidement et vous accompagne pour établir un devis adapté à vos besoins.</p>

<div class="contact-box">
<i class="fa fa-envelope-o"></i>
<div class="contact-info">
<span class="label">E-MAIL</span>
<a href="mailto:gestion.netcoservices@gmail.com">gestion.netcoservices@gmail.com</a>
</div>
</div>

<div class="contact-box">
<i class="fa fa-phone"></i>
<div class="contact-info">
<span class="label">TÉLÉPHONE</span>
<a href="tel:+33665798134">(+33) 6 65 79 81 34</a> - <a href="tel:+33760493025">(+33) 7 60 49 30 25</a>
</div>
</div>

<p class="footer-note">Réponse sous 24h ouvrées • Du lundi au vendredi</p>
</div>
</div>
.netco-container { background: #f9f9f9; padding: 40px; display: flex; justify-content: center; }
.netco-card { background: white; max-width: 500px; padding: 40px; border-radius: 15px; text-align: center; box-shadow: 0 4px 15px rgba(0,0,0,0.05); }

.icon-circle { background: #4a5d52; color: white; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 25px; margin: 0 auto 20px auto; }

.title { font-size: 24px; color: #333; margin-bottom: 15px; }
.subtitle { font-size: 14px; color: #666; margin-bottom: 30px; line-height: 1.5; }

.contact-box { display: flex; align-items: center; background: #f4f4f4; padding: 15px; border-radius: 10px; margin-bottom: 10px; text-align: left; }
.contact-box i { font-size: 20px; color: #4a5d52; margin-right: 15px; }
.contact-info .label { display: block; font-size: 10px; font-weight: bold; color: #888; letter-spacing: 1px; }
.contact-info a { color: #333; text-decoration: none; font-weight: bold; }

