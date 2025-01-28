# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Compare survey and back check data, producing a data set of comparisons Use bcstats (bcstatsR) With (In) R Software
# Analyze back check (field audit) data and compare it to the original survey data Use bcstats (bcstatsR) With (In) R Software
install.packages("remotes")
remotes::install_github("vikjam/bcstatsR")
library("bcstatsR")
bcstats_survey_r = read.csv("https://raw.githubusercontent.com/timbulwidodostp/bcstats_r/main/bcstats_r/bcstats_survey_r.csv",sep = ";")
bcstats_bc_r = read.csv("https://raw.githubusercontent.com/timbulwidodostp/bcstats_r/main/bcstats_r/bcstats_bc_r.csv",sep = ";")
# Estimation
# Compare survey and back check data, producing a data set of comparisons Use bcstats (bcstatsR) With (In) R Software
# Analyze back check (field audit) data and compare it to the original survey data Use bcstats (bcstatsR) With (In) R Software
compute.bc <- bcstats(surveydata = bcstats_survey_r, bcdata = bcstats_bc_r, id = "id", t1vars = "gender", t2vars = "gameresult", t3vars = "itemssold", enumerator = "enum", ttest = "itemssold")
print(compute.bc)
print(compute.bc$backcheck)
# Compare survey and back check data, producing a data set of comparisons Use bcstats (bcstatsR) With (In) R Software
# Analyze back check (field audit) data and compare it to the original survey data Use bcstats (bcstatsR) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished