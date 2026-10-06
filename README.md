# BioARchitect

**Explore the architecture of life in augmented reality.**

[![Demo visits](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fbioarchitect.goatcounter.com%2Fcounter%2F%252FBioARchitect.json&query=count&label=Demo%20visits&color=blueviolet)](https://cpadillafranzotti.github.io/BioARchitect/)
[![AR sessions](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fbioarchitect.goatcounter.com%2Fcounter%2Far-launch.json&query=count&label=AR%20sessions&color=orange)](https://cpadillafranzotti.github.io/BioARchitect/)
[![Android](https://img.shields.io/badge/Android-AR-3DDC84?logo=android&logoColor=white)](https://cpadillafranzotti.github.io/BioARchitect/)
[![iOS](https://img.shields.io/badge/iOS-AR-000000?logo=apple&logoColor=white)](https://cpadillafranzotti.github.io/BioARchitect/)
![Version](https://img.shields.io/badge/version-2.2-0053d6)
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
| [p53](https://cpadillafranzotti.github.io/BioARchitect/?alphafold=P04637) | AlphaFold confidence: ordered domains in blue, disordered regions in orange |
| [Top7](https://cpadillafranzotti.github.io/BioARchitect/?pdb=1QYS&style=surface) | The first designed protein with a fold not seen in nature |
| [DNA](https://cpadillafranzotti.github.io/BioARchitect/?pdb=1BNA&color=argentina) | The double helix in the AR palette 🇦🇷 |
| [Caffeine](https://cpadillafranzotti.github.io/BioARchitect/?pubchem=caffeine) | A small molecule, atom by atom |

## Features

- **Search four sources:** PDB (experimental structures), de novo designed proteins (search by keyword, e.g. *barrel*), AlphaFold DB (predicted models by UniProt accession) and PubChem (small molecules by name or CID).
- **Display styles:** cartoon, tube, space-filling spheres and molecular surface for proteins and nucleic acids; ball-and-stick for small molecules.
- **Color modes:** AlphaFold confidence (pLDDT), chain, secondary structure, rainbow (N→C) and the AR palette 🇦🇷.
- **Tap to identify:** tap any part of the structure to see the residue, nucleotide, ligand or atom (e.g. *Histidine 87 · chain A*).
- **Ligands:** show or hide bound ligands, such as the heme groups of hemoglobin.
- **What you are looking at:** each structure shows its ID, whether it is natural, de novo, predicted or a small molecule, and its real size next to its size in AR (*≈ 6 nm · ×100 million in AR*). Tap **Info** for title, organism, method, resolution and links.
- **Share:** send a link that opens the same structure, style and color. Handy for classes, talks and chats.
- **Snapshots (3D view):** pause the rotation, pose the molecule and download a PNG with a transparent background. In AR, use your phone's screenshot.
- **Augmented reality** on compatible Android phones and iPhones, straight from the browser, with on-screen tips to place, move and resize the model. On a computer, you can explore the structures in 3D.

## Requirements

- **Android:** Chrome on a phone with [Google Play Services for AR](https://developers.google.com/ar/devices).
- **iPhone / iPad:** Safari.
- **Social media apps** (Instagram, Facebook, TikTok…): their built-in browsers can't open AR. BioARchitect will offer to open the page in your browser.
- **Computer:** any modern browser, in 3D only.

## 🌿 BioARchitect on the Move

*Take 10 outside.* Between experiments or between lines of code, here's a good excuse to go for a walk and get some fresh air. Where would you place a molecule? Drop a protein into your favourite spot and share your snapshot with us.

### Share Your Snapshot

📸 **How to capture it:** while in AR, take a screenshot with your phone.

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

## How to cite

If you use BioARchitect in a class, a talk or a publication, please cite:

> Padilla Franzotti, C. (2026). *BioARchitect: a web-based augmented reality viewer for biomolecular structures.* https://cpadillafranzotti.github.io/BioARchitect/

## Data Sources

- **[RCSB PDB](https://www.rcsb.org/)**: experimental macromolecular structures, de novo design search and ligand names (Public Domain / CC0).
- **[AlphaFold DB](https://alphafold.ebi.ac.uk/)**: predicted protein structure models by UniProt accession ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
- **[PubChem](https://pubchem.ncbi.nlm.nih.gov/)**: small molecules by name or CID (Public Domain).

## 📄 License

This project is distributed under the terms of the **Academic Evaluation License – All Rights Reserved**. See the [LICENCE](LICENCE) file for more details.

## Author

Created by [Carla Padilla Franzotti](https://cpadillafranzotti.github.io/) · © 2025–2026
