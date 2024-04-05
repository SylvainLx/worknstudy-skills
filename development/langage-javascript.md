# Langage Javascript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les `structures` de base du langage ✔️
- les normes `ecmascript` ✔️
- l'utilisation de l'`asynchrone` ✔️
- les spécifités du mot-clef `this` ✔️

## 💻 Je code en Javascript

### Un exemple de code commenté ❌ / ✔️

```javascript
const handlePost = (e) => {
  e.preventDefault();
  const formData = new FormData();

  formData.append("title", title);
  formData.append("name", name);
  formData.append("source", source);
  formData.append("file", name);
  formData.append("description", desc);
  formData.append("speciality", speciality);
  formData.append("theme", theme);
  formData.append("keyword", keyword);
  formData.append("file", photo[0]);
  try {
    axios
      .post(
        `${import.meta.env.VITE_BACKEND_URL}/api/admin/masterclass`,

        formData,
        {
          headers: {
            "Content-Type": "multipart/form-data",
          },
        }
      )
      .then(() => {
        ToastAddMasterclass();
        window.location.reload();
      });
  } catch (err) {
    console.error(err);
    ToastErrorAddMasterclass();
  }
};
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/SylvainLx/Projet_3_MasterWild/)

Description : P-3 de la DWWM,

### J'ai utilisé ce langage en production ❌

[lien du projet](...)

### J'ai utilisé ce langage en environement professionnel ✔️

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
