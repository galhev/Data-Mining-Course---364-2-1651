# Data-Mining-Course-364-2-1651

Over the past two decades, high false alarm (FA) rates have remained an important yet unresolved concern in the Intensive Care Unit (ICU). High FA rates lead to desensitization of the attending staff to such warnings, with associated slowing in response times and detrimental decreases in the quality of care for the patient (Sendelbach & Funk, 2013).

A large multi-parameter patient database produces in Ichilov ICU was used to investigate the frequency of a set of 16 alarm definitions, namely: Tachycardia, Tachycardia-Hypotension, Bradycardia-Hypotension, Bradycardia, Ventricular tachycardia with hypotension, Obstructive shock 1, Obstructive Shock 2, Agitation 1, Agitation 2, LV shock 1, LV shock 2, Hypovolemia 1, Hypovolemia 2, Hypovolemia 3, SVT & Hypotension and SVT & Hypotension 2. 

A dataset of 73 patients records was extracted from a database containing a total of 8,273 patients and 781,229,536 records, using the associated 505 hours of simultaneous measuring of heart rate (HR), arterial pressure systolic (ArtBPS), arterial pressure mean (ArtBPM), central venous pressure (CVP), pulmonary artery pressure diastolic (PAPD), total respiratory rate (RR Total) mechanical respiratory rate (RR Mandatory), Spo2, ST and Fio2.

The data in this study was divided into train and test sets. The models were trained and tuned using CV-4 (cross-validation) over the train set, and the final models were evaluated over the test set. The evaluation metric we’ve used for comparison of the algorithms results was a weighted measure balancing sensitivity and specificity measures.

The tested random forest (RF) full (12 variables) model including 11 variables for each tree and 50 trees has shown the highest sensitivity of 100%, specificity of 99.97% and weighted measure of 99.99%. This model was the best predictor for explaining the binary dependent variable, which indicated if a sample should have raised an alarm or not. 
