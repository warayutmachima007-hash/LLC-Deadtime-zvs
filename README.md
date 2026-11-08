# Dead time decides ZVS

Interactive animation of a half-bridge LLC converter showing how dead time decides zero-voltage switching (ZVS) of the low-side MOSFET.

**Live page:** https://warayutmachima007-hash.github.io/llc-deadtime-zvs/

## What it shows
- Four dead times side by side: too short, just right, longer than needed, far too long
- Gate, Vds, Id and resonant current iLr of the low-side switch, plus a one-cycle overview
- Body-diode conduction, output-capacitance charge and discharge, and switching loss
- Adjustable Co(tr) and body-diode Vf; click or drag in any graph to move the cursor
- How to choose the dead time: t_dead ≥ 2·Co(tr)·Vin / I_Lm,pk

## Model
Time-domain simulation of a 400 V → 48 V / 1 kW half-bridge LLC (Lr 30 µH, Cr 47 nF, Lm 150 µH, n 4.2, fs 130 kHz), run in the browser. Output capacitance is a fixed time-related value Co(tr); hard-switching current spikes and ringing are not modelled.

## Reference
S. S. Queiroz and L. F. Costa, "Investigation of the Influence of the Dead-Time on the Performance of an LLC Resonant Converter for High-Power Application," Proc. IEEE PEDG, 2024. doi:10.1109/PEDG61800.2024.10667434

## Deploy
Single self-contained `index.html` (fonts from Google Fonts). Push to a GitHub repo named `llc-deadtime-zvs`, then Settings → Pages → Deploy from branch → `main` / root.
