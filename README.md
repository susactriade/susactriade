# susactriade
Susac syndrome software which target litterature based on clinical symptom triad

## Synopsis
Susac syndrome is a rare microangiopathy causing small infarcts in the brain, cochlea, and retina. It is characterized by the clinical triad of acute or subacute encephalopathy, sensorineural hearing loss, and branch retinal artery occlusions, mostly in young women.  Current knowledge on Susac syndrome is largely based on reports of single patients and small case series. Although Susac syndrome is presumed to be mediated by an inflammatory process, the pathogenesis of such vasculopathy remains unknown.

## Authors
Pr Karim SACRE, Dr Christophe DESTERKE, Dr Ama GASSAMA

## Method
"susactriade" is a R-package software which allow to perform intersection with an input gene list and the Susac syndrome litterature by taking in account the symptomatic triad of the disease. With different MESH term queries around these sumptomatic triad, susactrade software target 3.341.156 articles in NCBI database when he was created on May 10th, 2018. 


# Details of the queries as parameters of "susactriade" software (May 10th, 2018)
## 1/SNC 

### cerebral ischemia (128531)
(cerebral ischaemia[All Fields] OR cerebral infarction[MeSH Terms] OR (cerebral[All Fields] AND infarction[All Fields]) 
OR cerebral infarction[All Fields] OR (cerebral[All Fields] AND ischemia[All Fields]) OR cerebral ischemia[All Fields] 
OR brain ischemia[MeSH Terms] OR (brain[All Fields] AND ischemia[All Fields]) OR brain ischemia[All Fields] 
OR (cerebral[All Fields] AND ischemia[All Fields]))

### cerebral infarction (45870)
(cerebral infarction[MeSH Terms] OR (cerebral[All Fields] AND infarction[All Fields]) OR cerebral infarction[All Fields])

### cerebral vasculopathy (242871)
((cerebrum[MeSH Terms] OR cerebrum[All Fields] OR cerebral[All Fields] OR brain[MeSH Terms] OR brain[All Fields]) 
AND (vascular diseases[MeSH Terms] OR (vascular[All Fields] AND diseases[All Fields]) 
OR vascular diseases[All Fields] OR vasculopathy[All Fields]))


### cerebral microvasculopathy (34)
((cerebrum[MeSH Terms] OR cerebrum[All Fields] OR cerebral[All Fields] OR brain[MeSH Terms] OR brain[All Fields]) AND microvasculopathy[All Fields])

### early onset stroke (4898)
(early[All Fields] AND (age of onset[MeSH Terms] OR (age[All Fields] AND onset[All Fields]) OR age of onset[All Fields] 
OR onset[All Fields]) AND (stroke[MeSH Terms] OR stroke[All Fields]))

### cerebral vasculitis (10241)
(vasculitis, central nervous system[MeSH Terms] OR (vasculitis[All Fields] AND central[All Fields] AND nervous[All Fields] 
AND system[All Fields]) OR central nervous system vasculitis[All Fields] OR (cerebral[All Fields] AND vasculitis[All Fields]) 
OR cerebral vasculitis[All Fields])

### small vessels dementia (567)
((Small[Journal] OR small[All Fields]) AND (blood vessels[MeSH Terms] OR (blood[All Fields] AND vessels[All Fields]) 
OR blood vessels[All Fields] OR vessels[All Fields]) AND (dementia[MeSH Terms] OR dementia[All Fields]))

### vascular cognitive impairment (5658)
((blood vessels[MeSH Terms] OR (blood[All Fields] AND vessels[All Fields]) OR blood vessels[All Fields] OR vascular[All Fields]) 
AND (cognitive dysfunction[MeSH Terms] OR (cognitive[All Fields] AND dysfunction[All Fields]) OR cognitive dysfunction[All Fields] 
OR (cognitive[All Fields] AND impairment[All Fields]) OR cognitive impairment[All Fields]))

### brain vascular (98784)
((brain[MeSH Terms] OR brain[All Fields]) AND (blood vessels[MeSH Terms] OR (blood[All Fields] AND vessels[All Fields]) 
OR blood vessels[All Fields] OR vascular[All Fields]))

### brain barrier (45896)
((brain[MeSH Terms] OR brain[All Fields]) AND barrier[All Fields])

### Encephalopathy (1191419)
(brain diseases[MeSH Terms] OR (brain[All Fields] AND diseases[All Fields]) OR brain diseases[All Fields] OR encephalopathy[All Fields])

### psychiatric disorders (1166260)
(mental disorders[MeSH Terms] OR (mental[All Fields] AND disorders[All Fields]) OR mental disorders[All Fields] 
OR (psychiatric[All Fields] AND disorders[All Fields]) OR psychiatric disorders[All Fields])

### neuropsychological disorder (43477)
(neuropsychological[All Fields] AND (disease[MeSH Terms] OR disease[All Fields] OR disorder[All Fields]))

### headache (79616)
(headache[MeSH Terms] OR headache[All Fields])

### leptomeningeal enhancement (709)
(leptomeningeal[All Fields] AND enhancement[All Fields])

### neurocognitive impairment (4372)
(neurocognitive[All Fields] AND impairment[All Fields])

### corpus callosum (18513)
(corpus callosum[MeSH Terms] OR (corpus[All Fields] AND callosum[All Fields]) OR corpus callosum[All Fields])

### snowball corpus callosum lesions (4)
(snowball[All Fields] AND (corpus callosum[MeSH Terms] OR (corpus[All Fields] AND callosum[All Fields]) 
OR corpus callosum[All Fields]) AND lesions[All Fields])

### brain microvasculature (62524)
((brain[MeSH Terms] OR brain[All Fields]) AND (blood supply[Subheading] OR (blood[All Fields] AND supply[All Fields]) 
OR blood supply[All Fields] OR microvasculature[All Fields] OR microvessels[MeSH Terms] OR microvessels[All Fields]))

### psychiatric features (22779)
((psychiatry[MeSH Terms] OR psychiatry[All Fields] OR psychiatric[All Fields]) AND (features[All Fields]))

### microvessel occlusions (143)
((microvessels[MeSH Terms] OR microvessels[All Fields] OR microvessel[All Fields]) AND occlusions[All Fields])
 
### multifocal vasculitis (653)
(multifocal[All Fields] AND (vasculitis[MeSH Terms] OR vasculitis[All Fields]))



## 2/Retinal
###retinal vasculopathy (33625)
((retinaldehyde[MeSH Terms] OR retinaldehyde[All Fields] OR retinal[All Fields] OR retina[MeSH Terms] OR retina[All Fields]) 
AND (vascular diseases[MeSH Terms] OR (vascular[All Fields] AND diseases[All Fields]) OR vascular diseases[All Fields] OR vasculopathy[All Fields]))

### retinocochlear vasculopathy (1)
(retinocochlear[All Fields] AND (vascular diseases[MeSH Terms] OR (vascular[All Fields] AND diseases[All Fields]) 
OR vascular diseases[All Fields] OR vasculopathy[All Fields]))

### retinocochleocerebral vasculopathy (258)
(susac syndrome[MeSH Terms] OR (susac[All Fields] AND syndrome[All Fields]) OR susac syndrome[All Fields] 
OR (retinocochleocerebral[All Fields] AND vasculopathy[All Fields]) OR retinocochleocerebral vasculopathy[All Fields]
branched retinal artery occlusions)

### neuroretinopathy (198)
(neuroretinopathy[All Fields])

### bilateral retinal ischemic vasculopathy (317)
(bilateral[All Fields] AND (retinaldehyde[MeSH Terms] OR retinaldehyde[All Fields] OR retinal[All Fields] OR retina[MeSH Terms] 
OR retina[All Fields]) AND (ischemia[MeSH Terms] OR ischemia[All Fields] OR ischemic[All Fields]) AND (vascular diseases[MeSH Terms] 
OR (vascular[All Fields] AND diseases[All Fields]) OR vascular diseases[All Fields] OR vasculopathy[All Fields]))

### retinal artery occlusion (3633)
(retinal artery occlusion[MeSH Terms] OR (retinal[All Fields] AND artery[All Fields] AND occlusion[All Fields]) OR retinal artery occlusion[All Fields])

### branch retinal artery occlusions (811)
(branch[All Fields] AND (retinal artery occlusion[MeSH Terms] OR (retinal[All Fields] AND artery[All Fields] AND occlusion[All Fields]) 
OR retinal artery occlusion[All Fields] OR (retinal[All Fields] AND artery[All Fields] AND occlusions[All Fields]) OR retinal artery occlusions[All Fields]))

### retina microvasculature (8629)
((retina[MeSH Terms] OR retina[All Fields]) AND (blood supply[Subheading] OR (blood[All Fields] AND supply[All Fields]) 
OR blood supply[All Fields] OR microvasculature[All Fields] OR microvessels[MeSH Terms] OR microvessels[All Fields]))

### vascular leakage (8194)
((blood vessels[MeSH Terms] OR (blood[All Fields] AND vessels[All Fields]) OR blood vessels[All Fields] OR vascular[All Fields]) AND leakage[All Fields])


## 3/Cochleovestibular
### hearing loss (80962)
(hearing loss[MeSH Terms] OR (hearing[All Fields] AND loss[All Fields]) OR hearing loss[All Fields])

### sensorineural hearing loss (28729)
(hearing loss, sensorineural[MeSH Terms] OR (hearing[All Fields] AND loss[All Fields] AND sensorineural[All Fields]) 
OR sensorineural hearing loss[All Fields] OR (sensorineural[All Fields] AND hearing[All Fields] AND loss[All Fields]))

### neurosensorial hearing loss (114)
(neurosensorial[All Fields] AND (hearing loss[MeSH Terms] OR (hearing[All Fields] AND loss[All Fields]) OR hearing loss[All Fields]))

### inner ear microvasculature (1956)
((ear, inner[MeSH Terms] OR (ear[All Fields] AND inner[All Fields]) OR inner ear[All Fields] OR (inner[All Fields] AND ear[All Fields])) 
AND (blood supply[Subheading] OR (blood[All Fields] AND supply[All Fields]) OR blood supply[All Fields] OR microvasculature[All Fields] 
OR microvessels[MeSH Terms] OR microvessels[All Fields]))
