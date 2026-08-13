# Radiology Exchange concept landing page

A static landing page designed to test the positioning: **“Build your own virtual radiology group.”**

## Files

- `index.html` — complete landing page, responsive CSS, and lightweight feedback modal.
- No build system or framework is required.

## Preview locally

Double-click `index.html`, or from this folder run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Before sharing it

### 1. Add a real feedback destination

Open `index.html` and find:

```js
const FEEDBACK_EMAIL = "";
```

Add the email address where you want responses to go. The form will copy the visitor's answers to the clipboard and open a pre-filled email draft.

For a cleaner production experience, replace the prototype form behavior with Formspree, HubSpot, Typeform, Google Forms, or another form endpoint.

### 2. Consider self-hosting the images

The prototype references two Pexels images remotely. For a live test, consider downloading appropriately licensed copies and placing them in an `assets/` folder, then update the `<img src>` paths. This gives you more predictable loading and control.

Current prototype photo pages:
- Radiology workstation: https://www.pexels.com/photo/a-person-using-a-computer-to-diagnose-an-image-6235053/
- Physician video conference: https://www.pexels.com/photo/a-doctor-in-a-video-conference-using-a-laptop-8376339/

### 3. Review concept-stage claims

This page intentionally describes proposed functionality. Before positioning the service as operational, have healthcare counsel validate credentialing, state licensure/telehealth, Medicare/IDTF, billing, corporate-practice, professional-fee, malpractice, and critical-results workflows that apply to the intended model.

## Deploy with GitHub Pages — easiest method

1. Sign in to GitHub and create a new repository, for example `radiology-exchange`.
2. Upload `index.html` (and this README if desired) to the root of the repository.
3. Commit the files to your default branch, usually `main`.
4. Open the repository's **Settings**.
5. In the left sidebar, choose **Pages**.
6. Under **Build and deployment**, select **Deploy from a branch**.
7. Select the `main` branch and the `/ (root)` folder, then save.
8. GitHub will publish the site at a URL similar to:
   `https://YOUR-USERNAME.github.io/radiology-exchange/`

## Optional custom domain

In **Repository → Settings → Pages**, enter your custom domain. Configure the required DNS record with your domain provider and enable HTTPS when GitHub makes the option available.

For a subdomain such as `radiology.example.com`, GitHub's documentation directs you to create a `CNAME` record that points to `YOUR-USERNAME.github.io` (without the repository name).

For an apex/root domain such as `example.com`, follow GitHub's current A/AAAA or ALIAS/ANAME instructions rather than copying stale DNS values from old tutorials.
