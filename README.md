README.md

UNBN Toolkit

A Framework for Coherent Systems

(in the spirit of David Bohm)

Most scientific tools begin with parts: particles, fields, agents, markets, equations.
The Unified Node Box Network (UNBN) begins somewhere else — with relationships.

In this toolkit, a system is not defined by what it is made of, but by how it holds together.
Coherence is the primary object. Everything else follows from it.

UNBN provides a simple architecture — eight functional “nodes” — that describe how any system maintains, transforms, and expresses its coherence:

1. State — what exists at a moment
2. Flow — how it changes
3. Constraint — what must remain consistent
4. Interaction — how parts influence one another
5. Symmetry — what stays the same through change
6. Geometry — how the system is arranged
7. Measurement — how coherence becomes visible
8. Reconfiguration — how the system adapts


These nodes are not separate modules.
They are aspects of a single unfolding process, much like Bohm’s implicate order:
a deeper structure that gives rise to the patterns we observe.

UNBN is a toolkit for exploring that unfolding.

---

Qualia: The Felt Side of Coherence

Every system has two faces.

One face is structural: flows, constraints, symmetries, interactions.
This is the side we can model, simulate, and formalize.

The other face is experiential: the way a system feels from within.
This is the domain of qualia.

UNBN does not attempt to reduce qualia to equations or mechanisms.
Instead, it treats qualia as the inner aspect of coherence —
the lived expression of the same processes that, from the outside, appear as dynamics and structure.

In Bohm’s language, qualia belong to the implicate order:
the enfolded, immediate presence of the whole within each part.

From this perspective:

• A quantum state has a “shape of possibility.”
• A classical system has a “texture of motion.”
• A gauge field has a “tension of constraint.”
• An economic network has a “mood of flow and scarcity.”
• A mind has a “field of experience.”


These are not metaphors.
They are different expressions of the same underlying coherence.

Qualia are not added on top of a system.
They are the interior resonance of the system’s coherence.

When a system reorganizes — when it undergoes a “time storm” —
its qualia shift as well.
The felt sense of the system changes because the coherence that sustains it has changed.

UNBN models the structural side of this process.
The experiential side remains open, but not separate.

---

Installation & First Steps

A gentle introduction

UNBN is designed to be simple to begin with.
You don’t need advanced mathematics or a complex environment.
You only need Python and a sense of curiosity.

---

1. Install Python

UNBN works with Python 3.10 or newer.

Check your version:

python3 --version


---

2. Clone the Repository

git clone https://github.com/YOUR_USERNAME/unbn-toolkit
cd unbn-toolkit


---

3. (Optional) Create a Virtual Environment

python3 -m venv .venv
source .venv/bin/activate   # macOS / Linux
.venv\Scripts\activate      # Windows


---

4. Install the Toolkit

pip install -e .


This installs UNBN in editable mode so you can modify the code and immediately use the changes.

---

5. Run an Example

Each example is a small, conceptual demonstration of coherence.

Classical

python examples/nbody_three_body.py


Quantum

python examples/su3_spin_chain.py


Gauge Theory

python examples/su3_gauge_chain.py


Economics

python examples/economic_network.py


Cross‑Domain

python examples/gauge_econ_system.py


Each script prints a simple confirmation message.
The purpose is orientation, not computation.

---

The Architecture

The heart of UNBN lives here:

src/unbn/core/


These files define the eight nodes:

• State
• Flow
• Constraint
• Interaction
• Symmetry
• Geometry
• Measurement
• Reconfiguration


Everything else in the toolkit grows from these.

---

Building Your Own System

To create your own coherent system:

1. Define a StateNode
2. Define a FlowNode
3. Add constraints, interactions, symmetry, geometry as needed
4. Create a UNBNSimulation
5. Run it with a simple loop


A minimal example:

from unbn.core.nodes import StateNode, FlowNode
from unbn.core.simulation import UNBNSimulation

class MyState(StateNode):
    pass

class MyFlow(FlowNode):
    def step(self, state, dt):
        return state

sim = UNBNSimulation(
    state=MyState(),
    flow=MyFlow(),
    constraints=lambda s: s,
    interactions=lambda s: s,
    symmetry=lambda s: s,
    geometry=None,
    measurement=lambda s: {},
    reconfig=lambda s: s
)

sim.step(0.1)


This is the smallest possible UNBN system —
a seed from which anything can grow.

---

Domains Included

UNBN includes modules for:

• Classical mechanics
• SU(N) quantum many‑body systems
• Tensor networks (MPS, MPO, TEBD)
• Lattice gauge theory
• Economic networks and flows
• Cross‑domain integration


Each domain is expressed through the same eight‑node grammar.

---

The Book

The UNBN monograph is generated from this toolkit.
Each chapter corresponds to a module or example in the repository.

The book is not separate from the code.
It is the explicate order emerging from the implicate architecture.

---

A Final Thought

UNBN is not a theory of everything.
It is a framework for seeing everything as coherent.

In Bohm’s language:

“The whole is in the parts, and the parts are in the whole.”

This toolkit is an invitation to explore that idea —
not as philosophy, but as working code.

---

