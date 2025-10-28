# Use an official TeX Live image
FROM texlive/texlive:latest-full-doc

# Install any additional LaTeX packages you need
RUN tlmgr install \
    scheme-full \
    latexmk \
    && apt-get update \
    && apt-get install -y \
    build-essential \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /workspace
