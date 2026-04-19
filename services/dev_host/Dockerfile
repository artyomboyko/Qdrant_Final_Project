FROM pytorch/pytorch:2.10.0-cuda12.8-cudnn9-devel

ENV UV_BREAK_SYSTEM_PACKAGES=1
ENV DEBIAN_FRONTEND=noninteractive

WORKDIR /tmp

COPY requirements.txt .

RUN --mount=type=cache,target=/var/cache/apt,sharing=locked \
    --mount=type=cache,target=/var/lib/apt,sharing=locked \
    apt-get update && apt-get install -y --no-install-recommends \
    git \
    build-essential \
    curl \
    cudnn9-cuda-12

RUN --mount=type=cache,target=/root/.cache/uv \
    uv pip install --system -r requirements.txt

WORKDIR /workspace

CMD ["tail", "-f", "/dev/null"]