# GitHub Copilot tokeni leidmine

GitHub Copilot kasutamiseks on vaja genereerida isiklik juurdepääsutunnus (Personal Access Token ehk PAT).

---

## 🔑 Mis on GitHub Copilot token?

GitHub Copilot token on isiklik juurdepääsutunnus (PAT), mida kasutatakse GitHub Copilot API-le ligipääsemiseks. Seda läheb vaja näiteks siis, kui soovid kasutada Copiloti otse koodiredaktoris (nt VS Code) või mõnes muus rakenduses.

---

## 📋 Eeltingimused

- Aktiivne GitHub konto
- GitHub Copilot tellimus (Individual, Business või Enterprise)
  - Tellimuse saad aktiveerida aadressil: [github.com/features/copilot](https://github.com/features/copilot)

---

## 🛠️ Samm-sammult juhend

### 1. Ava GitHubi seaded

1. Logi sisse oma GitHubi kontole aadressil [github.com](https://github.com).
2. Klõpsa paremas ülanurgas oma profiilipildil.
3. Vali rippmenüüst **Settings** (Seaded).

### 2. Ava arendajaseaded

1. Keri lehekülje allossa.
2. Klõpsa vasakul menüüs **Developer settings** (Arendajaseaded).

### 3. Loo uus token

1. Vali vasakult **Personal access tokens** → **Tokens (classic)**.
2. Klõpsa **Generate new token** → **Generate new token (classic)**.
3. Anna tokenile nimetus (nt `copilot-token`).
4. Vali aegumisaeg vastavalt vajadusele.
5. Vali õigused (**scopes**) – Copiloti jaoks piisab tavaliselt:
   - `read:user`
   - `user:email`
6. Klõpsa **Generate token**.

### 4. Kopeeri token

> ⚠️ **Tähelepanu!** Token kuvatakse ainult üks kord. Kopeeri see kohe ja hoia turvalises kohas (nt paroolihaldurris).

---

## 🔧 Tokeni kasutamine VS Code'is

1. Ava VS Code.
2. Installi laiendus **GitHub Copilot** (kui pole veel installitud).
3. Vajuta `Ctrl+Shift+P` (Windows/Linux) või `Cmd+Shift+P` (Mac).
4. Otsi käsk **GitHub Copilot: Sign In**.
5. Järgi ekraanil kuvatavaid juhiseid – VS Code suunab sind automaatselt GitHubi lehele autentimiseks.

> **Märkus:** VS Code autentib Copiloti kasutaja OAuth voo kaudu, seega eraldi tokenit käsitsi sisestada tavaliselt ei ole vaja. PAT on vajalik peamiselt API otseintegratsioonide jaoks.

---

## ❓ Korduma kippuvad küsimused

**K: Kust ma tean, kas mul on Copilot tellimusega aktiveeritud?**  
V: Kontrolli aadressilt [github.com/settings/copilot](https://github.com/settings/copilot), kas Copilot on sinu kontol lubatud.

**K: Token aegus – mida teha?**  
V: Loo uus token samade sammude järgi ja uuenda see kõikides rakendustes, kus seda kasutasid.

**K: Tokenit lekib – mida teha?**  
V: Mine kohe GitHubi seadetesse (**Settings → Developer settings → Personal access tokens**) ja kustuta lekkinud token. Seejärel genereeri uus.

---

## 📎 Kasulikud lingid

- [GitHub Copilot dokumentatsioon](https://docs.github.com/en/copilot)
- [Isikliku juurdepääsutunnuse haldamine](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)
- [GitHub Copilot seaded](https://github.com/settings/copilot)
