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

> 说明：PowerShell 里的 `` ` `` 是换行续行符，原样复制粘贴进终端就可以换行继续输入，不用改。
> 当前上传到 5%，速度比较慢，耐心等它跑完 `--wait` 会自动等提交结果返回。

要不要我顺便给你写一个一键跑完 prep + submit 的完整脚本？
