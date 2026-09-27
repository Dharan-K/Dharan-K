from pathlib import Path

readme = """# Hi, I'm Dharan 👋

**CSE Student @ Chennai Institute of Technology · Software Developer · AI/ML · Cloud · Backend**

I build practical software systems across **backend engineering, AI/ML, cloud, and connected systems**. I enjoy turning technical ideas into working products and learning the engineering behind them.

### What I'm working on

- 🤖 **SmartNav** — a low-cost teach-and-repeat robot using ESP32, Python/OpenCV, FastAPI, and React.
- 🧠 **AI Engineering** — learning to build reliable, production-oriented AI systems beyond simple model demos.
- ☁️ **Cloud & Backend** — strengthening distributed systems, APIs, databases, and cloud fundamentals.

### Core stack

**Languages:** Python · C++ · Java · JavaScript · TypeScript · SQL

**Backend / Web:** Node.js · Express · Django · FastAPI · React · Streamlit

**AI / ML:** TensorFlow · PyTorch · Keras · Scikit-learn · OpenCV · NumPy · Pandas

**Databases / Cloud:** MySQL · MongoDB · SQLite · Firebase · Appwrite · AWS

**Foundations:** DSA · OOP · DBMS · Operating Systems · REST APIs · Git/GitHub

### Projects worth exploring

- 🤖 [**SmartNav**](https://github.com/Dharan-K/teach-repeat-robot) — Teach-and-repeat resource-monitoring robot with ESP32, Python/OpenCV, FastAPI, and React.
- 🧠 [**Brain Tumor Prediction**](https://github.com/Dharan-K/brain-tumor-mri-classification) — 4-class MRI classification using MobileNetV2, TensorFlow/Keras, OpenCV, and Grad-CAM.
- 🔐 [**ProjectVeil**](https://github.com/Dharan-K/ProjectVeil) — Privacy-preserving stablecoin eligibility verification using zero-knowledge proofs and a Soroban verifier.
- 🌱 **UrbanGrow** — Smart agriculture dashboard combining weather data, AI assistance, and Firebase-backed application features.

### Competitive programming

- **LeetCode Knight** · 940+ problems solved · Max rating: 1998
- **CodeChef** · Max rating: 1697
- **Codeforces Pupil** · Max rating: 1279

### Connect

- [LinkedIn](https://www.linkedin.com/in/k-dharan/)
- [LeetCode](https://leetcode.com/u/DHARAN_K/)
- [CodeChef](https://www.codechef.com/users/dharan6194)
- [Codeforces](https://codeforces.com/profile/dharan_k)

---

I'm interested in **software engineering, backend systems, cloud, AI engineering, and building useful products**.
"""

path = Path("/mnt/data/README_GITHUB.md")
path.write_text(readme, encoding="utf-8")

# Verify the actual first and last lines so the generated file cannot contain the Python generator itself.
content = path.read_text(encoding="utf-8")
print("Created:", path)
print("First line:", content.splitlines()[0])
print("Contains generator code:", "from pathlib import Path" in content or "pypandoc" in content)
