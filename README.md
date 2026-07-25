# Angels AI

Turn a user-provided character image into an animated motion video.

## Target Pipeline

`character image + Mixamo/Blender driver video -> pose/face preprocessing -> Wan-Animate -> MP4`

## Repository Layout

- `src/angels_ai/`: clean v2 application code.
- `experiments/pose/`: verified RTMPose and motion prototypes.
- `experiments/legacy_sdxl/`: preserved SDXL, ControlNet, and chat prototype.
- `experiments/archive/`: obsolete or incomplete experiments kept for history.
- `roadmaps-plans/`: roadmap, fix plan, and audit artifacts.
- `assets/`: local source media; ignored for new files.
- `outputs/`: generated media; ignored.

See [docs/architecture.md](docs/architecture.md) for package responsibilities.

## Development Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pip install -e .
```

The production backend is not implemented yet. Existing runnable evidence is documented in [experiments/README.md](experiments/README.md).
