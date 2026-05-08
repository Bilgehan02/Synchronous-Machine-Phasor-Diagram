# ⚡ Synchronous Machine Phasor Diagram

An interactive phasor diagram tool for analyzing **salient pole** and **round rotor** synchronous machines — built with pure HTML, CSS, and JavaScript. No frameworks, no dependencies.

## 🔴 Live Demo

> Open `phasor_diagram.html` directly in your browser — no server required.

---

## 📌 Features

- **Two machine types** supported:
  - Round rotor (cylindrical) — uniform air gap, single reactance (Xs)
  - Salient pole — non-uniform air gap, two-axis reactance (Xd, Xq)
- **Real-time phasor rendering** as you adjust parameters
- **Leading / lagging power factor** conditions
- **d-q axis decomposition** — visualize Id, Iq, Vd, Vq components
- **Generator & motor mode** support
- Fully responsive, runs offline

---

## 🧮 Theory

### Round Rotor Machine

The terminal voltage phasor is given by:

```
Ef = Vt + Ra·Ia + jXs·Ia
```

Where `Xs` is the synchronous reactance (same in both axes).

### Salient Pole Machine

Uses the two-reaction theory (Blondel):

```
Ef = Vt + Ra·Ia + jXd·Id + jXq·Iq
```

Where:
- `Xd` — direct-axis synchronous reactance
- `Xq` — quadrature-axis synchronous reactance (Xq < Xd)
- `Id`, `Iq` — d- and q-axis current components

The power angle `δ` is determined iteratively from the phasor geometry.

---

## 🚀 Usage

```bash
git clone https://github.com/USERNAME/synchronous-machine-phasor-diagram.git
cd synchronous-machine-phasor-diagram
# Open in browser
open phasor_diagram.html
```

Or simply download `phasor_diagram.html` and open it locally.

---

## 📂 File Structure

```
├── phasor_diagram.html   # Entire application — single file
└── README.md
```

---

## 🎯 Who Is This For?

- Electrical engineering students studying electric machines
- Instructors looking for visual teaching aids
- Engineers who want a quick, offline reference tool

---

## 🛠 Built With

- HTML5 Canvas / SVG
- No external libraries or dependencies

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

*If this tool helped you understand synchronous machines better, consider giving it a ⭐*
