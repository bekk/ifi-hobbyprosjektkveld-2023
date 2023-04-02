# Hobbyprosjektkveld Navet x Bekk 

## Introduksjon 👋

I denne guiden vil vi gå gjennom stegene for å sette opp et nytt webprosjekt fra scratch og gjøre dette tilgjengelig for hele verden på nett!

Vi vil ta i bruk moderne teknologier som blir brukt på virkelige prosjekter for å løse kunders problemer.

Er det noe som helst som er uklart eller du trenger hjelp med, husk at du alltid kan vinke til en Bekker! 🖐

### Hva denne guiden er 🟢
Denne guiden kan man bruke som en kickstart til et nytt hobbyprosjekt. Guiden er ment for å vise hvor enkelt det kan være å få en produksjonsklar nettside ut på nett, ved å ta i bruk moderne teknologier.


### Hva denne guiden *ikke* er 🔴
Dette er *ikke* ett sted hvor man lærer grunnleggende webutvikling. Byggesteinene til weben er HTML, CSS og JavaScript. Dette er viktig å poengtere og vi anbefaler sterkt å sette seg inn i disse dersom man ønsker å jobbe med webutvikling. 

Men i webutviklingssfæren i dag finnes det en jungel av verktøy som hjelper oss å lage løsninger raskere og bedre enn hva vi kunne gjort med ren HTML, CSS og JavaScript. 

Et eksempel på et slikt verktøy er Next.js, som vi vil bruke i dag. [Next.js](https://nextjs.org/) er et *rammeverk* for [React](https://react.dev/), som igjen er et *bibliotek* for webutvikling. 


### Hva vil man sitte igjen med? 🎁 
Når du har følgt denne guiden vil du sitte igjen med en nettside bygget med Next.js. Nettsiden din vil bli tilgjengelig via Vercel, en skyplattform som bl.a. tilbyr hosting av nettsider. Dette kan være starten på ditt neste store prosjekt, eller bare en gøy liten greie du kan vise til familie, venner og potensielle arbeidsgivere.    


### Prerequisites 🔨
For å kunne gjennomføre disse stegene er man nødt til å ha tre ting klart.

1. Installert [Node](https://nodejs.org/en)
2. En bruker på [GitHub](https://github.com/)
3. Installert [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) 
4. Installert en IDE (f.eks. [VsCode](https://code.visualstudio.com/))



# Guide
> ℹ I stegene under vil du måtte bruke terminalen en del. Den er litt forskjellig basert på OS. Er du i tvil på hvordan du åpner og bruker terminalen, bare spør en bekker. 


## Del 1: Opprett prosjektet lokalt 📦 
<details>
    <summary> 
    💡Navigasjon i terminalen
    </summary>

    
    -  gå til mappe: cd <mappe man vil navigere til>
    -  vis filer i nåværende mappe: ls     
</details>
<br/>

Åpne terminalen din og naviger til et sted på filsystemet hvor du ønsker å opprette prosjektet ditt og kjøre kommandoen under:  

```bash
npx create-next-app@latest 
```
Først vil du få spørsmål om hva prosjektet skal hete, her kan du velge et kreativt navn selv og trykke `enter`.

Deretter vil få opp en rekke prompts hvor du blir bedt om å velge hvordan prosjektet ditt skal være konfigurert. 

```bash
 What is your project named? ... mitt-fete-prosjekt
√ Would you like to use TypeScript with this project? ... No / Yes
√ Would you like to use ESLint with this project? ... No / Yes
√ Would you like to use `src/` directory with this project? ... No / Yes
√ Would you like to use experimental `app/` directory with this project? ... No / Yes
√ What import alias would you like configured? ... @/*

```

Velg default (`enter`) på alle.


## Del 2: Utforsk prosjektet og gjør noen endringer 💅

## Del 3: Publiser prosjetet ditt på GitHub
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









