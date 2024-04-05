# TypeScript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- l'intéret de TypeScript dans l'IDE ✔️
- les types de bases ✔️
- comment et pourquoi étendre une interface ✔️
- les classes et les decorators ✔️

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```
type Props = {
  title: string;
  ads: AdCardProps[];
};
export default function AdCards({ title, ads }: Props) {
  const [cart, setCart] = useState<number>(0);

  return (
    <>
      <h2>{title}</h2>
      <p>Total: {cart}</p>
      <section className={styles["recent-ads"]}>
        {ads.map((ad) => (
          <div key={ad.id}>
            <AdCard
              imgUrl={ad.imgUrl}
              link={`/ads/${ad.id}`}
              price={ad.price}
              title={ad.title}
              key={ad.title}
            />
            <button
              className={styles.button}
              onClick={() => setCart(cart + ad.price)}
            >
              Ajouter au panier
            </button>
          </div>
        ))}
      </section>
    </>
  );
}
```

### Utilisation dans un projet ✔️

[lien github](https://github.com/SylvainLx/Youcode/)

Description : Tutoriel en Next, Typescript

### Utilisation en production si applicable ✔️

[lien du projet](https://sylvainleguay.fr)

Description : Site de mon portfolio

### Utilisation en environement professionnel ✔️

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
