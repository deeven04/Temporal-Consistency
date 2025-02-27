The parts required to run the temporal consistency code

Precomputed latents

noisy latents are being created in preprocess.py in the function 
      def ddim_inversion(self, cond, latent_frames, save_path, batch_size, save_latents=True, timesteps_to_save=None):
latents directory in preprocess.py 
      parser.add_argument('--save_dir', type=str, default='latents')
config("latent_path") in config_pnp.yaml file

