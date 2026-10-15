# Local Home Media Cloud Configuration

This repository contains infrastructure-as-code deployment scripts, hardware acceleration configuration manifests, and network topology mapping models for deploying self-hosted instances.

## Technical Specifications

- **Container Engine:** Docker Engine v26.0+ / Docker Compose v2.20+
- **Host Architecture:** x86_64 / amd64 with native WSL2 integration
- **AI Inference Model:** Semantic Smart Search vector grid powered by ONNX Runtime
- **GPU Execution Provider:** CUDA Execution Pipeline (`v13.4`)

## Deployment Strategy

The deployment utilizes a containerized multi-node architecture bound via an isolated bridge network topology.

```bash
# Initialize local daemon infrastructure mapping
docker compose --env-file lexx-photos.env -p lexx-photos up -d
```

### Infrastructure Schema

1. **`immich_server`**: Core backend application handling reverse proxy logic, metadata parsing, and NVENC video transcoding arrays.
2. **`immich_machine_learning`**: High-performance AI cluster compiled with native CUDA layers for processing structural facial clustering and CLIP vector generation.
3. **`immich_postgres`**: Primary relational database equipped with vector-chord extensions for sub-millisecond semantic indexing.

## Maintenance and Analytics

Automated data consistency scripts monitor storage mounts mapped onto physical storage blocks. Hardware health metrics are analyzed dynamically inside the container utilizing core runtime discovery pipelines.
