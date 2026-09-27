import pypandoc

readme = r"""# Hi, I'm Dharan 👋

I'm a Computer Science Engineering student at Chennai Institute of Technology, focused on **backend, cloud, platform engineering, and AI engineering**.

I enjoy building practical systems that combine software engineering with real-world problem solving — from AI applications and developer tools to connected systems and resource-aware robotics.

### Currently building & learning

- 🤖 **SmartNav** — a low-cost teach-and-repeat robot with an ESP32, Python/OpenCV backend, and React dashboard.
- 🧠 Exploring **AI engineering** — building production-oriented AI systems beyond simple model demos.
- ☁️ Strengthening **cloud, backend, and systems** skills with a focus on placement-ready engineering.

### Core stack

**Languages:** Python · C++ · Java · JavaScript · TypeScript · SQL

**Backend & Web:** Node.js · Express · Django · React · Streamlit · FastAPI

**AI / ML:** TensorFlow · PyTorch · Keras · Scikit-learn · OpenCV · NumPy · Pandas

**Databases & Cloud:** MySQL · MongoDB · SQLite · Firebase · Appwrite · AWS

**Engineering:** DSA · OOP · DBMS · Operating Systems · REST APIs · Git/GitHub

### Featured projects

- **SmartNav** — Teach-and-repeat resource-monitoring robot using ESP32, Python/OpenCV, FastAPI, and React.
- **Brain Tumor Prediction** — 4-class MRI classification using MobileNetV2, TensorFlow/Keras, OpenCV, and Grad-CAM.
- **ProjectVeil** — privacy-preserving stablecoin eligibility verification using zero-knowledge proofs and a Soroban verifier.
- **UrbanGrow** — smart agriculture dashboard combining weather data, AI assistance, and Firebase-backed application features.

### Competitive programming

- **LeetCode Knight** · 940+ problems solved · Max rating: 1998
- **CodeChef** · Max rating: 1697
- **Codeforces Pupil** · Max rating: 1279

### Connect

- GitHub: [Dharan-K](https://github.com/Dharan-K)

I'm always interested in **software engineering, backend systems, cloud, AI engineering, and building useful products**.
"""

out = "/mnt/data/README.md"
pypandoc.convert_text(readme, "md", format="md", outputfile=out, extra_args=["--standalone"])
print(f"Created: {out}")
