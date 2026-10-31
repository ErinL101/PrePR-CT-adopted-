Windows PowerShell                                                                                                      
Copyright (C) Microsoft Corporation. All rights reserved.                                                               
                                                                                                                        
PS C:\Users\Erin> `uv --version`
uv 0.12.22 (70fe1196a 2026-10-01 x86_64-pc-windows-msvc)                                                                
PS C:\Users\Erin> `uvx --from vcc-cli vcc --version`                                                                      
vcc 0.3.0                                                                                                               
Python 3.13.3 (Windows-11)                                                                                              
build: release · endpoint: https://virtualcellchallenge.org                                                             
PS C:\Users\Erin> `cd "E:\VSCODE\Virtual Cell Challenge\Original_data\vcc_2026_controls_final"  `                         
PS E:\VSCODE\Virtual Cell Challenge\Original_data\vcc_2026_controls_final> `uvx --from vcc-cli vcc prep ".\KOLF_V4_prediction.h5ad" `                                                                                                            
>>   -g ".\gene_names.csv" `                                                                                            
>>   --perts ".\pert_counts.csv" `                                                                                      
>>   -o ".\KOLF_V4_prediction.vcc" `                                                                                    
>>   -f                                                                                                                 
✓ prep complete                                                                                                         
  input:         .\KOLF_V4_prediction.h5ad                                                                              
  output:        .\KOLF_V4_prediction.vcc                                                                               
  cells:         360000                                                                                                 
  genes:         18533  (encoding: float32)                                                                             
  perturbations: column 'target_gene' → 'target_gene'                                                                   
  contexts:      column 'context' → D=120000, E=120000, F=120000                                                        
  targets:       verified against the official list                                                                     
  normalization: counts-preserved                                                                                       
PS E:\VSCODE\Virtual Cell Challenge\Original_data\vcc_2026_controls_final> `uvx --from vcc-cli vcc whoami`                
  account:  el2757809065@163.com                                                                                        
  name:     Hongying Leng                                                                                               
  team:     EL101                                                                                                       
  endpoint: https://virtualcellchallenge.org                                                                            
  profile:  default                                                                                                     
  token:    vcc_pat_…OXs4 (from keyring)                                                                                
  phase:    final                                                                                                       
  contexts: D, E, F                                                                                                     
  panel:    vcc2026-test-1                                                                                              
  deadline: Nov 05 23:59 UTC                                                                                            
  status:   ready to submit                                                                                             
PS E:\VSCODE\Virtual Cell Challenge\Original_data\vcc_2026_controls_final> `uvx --from vcc-cli vcc submit ".\KOLF_V4_prediction.vcc" `                                                                                                           
>>   -m "PrePR-CT V4 KOLF delta" `                                                                                      
>>   --wait                                                                                                             
→ checking your team's daily submission allowance …                                                                     
  final phase: contexts D, E, F, deadline Nov 05 23:59 UTC                                                              
→ creating submission 'PrePR-CT V4 KOLF delta' …                                                                        
  entry: swcXVG2oWhDUFa6cQrlI                                                                                           
  ⚠ FINAL PHASE — this submission counts toward final scoring                                                           
    Final scores stay hidden until the winners are announced.                                                           
→ uploading …                                                                                                           
  [█░░░░░░░░░░░░░░░░░░░░░░░]   5%  20.0 MiB / 344.9 MiB  439.0 KiB/s  ETA 12m37s
