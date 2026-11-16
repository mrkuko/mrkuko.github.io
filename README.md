# Osobný web (GitHub Pages)

Statická stránka: `index.html` + `assets/`. Bez build kroku, Tailwind sa načítava z CDN.

## Nasadenie na https://mrkuko.github.io

1. Na GitHube vytvor **verejný** repozitár s názvom presne `mrkuko.github.io` (účet `mrkuko`).
2. Nahraj doň obsah tohto priečinka (nie priečinok samotný):

   ```bash
   cd web
   git init -b main
   git add .
   git commit -m "Osobný web"
   git remote add origin git@github-mrkuko:mrkuko/mrkuko.github.io.git
   git push -u origin main
   ```

3. Repozitár → **Settings → Pages** → Source: *Deploy from a branch*, Branch: `main`, folder `/ (root)`.
4. O minútu je web na `https://mrkuko.github.io`.

`.nojekyll` vypína Jekyll, aby GitHub súbory nijako neupravoval.

## Odkaz na profile

- Do profilu na GitHube (Edit profile → Website) daj `https://mrkuko.github.io`.
- Voliteľne: repozitár `mrkuko/mrkuko` s `README.md` sa zobrazí priamo na profile. Stačí krátky text a odkaz na web.

## Úpravy

- Texty sú priamo v `index.html`, sekcie sú označené komentármi `<!-- ============ ... ============ -->`.
- Obrázky v `assets/` (zmenšené kópie screenshotov z repozitárov projektov).
- E-mail sa skladá až v prehliadači (JavaScript), aby ho boti nenašli v HTML. Telefón na webe zámerne nie je.
