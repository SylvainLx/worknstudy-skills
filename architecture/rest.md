# REST API

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les verbes HTTP ✔️
- les statuts HTTP ✔️
- les endpoints ✔️
- CORS ✔️
- la nomenclature recommandée pour les routes ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```
const adminRoutes = require("./routes/adminRoutes");


router.post("/masterclass", multer, masterclassController.addOne);
router.get("/masterclass", masterclassController.getAll);
router.get("/masterclass/:id", masterclassController.getOne);
router.put("/masterclass/:id", masterclassController.editOne);
router.delete("/masterclass/:id", masterclassController.deleteOne);

exports.getAll = async (req, res) => {
  try {
    const data = await masterclassController.getAll();
    if (data.length === 0) {
      return res.status(404).send("Aucune masterclass trouvée");
    }
    return res.status(200).json({ data });
  } catch (e) {
    console.warn(e);
    return res.sendStatus(500);
  }
};
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/SylvainLx/Projet_3_MasterWild/tree/main/backend/src)

Description : backend p3 avec les routes, structure mvc utilisant les endpoints, et status http dans les requetes

### Utilisation en production si applicable❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ❌

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
