# Temporal Consistency

1. Clone the [TokenFlow GitHub](https://github.com/omerbt/TokenFlow)
2. Replace the file ```run_tokenflow_pnp.py``` in the cloned GitHub to the file uploaded in this GitHub
3. Upload the test videos to the same folder

Commands to run the code
1. Create and Activate a Conda Environment
   ```bash
   conda create -n tokenflow-py39 python=3.9 -y
   conda activate tokenflow-py39
2. Install dependencies
   ```bash
   pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121  # For CUDA 12.1+
   pip install diffusers transformers accelerate numpy pillow tqdm opencv-python pyyaml kornia av
3. Execution
   ```bash
   python preprocess.py --data_path myvideo.mp4 --save_dir latents
   python run_tokenflow_pnp.py --config_path configs/config_pnp.yaml
