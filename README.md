# Cerulean Dreamscape Orrery

An interactive orrery for the *[Rothie AA-A h389](https://signals.canonn.tech/?system=Rothie%20AA-A%20h389)* system, depicting the red dwarf, its gas giant *2 g*, and the close binary pair *2 h*/*2 i*, which orbit only about 168,000 km apart. It plots their real orbital motion from recorded Keplerian elements and predicts when *2 g* passes close enough to the pair to make surface contact.

Built by [Canonn Research Group](https://canonn.science/) for the Elite Dangerous exploration community.

## Features

- **Four synchronised views** — a top-down system view, a close-up on the pair's barycentre, an edge-on cross-section (switchable between "from the star" and "across the orbit"), and a full-orbit height/plane diagram.
- **Playback controls** — play/pause, adjustable speed (15 minutes to 10 days per second), step forward/back, and jump to a specific date/time.
- **Live readouts** — surface-to-surface distance from *2 g* to *2 h*, to *2 i*, and to the pair's barycentre, updating as time advances.
- **Encounter table** — every predicted close approach from 2026–2048, with contact start/end times (in-universe date, hover for the real-world UTC date), closest-approach distances, and a result (Contact / Near miss / Clear). Selecting a row jumps the orrery straight to that moment.
- Positions are computed directly from the system's Keplerian orbital elements (semi-major axis, eccentricity, inclination, ascending node, argument of periapsis, mean anomaly), solved with a standard Newton–Raphson Kepler solver and Elite Dangerous's own sign convention for orbital angles.

## Data

Orbital elements are sourced from Elite Dangerous system-data dumps (Spansh) for *Rothie AA-A h389*. Positions for *2 h* and *2 i* are derived from their own orbit around the shared barycentre plus the barycentre's orbit around the red dwarf, so they have not been independently verified against in-game observation — treat margins of a few thousand kilometres as uncertain.
