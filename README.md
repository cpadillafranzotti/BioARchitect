# BioARchitect

**Explore the architecture of life in augmented reality.**

[![Demo visits](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fbioarchitect.goatcounter.com%2Fcounter%2F%252FBioARchitect.json&query=count&label=Demo%20visits&color=blueviolet)](https://cpadillafranzotti.github.io/BioARchitect/)
[![AR sessions](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fbioarchitect.goatcounter.com%2Fcounter%2Far-launch.json&query=count&label=AR%20sessions&color=orange)](https://cpadillafranzotti.github.io/BioARchitect/)
[![Android](https://img.shields.io/badge/Android-AR-3DDC84?logo=android&logoColor=white)](https://cpadillafranzotti.github.io/BioARchitect/)
[![iOS](https://img.shields.io/badge/iOS-AR-000000?logo=apple&logoColor=white)](https://cpadillafranzotti.github.io/BioARchitect/)
![Version](https://img.shields.io/badge/version-2.3-0053d6)
[![License: Academic Evaluation](https://img.shields.io/badge/license-Academic%20Evaluation-3d8fd6)](LICENCE)

BioARchitect is a web-based viewer that brings proteins, nucleic acids and small molecules into your space. Search a structure, choose how to display it, and place it on your table with your phone's camera. No app to install.

<p align="left">
  <a href="https://cpadillafranzotti.github.io/BioARchitect/" target="_blank">
    <img src="https://img.shields.io/badge/VIEW_LIVE_DEMO-0053d6?style=for-the-badge" alt="Try Live Demo">
  </a>
</p>

<p align="center">
  <img src="bioarchitect-preview.gif" alt="BioARchitect AR Demo" width="380px">
</p>

## Quick start

1. Open the demo on your phone.
2. Pick a database and type an ID or a name, or tap one of the examples.
3. Tap **View in AR**, point your phone at the floor or a table, and move it slowly until the molecule appears.

## Try these

Each link opens a structure ready to explore:

| Structure | What to look for |
|---|---|
| [Hemoglobin](https://cpadillafranzotti.github.io/BioARchitect/?pdb=4HHB) | Four chains carrying four heme groups (tap one to see its name) |
| [p53](https://cpadillafranzotti.github.io/BioARchitect/?alphafold=P04637&color=plddt) | AlphaFold confidence: ordered domains in blue, disordered regions in orange |
| [Top7](https://cpadillafranzotti.github.io/BioARchitect/?pdb=1QYS&style=surface) | The first designed protein with a fold not seen in nature |
| [Hemoglobin surface by charge](https://cpadillafranzotti.github.io/BioARchitect/?pdb=4HHB&style=surface&color=charge) | Positive and negative patches on the protein surface |
| [DNA](https://cpadillafranzotti.github.io/BioARchitect/?pdb=1BNA&color=flag&flag=AR) | The double helix in the colors of the Argentine flag 🇦🇷 |
| [Caffeine](https://cpadillafranzotti.github.io/BioARchitect/?pubchem=caffeine) | A small molecule, atom by atom |

## Features

- **Search four sources:** PDB (experimental structures, including large mmCIF-only entries), de novo designed proteins (search by keyword, e.g. *barrel*), AlphaFold DB (predicted models by UniProt accession) and PubChem (small molecules by name or CID).
- **Display styles:** cartoon, tube, space-filling spheres and molecular surface for proteins and nucleic acids; ball-and-stick for small molecules.
- **Color schemes:** scientific and fun, in two menus side by side. See [About the color palettes](#about-the-color-palettes).
- **Tap to identify:** tap any part of the structure to see the residue, nucleotide, ligand or atom (e.g. *Histidine 87 · chain A*). The selected residue lights up in magenta, also in AR.
- **Sequence:** see the sequence of every chain, colored like the structure, with gaps where residues are missing from the model (often flexible or disordered regions). Tap a residue in the sequence to find it in 3D, or tap the structure to find it in the sequence.
- **Help:** a short explanation of the current representation and color scheme, for students and curious minds.
- **Ligands:** show or hide bound ligands, such as the heme groups of hemoglobin, and see their names, formulas and copies in **Info**.
- **Biological assembly or asymmetric unit:** PDB entries open as their biological assembly (the form the molecule is thought to take in the cell); switch to the asymmetric unit deposited in the PDB in one tap.
- **What you are looking at:** each structure shows its ID, whether it is experimental, contains a de novo design, is predicted or is a small molecule, and its real size next to its size in AR (*≈ 6 nm · ×100 million in AR*). Tap **Info** for title, organism, method, resolution and links.
- **Share:** send a link that opens the same structure, style and color. Handy for classes, talks and chats.
- **Save what you see:**
  - **PNG:** image with a transparent background, for slides and posters. In AR, use your phone's screenshot.
  - **SVG:** editable vector drawing of the same view (Illustrator, Inkscape, PowerPoint).
  - **PDF:** one-page sheet with the view, its color legend, the entry details, ligands and links.
  - **GLB:** 3D model with its colors, ready to import into Blender or insert into PowerPoint.
  - **STL:** for 3D printing, at 1 Å = 1 mm (hemoglobin ≈ 6.5 cm). Surface and Spheres print best.
- **Augmented reality** on compatible Android phones and iPhones, straight from the browser, with on-screen tips to place, move and resize the model. You can identify residues, read the sequence and change colors without leaving AR. On a computer, you can explore the structures in 3D.
- **Change molecule without leaving AR** (Android): open **Display** to search or tap an example; the new structure appears in the same spot.
- **Clean AR view:** one tap hides every label and button, leaving only the molecule in your space and a small BioARchitect watermark. Ideal for photos and screen recordings.
- **English and Spanish:** switch with **EN | ES** at the top. BioARchitect opens in English; it remembers your choice.
- **Light and dark mode:** switch with the 🌙 / ☀️ button at the top left. BioARchitect follows your phone's setting until you choose, and remembers your choice.
- **Embed it in your website:** see [Embed BioARchitect](#embed-bioarchitect-in-your-website).

## About the color palettes

| Palette | What it shows | Source |
|---|---|---|
| Confidence (pLDDT) | How confident AlphaFold is about each residue (0–100) | AlphaFold DB model file |
| Chain | Each polymer chain in a different color | Structure file |
| Secondary structure | Helices, strands and coils | Structure file (HELIX/SHEET records), or assigned from Cα geometry when absent |
| Rainbow (N→C) | Position along each chain, from N- to C-terminus | Structure file |
| Hydrophobicity | Hydrophilic to hydrophobic residues | Kyte & Doolittle hydropathy scale (*J Mol Biol* 1982, 157:105–132) |
| Charge | Side-chain charge at neutral pH: Asp/Glu negative, Lys/Arg positive, His shown apart, polar and nonpolar | Standard residue classification |
| Flexibility (B-factor) | Rigid to mobile regions | B-factors deposited with each experimental structure, scaled within that structure (5th–95th percentile) |
| Chain · colorblind-safe | Each chain in a color that stays distinguishable with color vision deficiencies | Okabe & Ito palette (2008) |

Besides these scientific schemes, BioARchitect has a set of **fun color schemes** for outreach and play. They are for enjoying the structures, not for interpreting them. Some come with a gentle animated scene behind the molecule; it can be turned off with ✨ Effects, and it is never included in saved images or 3D files.

**Note on flexibility:** B-factors also depend on resolution, crystal packing and refinement, so colors compare regions *within* one structure, not between structures. They are only available for experimental structures; for AlphaFold models, use pLDDT.

## Methods and limitations

BioARchitect is designed for exploring, teaching and communicating structures in augmented reality. It is not meant for detailed structural analysis, which needs dedicated molecular modeling software.

BioARchitect reads the structure files and builds the 3D models itself, in the browser:

- **Biological assembly:** built from the deposited coordinates with the symmetry operations described in the mmCIF file (assembly 1). If the file describes none, or the assembly is too large for a phone, the asymmetric unit is shown and this is stated in **Info**.
- **Secondary structure:** taken from the structure file when available (HELIX/SHEET records or mmCIF annotations). AlphaFold files do not include it, so BioARchitect estimates it from Cα distances, an approximation of DSSP. **Info** and the legend say which one is shown.
- **Molecular surface:** a Gaussian density surface, an approximation of the solvent-excluded surface.
- **Models and alternate positions:** for files with several models (e.g. NMR ensembles), the first model is shown; for atoms with alternate locations, conformation A.
- **Sequence:** shows the residues present in the model, numbered as in the file; gaps mark residues that were not modeled.
- **Ligands:** bonds are inferred from interatomic distances, without bond orders.
- **Tap to identify:** in Cartoon and Tube, the residue whose Cα is closest to the tapped point.
- **Scale:** in AR, 1 Å = 1 cm (×100 million) for macromolecules and 1 Å = 2 cm for small molecules; the value updates when you resize the model.
- **De novo designs:** detected from the entry's keywords and title; an entry may contain both designed and natural chains.

3D display and AR: [`<model-viewer>`](https://modelviewer.dev/) (Google, Apache 2.0) and [three.js](https://threejs.org/) (MIT).

## Requirements

- **Android:** Chrome on a phone with [Google Play Services for AR](https://developers.google.com/ar/devices).
- **iPhone / iPad:** Safari.
- **Social media apps** (Instagram, Facebook, TikTok…): their built-in browsers can't open AR. BioARchitect will offer to open the page in your browser.
- **Computer:** any modern browser, in 3D only.

## 🌿 BioARchitect on the Move

*Take 10 outside.* Between experiments or between lines of code, here's a good excuse to go for a walk and get some fresh air. Where would you place a molecule? Drop a protein into your favourite spot and share your snapshot with us.

### Share Your Snapshot

📸 **How to capture it:** while in AR, tap the 👁 button to hide all the labels, then take a screenshot with your phone.

Want to submit a photo or get in touch? Click below to send your snapshot and caption directly:

<p align="left">
  <a href="mailto:carlastembio@gmail.com?subject=BioARchitect%20On%20The%20Move%20-%20Photo%20Submission&body=Hi%20Carla,%0A%0AHere%20is%20my%20snapshot%20for%20BioARchitect!%0A-%20Location:%20%0A-%20Caption:%20%0A%0A(Please%20attach%20your%20photo%20to%20this%20email)" target="_blank">
    <img src="https://img.shields.io/badge/SEND_PHOTO_OR_MESSAGE-0053d6?style=for-the-badge&logo=minutemailer&logoColor=white" alt="Send Photo or Message">
  </a>
</p>

## 💙 Support BioARchitect

BioARchitect is an independent project. If you find it useful or enjoy it, you can support its development:

<p align="left">
  <a href="https://cafecito.app/bioarchitect" target="_blank">
    <img src="https://img.shields.io/badge/Cafecito-Buy_me_a_cafecito-74acdf?style=for-the-badge&logo=buymeacoffee&logoColor=white" alt="Support on Cafecito">
  </a>
  <a href="https://buymeacoffee.com/bioarchitect" target="_blank">
    <img src="https://img.shields.io/badge/Buy_me_a_coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy me a coffee">
  </a>
</p>

Sharing it, citing it or sending feedback also helps a lot!

## Using BioARchitect in a class or talk?

Go ahead! Please mention **BioARchitect by Carla Padilla Franzotti** and link to the [demo](https://cpadillafranzotti.github.io/BioARchitect/). I'd love to hear how you used it.

## Embed BioARchitect in your website

You can show BioARchitect inside your own website, course page or blog with an `iframe`. Add `embed=1` to show only the viewer, with a small *Open in BioARchitect ↗* link:

```html
<iframe src="https://cpadillafranzotti.github.io/BioARchitect/?pdb=4HHB&style=surface&color=charge&embed=1"
        width="100%" height="600" style="border:0"
        allow="xr-spatial-tracking; fullscreen; web-share; clipboard-write"
        title="Hemoglobin in BioARchitect"></iframe>
```

- **Choose what it shows** with the same options as a shared link: `pdb=`, `alphafold=` or `pubchem=`, plus `style=` and `color=`. The easiest way: open the structure in BioARchitect, set it up, tap **Share** and copy the link.
- **Language:** add `&lang=es` for Spanish or `&lang=en` for English.
- **Light or dark:** add `&theme=dark` or `&theme=light` to match your site. Without it, the viewer follows the visitor's system setting.
- **Keep `allow="xr-spatial-tracking"`** so AR can start on Android. On iPhone, AR opens from the *Open in BioARchitect ↗* link.
- Embedding the live demo in educational and non-commercial websites is welcome, with credit to **BioARchitect by Carla Padilla Franzotti**.

## Data Sources

- **[RCSB PDB](https://www.rcsb.org/)**: experimental macromolecular structures, de novo design search and ligand names (Public Domain / CC0).
- **[AlphaFold DB](https://alphafold.ebi.ac.uk/)**: predicted protein structure models by UniProt accession ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
- **[PubChem](https://pubchem.ncbi.nlm.nih.gov/)**: small molecules by name or CID (Public Domain).

## 📄 License

This project is distributed under the terms of the **Academic Evaluation License – All Rights Reserved**. See the [LICENCE](LICENCE) file for more details.

## Author

Created by [Carla Padilla Franzotti](https://cpadillafranzotti.github.io/) · © 2025–2026
