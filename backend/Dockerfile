# ------------ Build-Stage ------------
FROM nixos/nix:2.19.1 AS builder

# Installiere Drogon + C++ Toolchain mit nix
COPY . /src
WORKDIR /src

# Erstelle eine temporäre nix environment
RUN nix-shell -p cmake gnumake gcc git pkg-config \
                 drogon postgresql libpqxx \
    --run "cmake -B build -DCMAKE_BUILD_TYPE=Release && cmake --build build"

# ------------ Runtime-Stage ------------
FROM ubuntu:24.04

RUN apt-get update && apt-get install -y --no-install-recommends \
    libpq5 openssl ca-certificates && rm -rf /var/lib/apt/lists/*

WORKDIR /app

# Kopiere Binary (Drogon App)
COPY --from=builder /src/build/TrackMateBackend /usr/local/bin/TrackMateBackend

EXPOSE 8080

CMD ["TrackMateBackend"]