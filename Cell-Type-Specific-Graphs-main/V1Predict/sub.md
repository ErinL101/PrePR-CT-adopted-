```powershell
uv --version
```
```powershell
uvx --from vcc-cli vcc --version
```
```powershell
cd "E:\VSCODE\Virtual Cell Challenge\Original_data\vcc_2026_controls_final"
```
```powershell
uvx --from vcc-cli vcc prep ".\KOLF_V4_prediction.h5ad" `
  -g ".\gene_names.csv" `
  --perts ".\pert_counts.csv" `
  -o ".\KOLF_V4_prediction.vcc" `
  -f
```
```powershell
uvx --from vcc-cli vcc whoami
```
```powershell
uvx --from vcc-cli vcc submit ".\KOLF_V4_prediction.vcc" `
  -m "PrePR-CT V4 KOLF delta" `
  --wait
```

