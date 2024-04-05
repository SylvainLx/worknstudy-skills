# GraphQL

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la différence entre REST et GraphQL ✔️
- les besoins auxquels répond GraphQL ✔️
- la définition d'un schéma ✔️
- Query ✔️
- Mutation ✔️
- Subscription ❌

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```
@Resolver()
export class AdResolver {
  @Query((_returns) => [Ad])
  ad(): Promise<Ad[]> {
    return Ad.find();
  }

  @Query((_returns) => Ad)
  adByid(@Arg("id") id: number): Promise<Ad> {
    return Ad.findOneBy({ id });
  }

  @Mutation((_returns) => Ad)
  async updateAd(
    @Arg("id") id: number,
    @Arg("title") title: string,
    @Arg("description") description: string,
    @Arg("price") price: number,
    @Arg("imgUrl") imgUrl: string
  ): Promise<Ad> {
    const ad = await Ad.findOneBy({ id });
    if (!ad) throw new Error("Ad not found!");
    ad.title = title;
    ad.description = description;
    ad.price = price;
    ad.imgUrl = imgUrl;
    await ad.save();
    return ad;
  }
}
```

### Utilisation dans un projet ❌ / ✔️

https://github.com/SylvainLx/good_corner

Description : cas pratique sur l'application de graphql dans un projet full stack

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

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
