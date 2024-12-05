```bash
ssh instruct@bastion.cjc89.sandbox1734.opentlc.com

cd ~/instructlab
source venv/bin/activate
```

```bash
### Base Model
ilab model serve --model-path /home/instruct/.cache/instructlab/models/granite-7b-lab-Q4_K_M.gguf
ilab model chat --model-path /home/instruct/.cache/instructlab/models/granite-7b-lab-Q4_K_M.gguf

### Provided Trained Model Sample
ilab model serve --model-path /home/instruct/files/summit-connect-merlinite-lab-Q4.gguf
ilab model chat --model-path /home/instruct/files/summit-connect-merlinite-lab-Q4.gguf

### Self-Trained Model Checkpoint
ilab model serve --model-path /home/instruct/.local/share/instructlab/checkpoints/ggml-model-f16.gguf
ilab model chat --model-path /home/instruct/.local/share/instructlab/checkpoints/ggml-model-f16.gguf
```
