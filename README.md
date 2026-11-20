# pet-x-website-stag

Staging repository for the Pet-X Solutions website (petxusa.com, Groom-X), which is moving from WordPress to Next.js.

## Home page design (static reference)

`index.html` is the approved home page design as a static page. It is the reference for the Next.js build.

- `index.html`: the page, with its page-level CSS and scripts inline
- `assets/`: the layout, motion, component and scene files the page loads, plus the Nasalization font in `assets/brand/`
- `img/`: photos, partner logos and the Groom-X app screens from the Figma file (`img/app/`)
- `share.jpg`: the social share image

### Run it locally

The page uses JavaScript modules, so it must be served over HTTP. Opening the file directly does not work.

```bash
npx serve .
# or
python3 -m http.server 8000
```

Then open http://localhost:8000.

### Design system

- Colours: teal-blue `#1E97B7`, deep green `#158B51`, pink `#9C4C97`, button gradient `#444798` to `#9C4C97`, dark background gradient `#23204A` to `#301938`
- Fonts: Nasalization for the logo and the h1 only, Poppins for everything else (Google Fonts)
- Buttons: pill shape

### Notes for the build

- The call-to-action links point to `mailto:info@petxusa.com` as placeholders until the sign-up flow exists.
- Prices are the ones on the current live site ($39.99, $45.99, $49.99 per month). The Figma Subscription screen shows different prices, so confirm them before launch.
