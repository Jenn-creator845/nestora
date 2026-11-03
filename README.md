# Nestora — GitHub Pages website

A responsive static site for browsing monthly rentals, furnished stays and homes for sale. No build step is required. The included properties, photographs and prices are illustrative examples, not real listings.

## Preview locally

Open `index.html` in a browser, or serve the folder with `python -m http.server 8000` and open http://localhost:8000. Keep the files and `assets` folder together.

## Publish on GitHub Pages

1. Create a new GitHub repository, for example `nestora`.
2. Extract this ZIP, open the `nestora` folder, and upload its CONTENTS to the repository root. `index.html` must be at the root, alongside `style.css`, `app.js`, `listings.js` and `assets/`.
3. On GitHub go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. Wait for the deployment to finish. GitHub Pages shows the website address on the same Settings → Pages screen. A project site usually looks like `https://USERNAME.github.io/nestora/`.

## Update properties and contact

Edit `listings.js`: each object represents a property. Set `type` to `rent`, `furnished`, or `sale`; `period` to `month`, `night`, or `sale`; and `price` to a number in KES. Put photos in `assets` and set each `image` to its relative path, for example `assets/my-home.jpg`. The sample photos are cropped from the illustrative mockup in the supplied PDF; replace them with approved photographs. Verify property descriptions, prices, and availability before publishing.

To activate property enquiries, change `window.NESTORA_WHATSAPP` from an empty string to Jennifer's number with country code and digits only, e.g. `2547XXXXXXXX`. Each listing's WhatsApp button will open a prefilled message. Test it before launch. Until then, no contact button is presented as active.

Update files on GitHub and commit the changes; Pages will redeploy. GitHub Pages is static: it does not provide a protected admin portal, database, photo uploads, secure credentials, or server-side enquiry processing. Updating listings currently requires editing repository files. A shared, password-protected admin and live listings require an external backend/CMS and suitable access controls. Never put passwords or secrets in this public repository.

The logo is taken from the logo concept in the supplied PDF. The sample images, locations and prices are for demonstration.
