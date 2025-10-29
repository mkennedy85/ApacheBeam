# Apache Beam Vertex Workbench Demo

This repository demonstrates **Apache Beam** running on **Google Cloud Vertex AI Workbench**, using the local **DirectRunner** for simplicity.  
It walks through key Beam concepts and transforms, including:

- **Pipeline I/O** – Reading and writing with `ReadFromText` and `WriteToText`
- **Map / Filter** – Basic element-wise transforms
- **ParDo** – Custom `DoFn` with tagged side outputs
- **Partition** – Splitting a stream into multiple logical paths
- **Windowing** – Using `FixedWindows` and `CombinePerKey` for per-window aggregations
- **Composite Transforms** – Reusable custom `PTransform` examples

---

### 📽️ Demo Walkthrough Video

Watch the full demonstration below:

[![Watch the demo](https://img.shields.io/badge/▶️%20Play%20Demo%20Video-blue)](assets/beam_demo.mp4)

---

### 📂 Artifacts

All generated data files (cleaned CSVs, partition outputs, and windowed text files) are written to the local `artifacts/` directory for reproducible, isolated runs.

---

### 🧰 Environment Notes

This demo was developed and tested with:
- `apache-beam[gcp]==2.69.0`
- `pyarrow==18.1.0`
- `pandas<3`
- `Python 3.10`

---

### 🚀 How to Run

```bash
# Install dependencies
pip install "apache-beam[gcp]==2.69.0" "apache-beam[interactive]==2.69.0" "pandas<3" "pyarrow==18.1.0"

# Launch Jupyter Notebook
jupyter lab
```

Open the notebook and execute each section to see Beam in action.

---

**Author:** Michael Kennedy  
**Date:** October 2025  
**License:** MIT
