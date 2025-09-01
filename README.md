## GitHub Pages wrapper for my Streamlit portfolio.
The actual app (code, features, and updates) lives in Astrojigs/Portfolio
 and is deployed at https://astrojigs.streamlit.app/
 
 _This repo simply serves a lightweight index.html that embeds the Streamlit app at https://astrojigs.dev
 via an <iframe>._

 > If you’re looking for source code or issues related to the portfolio itself, go to Astrojigs/Portfolio.

### How it works

- Static host: GitHub Pages (root of main branch).

- Custom domain: astrojigs.dev (configured via the CNAME file).

- Single file wrapper: index.html renders a full-viewport <iframe> pointing at the Streamlit app.

- Favicons / PWA bits: stored under /assets and referenced from index.html.

Because this site is an iframe wrapper, the browser URL stays astrojigs.dev while you navigate the Streamlit app inside it. That means inner routes like /contact won’t appear in the address bar (they exist inside the embedded app).
