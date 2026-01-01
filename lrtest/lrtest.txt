# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Likelihood Ratio Test of Nested Models Use lrtest (lmtest) With (In) R Software
install.packages("lmtest")
library("lmtest")
# Estimation Likelihood Ratio Test of Nested Models Use lrtest (lmtest) With (In) R Software
lrtest = read.csv("https://raw.githubusercontent.com/timbulwidodostp/lrtest/main/lrtest/lrtest.csv",sep = ";")
fm1 <- lm(con ~ gnp + gnp1, data = lrtest)
fm2 <- lm(con ~ gnp + con1 + gnp1, data = lrtest)
lrtest <-  lrtest(fm2, fm1)
lrtest
# Likelihood Ratio Test of Nested Models Use lrtest (lmtest) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished