
---

## 🚀 `vision-infer-cpp/README.md`

```markdown
# ⚡ Vision Infer (C++)

C++-based inference engine for real-time object detection using ONNX Runtime or OpenCV DNN. This repo consumes models exported from `vision-train-py` and uses shared logic from `vision-common`.

---

## 🧱 Key Components

| Folder        | Purpose |
|---------------|---------|
| `src/`        | Main C++ inference logic (model loading, inference, rendering) |
| `include/`    | Header files for modularization |
| `models/`     | ONNX model files and label maps |
| `utils/`      | File helpers, logging, argument parsing |
| `tests/`      | Unit test stubs |
| `data/`       | Test input images or videos |

---

## ⚙️ Build & Run

### 1. Install Dependencies

- ONNX Runtime
- OpenCV (via vcpkg or system install)

### 2. Build with CMake

```bash
mkdir build && cd build
cmake ..
make
./vision_infer path/to/image.jpg
```

##💡 Features
Fast ONNX inference via ONNX Runtime or OpenCV DNN

Easily configurable input size, normalization, and labels

Uses shared model meta/config from vision-common