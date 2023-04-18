# Hobbyprosjektkveld Navet x Bekk

## Introduksjon 👋

I denne guiden vil vi gå gjennom stegene for å sette opp et nytt webprosjekt fra scratch og gjøre dette tilgjengelig for hele verden på nett!

Vi vil ta i bruk moderne teknologier som blir brukt på virkelige prosjekter for å løse kunders problemer.

Er det noe som helst som er uklart eller du trenger hjelp med, husk at du alltid kan vinke til en Bekker! 🖐

### Hva denne guiden er 🟢

Denne guiden kan man bruke som en kickstart til et nytt hobbyprosjekt. Guiden er ment for å vise hvor enkelt det kan være å få en produksjonsklar nettside ut på nett, ved å ta i bruk moderne teknologier.

### Hva denne guiden _ikke_ er 🔴

Dette er _ikke_ ett sted hvor man lærer grunnleggende webutvikling. Byggesteinene til weben er HTML, CSS og JavaScript. Men i webutviklingssfæren i dag finnes det en jungel av verktøy som hjelper oss å lage løsninger raskere og bedre enn hva vi kunne gjort med ren HTML, CSS og JavaScript. I denne guiden vil vi ta i bruk noen ekstra verktøy for å hjelpe oss på veien, men det anbefales å bli kjent med det grunnleggende for å jobbe med webutvikling.

Et eksempel på et slikt verktøy er Next.js, som vi vil bruke i dag. [Next.js](https://nextjs.org/) er et _rammeverk_ for [React](https://react.dev/), som igjen er et _bibliotek_ for webutvikling.

### Hva vil man sitte igjen med? 🎁

Når du har følgt denne guiden vil du sitte igjen med en nettside bygget med Next.js. Nettsiden din vil bli tilgjengelig via Vercel, en skyplattform som bl.a. tilbyr hosting av nettsider. Dette kan være starten på ditt neste store prosjekt, eller bare en gøy liten greie du kan vise til familie, venner og potensielle arbeidsgivere.

### Prerequisites 🔨

For å kunne gjennomføre disse stegene er man nødt til å ha noen ting klart:

1. Installert [Node](https://nodejs.org/en)
2. En bruker på [GitHub](https://github.com/)
3. Installert [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
4. Installert en IDE (f.eks. [VSCode](https://code.visualstudio.com/))

# Guide

> ✋ I stegene under vil du måtte bruke terminalen. Den er litt forskjellig basert på OS. Er du i tvil på hvordan du åpner og bruker terminalen, bare spør en bekker.

## Del 1: Opprett prosjektet lokalt 📦

<details>
    <summary> 
    💡Navigasjon i terminalen
    </summary>

  <ul> 
    <li> gå til mappe: <code>cd sti/til/mappe</code></li>
    <li> vis filer <code>ls</code></li>
  <ul>  
</details>
<br/>

Åpne terminalen din og naviger til et sted på maskinen din hvor du ønsker å opprette prosjektet ditt. Deretter kjør kommandoen under for opprette et nytt Next.Js-prosjekt:

```bash
npx create-next-app@latest
```

Først vil du få spørsmål om hva prosjektet skal hete, her kan du velge et kreativt navn selv og trykke `enter`.

Deretter vil få opp en rekke prompts hvor du blir bedt om å velge hvordan prosjektet ditt skal være konfigurert (se eksempel under). Du kan velge default-verdiene (`enter`) for alle valgene.

```bash
 What is your project named? ... mitt-fete-prosjekt
√ Would you like to use TypeScript with this project? ... No / Yes
√ Would you like to use ESLint with this project? ... No / Yes
√ Would you like to use `src/` directory with this project? ... No / Yes
√ Would you like to use experimental `app/` directory with this project? ... No / Yes
√ What import alias would you like configured? ... @/*

```

🎉 Dersom alt har gått fint i stegene over, skal du nå sitte igjen med et nytt Next.Js prosjekt!

🙋‍♂️Gikk ikke ting helt etter planen? Husk at du kan alltid spørre en Bekker!

## Del 2: Utforsk prosjektet og gjør noen endringer 💅

Nå som vi har fått opprettet prosjektet vårt, er vi klar til å gjøre det til vårt eget.

### Filer i prosjektet

<table>
  <tr>
    <td valign="top"><img src="https://user-images.githubusercontent.com/21195934/232860559-8dc34b8c-79f9-47e8-bb3d-8b2d3bd09555.png" height="100%" width="100%"/></td>
    <td valign="top"><p>Når du åpner prosjektet ditt i din favoritt IDE, blir du møtt med en filstrukutur lignende bildet til venstre. Det er kanskje mange filer som du aldri har sett før, men her er en veldig kort forklaring: </p>
    <ul> 
      <li>Filer som slutter på ".tsx" er filer du skriver React kode med TypeScript i. Det er typisk her man vil gjøre endringer som reflekteres i nettleseren.</li> 
      <li>Filer som slutter på ".ts" skriver man TypeScript (typet JavaScript).</li>
      <li>Filer som slutter på ".css" er der man skriver CSS. Altså styling av nettsiden.</li>
      <li>Resterende filer er stort sett konfigurasjonsfiler for verktøy som blir brukt i prosjektet.</li>
    </ul>
    </td>
  </tr>
</table>

### Kjør opp prosjektet

<details> 
  <summary>💡Tips for VSCode</summary>

Du kan åpne terminalen i VSCode. Enten fra oppgavelinjen på toppen, eller ved å bruke Command Pallett og søke etter funksjonen. Command Pallett kan du åpne ved å trykke <code>ctrl+shift+p</code> eller <code>cmd+shift+p</code>, og er nyttig for å søke etter funksjoner du trenger i VSCode.

</details>

Åpne terminalen, naviger til prosjektet ditt og kjør denne kommandoen:  
`npm run dev`

Dette vil starte en webserver på maskinen din og tilgjengeliggjøre nettsiden din lokalt. Åpne nettleseren din og gå til `http://localhost:3000/` for å ta en titt på nettsiden. 

### Gjør din første endring

Du kan velge selv hva du vil gjøre utav dette prosjektet, men det er nok lurt å starte i `src/pages/index.tsx`. 

`index.tsx` filen består av en JavaScript-funksjon som returnerer et `JSX.Element`. En slik funksjon er kjent som en React komponent. Inne i slike funksjoner kan man skrive en blanding av HTML og JavaScript for å bygge komponenter til en nettside. 

❓ Er alt dette helt nytt for deg? Da anbefales det å ta en titt på [React sin dokumentasjon](https://react.dev/learn). Ellers kan du erstatte innholdet i `index.tsx` med eksempelkoden under. 

<details> 
 <summary> Eksempelkode <code>index.tsx</code></summary>

 ```javascript
import Head from "next/head";
import styles from "@/styles/Home.module.css";

export default function Home() {
  const mittNavn = "Ola Nordmann";
  return (
    <>
      <Head>
        <title>Create Next App</title>
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <main className={styles.main}>
        <h1>Hei, {mittNavn}!👋</h1>
        <p>Her kan man kode med vanlig HTML, kombinert med JavaScript.</p>
      </main>
    </>
  );
}

```
</details>


## Del 3: Publiser prosjektet ditt på GitHub

1. Logg inn på brukeren din på GitHub.com
2. Opprett et nytt repository.
3. Kopier terminalkommandoene som står under "push existing repository" Det burde se ca. slik ut:

```bash
git remote add origin git@github.com:bekk/ifi-hobbyprosjektkveld-2023.git
git branch -M main
git push -u origin main
```

## Del 4: Vis prosjektet ditt til verden 🌍

1. Gå til [Vercel](https://vercel.com/) og opprett en bruker, gjerne ved å bruke GitHub-brukeren din.

2. Opprett et nytt Vercel-prosjekt. Importer GitHub-repoet som ble publisert på GitHub i del 3.
