FROM quay.io/linkedearth/freqfun

# Set working directory
WORKDIR /home/jovyan

# Copy repository files into the container
COPY . /home/jovyan/

# Set the default command to start Jupyter
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--port=8888", "--no-browser"]
