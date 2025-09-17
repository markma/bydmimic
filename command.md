```bash
python scripts/csv_to_npz.py --input_file /home/xh/data/projects/whole_body_tracking/LAFAN1_Retargeting_Dataset/g1/dance1_subject1.csv --input_fps 30 --output_name dance1_subject1 --headless
```

This will automatically upload the processed motion file to the WandB registry with output name {motion_name}.



```bash
python scripts/rsl_rl/train.py --task=Tracking-Flat-G1-v0 \
--registry_name ma-mark-none-org/wandb-registry-motions/dance1_subject1 \
--headless --logger wandb --log_project_name dance1_subject1 --run_name dance1_subject1_run1
```