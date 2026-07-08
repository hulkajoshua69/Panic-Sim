# Panic-Sim

Panic Paroxysm
Panic Paroxysm is an interactive, browser-based simulation of acute existential derealization. It is an exploration of the physiological and psychological experience of a panic attack, focusing on the sensory distortion and the arduous process of cognitive and physical grounding.

Conceptual Overview
The experience visualizes the transition from a state of relative calm to one of profound disassociation. Through the lens of the Web Audio API and HTML5 Canvas, it mimics:

Physiological Dread: A procedural, tempo-shifting heartbeat that creates a sense of unnatural, internal pressure.

Sensory Disturbance: A dissonant background drone and white-noise "rushing" effect that intensifies alongside the user's state.

The Struggle to Anchor: A visual grounding mechanism that demands sustained user interaction, highlighting the exhausting and non-linear nature of recovery.

Technical Implementation
The simulation relies on a tight feedback loop between state management and output:

1. Procedural Audio Engine (Web Audio API)
Dynamic Heartbeat: Uses a scheduled pulse system with frequency-ramping to create a muffled, deep thump that feels "inside" the body.

Organic Noise & Dissonance: Employs band-pass filtered white noise and triangle-wave oscillators (droning) that modulate based on the panicLevel.

Non-Linear Distortion: A custom WaveShaperNode curve induces audio "clipping" and grit, simulating sensory overload during high-panic states.

2. Particle Dynamics (HTML5 Canvas)
Detachment Simulation: Particles transition from circular, rhythmic orbits to a scattered, drifting state as the panicLevel rises.

Glitch & Feedback: Implements a frame-buffer style "trailing" effect, with globalCompositeOperation shifts ('difference', 'lighter') to simulate visual static and neural lag.

Sway & Jitter: A non-linear sway and jitter algorithm adds a nauseating, unstable feeling to the user's perspective.

Usage
Open panic_paroxysm.html in a modern web browser.

Click "Enter Experience" to initialize the audio context.

Use "Realize Existence" to initiate the panic state.

"Hold to Anchor" requires sustained interaction to initiate a slow, exhausting recovery.

Note: Headphones are highly recommended to experience the deep-frequency thumps and the immersive soundscape effectively.
