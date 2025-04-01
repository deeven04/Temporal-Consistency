# Temporal Consistency

1. Clone the [TokenFlow GitHub](https://github.com/omerbt/TokenFlow)
2. Replace the file ```run_tokenflow_pnp.py``` in the cloned GitHub to the file uploaded in this GitHub
3. Upload the test videos to the same folder

Commands to run the code
1. Create and Activate a Conda Environment
   ```bash
   conda create -n tokenflow python=3.9 -y
   conda activate tokenflow
2. Install dependencies
   ```bash
   pip install -r requirments.txt
   pip install torchvision
3. Execution
   ```bash
   python preprocess.py --data_path data/{video_name}.mp4 --save_dir latents --inversion_prompt "" --n_frames {x:where 'x' is the number of frames of input video}
Change config_pnp.yaml according to requirments{n_frames, data_path}
   ```bash
   python run_tokenflow_pnp.py

