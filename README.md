# JungleStudios - Guida

Questa guida ti aiuterà a personalizzare e configurare il template del sito JungleStudios. Il template è realizzato utilizzando TailwindCSS e Line Awesome (per le icone).

## Indice
1. [Installazione](#installazione)
2. [Personalizzazione](#personalizzazione)
    - [Titolo del Sito e Logo](#titolo-del-sito-e-logo)
    - [Link di Navigazione](#link-di-navigazione)
    - [Sezione Chi Siamo](#sezione-chi-siamo)
    - [Sezione Servizi](#sezione-servizi)
    - [Sezione Portfolio](#sezione-portfolio)
    - [Sezione Contatti](#sezione-contatti)
    - [Footer](#footer)
3. [Animazioni](#animazioni)
4. [Animazioni di Scorrimento](#animazioni-di-scorrimento)
5. [Ritocchi Finali](#ritocchi-finali)

## Installazione

Per utilizzare questo template, scarica o clona il repository e apri il file `index.html` nel tuo browser.

```bash
git clone https://github.com/your-username/JungleStudios.git
cd JungleStudios
```

Apri `index.html` nel tuo browser preferito per visualizzare il sito.

## Personalizzazione

### Titolo del Sito e Logo

Il titolo del sito è impostato nella sezione header del file `index.html`. Puoi cambiare il testo o sostituirlo con un'immagine logo.

#### Cambia il Titolo del Sito

```html
<h1 class="text-3xl font-bold">JungleStudios</h1>
```
Sostituisci `JungleStudios` con il nome desiderato per il sito.

#### Usa un Logo Immagine

```html
<h1><img src="path/to/logo.png" alt="JungleStudios Logo" class="h-10"></h1>
```
Sostituisci `path/to/logo.png` con il percorso del tuo logo.

### Link di Navigazione

I link di navigazione si trovano nella sezione header. Puoi aggiornare il testo e gli URL dei link per adattarli alla struttura del tuo sito.

```html
<nav>
  <ul class="flex space-x-8">
    <li><a href="#about" class="hover:text-gray-300">Chi Siamo</a></li>
    <li><a href="#services" class="hover:text-gray-300">Servizi</a></li>
    <li><a href="#portfolio" class="hover:text-gray-300">Portfolio</a></li>
    <li><a href="#contact" class="hover:text-gray-300">Contatti</a></li>
  </ul>
</nav>
```
### Sezione Chi Siamo

Il contenuto della sezione Chi Siamo può essere personalizzato all'interno della `section` con l'ID `about`.

```html
<section id="about" class="h-screen py-12 px-6 fade-in scroll-anim flex items-center">
  <div class="text-center w-full">
    <h2 class="text-4xl font-bold mb-8">Chi Siamo</h2>
    <p class="text-xl max-w-4xl mx-auto">Siamo JungleStudios, un piccolo ma professionale team di sviluppo web dedicato alla creazione di siti web e applicazioni sorprendenti. Il nostro obiettivo è fornire soluzioni di alta qualità e innovative ai nostri clienti.</p>
  </div>
</section>
```
Modifica l'intestazione e il testo del paragrafo per riflettere le informazioni del tuo team.

### Sezione Servizi

La sezione Servizi elenca i servizi che offri. Ogni servizio ha un'icona, un titolo e una descrizione.

```html
<section id="services" class="h-screen py-12 px-6 bg-gray-800 slide-in scroll-anim flex items-center">
  <div class="text-center w-full">
    <h2 class="text-4xl font-bold mb-8">I Nostri Servizi</h2>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-16">
      <div class="bg-gray-700 p-8 rounded-lg">
        <i class="las la-code la-4x text-green-500"></i>
        <h3 class="text-3xl font-bold mt-6">Sviluppo Web</h3>
        <p class="mt-4 text-lg">Servizi di sviluppo web di alta qualità utilizzando le ultime tecnologie.</p>
      </div>
      <div class="bg-gray-700 p-8 rounded-lg">
        <i class="las la-paint-brush la-4x text-green-500"></i>
        <h3 class="text-3xl font-bold mt-6">Design</h3>
        <p class="mt-4 text-lg">Design web creativo e moderno per far risaltare il tuo sito.</p>
      </div>
      <div class="bg-gray-700 p-8 rounded-lg">
        <i class="las la-mobile-alt la-4x text-green-500"></i>
        <h3 class="text-3xl font-bold mt-6">Responsivo</h3>
        <p class="mt-4 text-lg">Garantiamo che il tuo sito sia perfetto su tutti i dispositivi, dai telefoni ai desktop.</p>
      </div>
    </div>
  </div>
</section>
```
Cambia le icone, i titoli e le descrizioni per adattarli ai tuoi servizi. Le icone possono essere trovate su [Line Awesome](https://icons8.com/line-awesome).

### Sezione Portfolio

La sezione Portfolio mostra i tuoi progetti. Ogni progetto ha un'immagine e un titolo.

```html
<section id="portfolio" class="h-screen py-12 px-6 fade-in scroll-anim flex items-center">
  <div class="text-center w-full">
    <h2 class="text-4xl font-bold mb-8">Il Nostro Portfolio</h2>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-16">
      <div class="bg-gray-700 p-8 rounded-lg">
        <img src="https://source.unsplash.com/random/800x600?web" alt="Progetto 1" class="w-full h-64 object-cover rounded-lg">
        <h3 class="text-3xl font-bold mt-6">Progetto Uno</h3>
      </div>
      <div class="bg-gray-700 p-8 rounded-lg">
        <img src="https://source.unsplash.com/random/800x600?tech" alt="Progetto 2" class="w-full h-64 object-cover rounded-lg">
        <h3 class="text-3xl font-bold mt-6">Progetto Due</h3>
      </div>
      <div class="bg-gray-700 p-8 rounded-lg">
        <img src="https://source.unsplash.com/random/800x600?design" alt="Progetto 3" class="w-full h-64 object-cover rounded-lg">
        <h3 class="text-3xl font-bold mt-6">Progetto Tre</h3>
      </div>
    </div>
  </div>
</section>
```
Sostituisci gli URL delle immagini e i titoli dei progetti con i tuoi.

### Sezione Contatti

La sezione Contatti contiene un form per i visitatori per contattarti. Il form può essere collegato a un servizio backend o di email.

```html
<section id="contact" class="h-screen py-12 px-6 bg-gray-800 slide-in scroll-anim flex items-center">
  <div class="text-center w-full">
    <h2 class="text-4xl font-bold mb-8">Contattaci</h2>
    <form action="#" method="POST" class="grid grid-cols-1 gap-4 max-w-2xl mx-auto">
      <input type="text" name="name" placeholder="Il Tuo Nome" class="p-4 rounded-lg bg-gray-900 border border-gray-700 focus:outline-none focus:border-green-500">
      <input type="email" name="email" placeholder="La Tua Email" class="p-4 rounded-lg bg-gray-900 border border-gray-700 focus:outline-none focus:border-green-500">
      <textarea name="message" placeholder="Il Tuo Messaggio" class="p-4 rounded-lg bg-gray-900 border border-gray-700 focus:outline-none focus:border-green-500"></textarea>
      <button type="submit" class="bg-green-600 p-4 rounded-lg hover:bg-green-500">Invia Messaggio</button>
    </form>
  </div>
</section>
```
### Footer

Il footer contiene informazioni sul copyright e può essere personalizzato per includere link ai tuoi social media o altre informazioni.

```html
<footer class="bg-gray-800 p-4 text-center text-gray-400">
  &copy; 2024 JungleStudios. Tutti i diritti riservati.
</footer>
```
## Animazioni

Le animazioni personalizzate sono definite nella sezione `style` del file `index.html`. Le animazioni includono `fadeIn` e `slideIn`.

```css
/* Animazioni */
.fade-in {
  animation: fadeIn 2s ease-in forwards;
}
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
.slide-in {
  animation: slideIn 1s ease-out forwards;
}
@keyframes slideIn {
  from { transform: translateY(20px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}
```
## Animazioni di Scorrimento

Il template include animazioni di scorrimento che rivelano gli elementi quando entrano in vista. Questo è gestito dal codice JavaScript in fondo al file `index.html`.

```javascript
// Animazione di Scorrimento
const scrollElements = document.querySelectorAll('.scroll-anim');

const elementInView = (el, dividend = 1) => {
  const elementTop = el.getBoundingClientRect().top;
  return (
    elementTop <= (window.innerHeight || document.documentElement.clientHeight) / dividend
  );
};

const displayScrollElement = (element) => {
  element.classList.add('show');
};

const handleScrollAnimation = () => {
  scrollElements.forEach((el) => {
    if (elementInView(el, 1.25)) {
      displayScrollElement(el);
    }
  });
};

window.addEventListener('scroll', () => {
  handleScrollAnimation();
});

// Caricamento iniziale
handleScrollAnimation();
```
## Ritocchi Finali

Dopo aver personalizzato il template secondo le tue esigenze, assicurati di testarlo su diversi dispositivi per garantire che sia completamente funzionale. Puoi distribuire il sito su un servizio di hosting web come GitHub Pages, Netlify, Vercel oppure ospitare il sito da Locale tramite un server web locale come serve o live-server.

### Distribuire su GitHub Pages

1. Crea una nuova repository su GitHub.
2. Carica tutti i file del tuo progetto nella repository.
3. Vai nelle impostazioni del repository, scorri fino alla sezione GitHub Pages.
4. Nella sezione "Source", seleziona il branch principale (main o master) e la cartella root.
5. Salva le impostazioni. GitHub Pages pubblicherà automaticamente il sito web. 

### Distribuire su Netlify

1. Registra un account su [Netlify](https://www.netlify.com/).
2. Crea un nuovo sito dal tuo dashboard.
3. Collega il repository GitHub, GitLab o Bitbucket contenente i file del progetto.
4. Netlify procederà alla build e alla pubblicazione automatica del sito.

### Distribuire su Vercel

1. Registra un account su [Vercel](https://vercel.com/).
2. Crea un nuovo progetto e collega il tuo repository GitHub, GitLab o Bitbucket.
3. Vercel procederà alla build e alla pubblicazione automatica del sito.

### Ospitare il sito da Locale

Se preferisci testare il sito in locale prima di distribuirlo, puoi utilizzare strumenti come `serve` o `live-server`.

#### Usare `serve`

```bash
npx serve .
```

Il comando avvierà un server web locale e renderà il sito accessibile nel browser all'indirizzo http://localhost:5000.

#### Usare `live-server`

```bash
npx live-server
```
Il comando avvierà un server web locale con supporto per il live-reload, il che significa che il sito verrà ricaricato automaticamente ogni volta che apporterai modifiche ai file.

## Conclusione

Seguendo questa guida, potrai personalizzare e distribuire il template JungleStudios, creando un sito web professionale e accattivante. Assicurati di testare il sito su diversi dispositivi e browser per garantire un'esperienza utente uniforme e di alta qualità.

---

---

Seguendo questa guida, puoi adattare il template JungleStudios alle tue esigenze.

---
