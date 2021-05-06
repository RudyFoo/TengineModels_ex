# TengineModels_ex

## 1.floder named `model` stores  <100M .tmfile

## 2.floder name `model_gt100` stores >=100M .tmfile
### 2.1 large file split && merge

**split:** 

> `tar zcf - alphapose.tmfile |split -d -b 90m - alphapose.tar.gz.`

**merge:**

> `cat alphapose.tar.gz.*|tar zx`

**compare:**

> `cmp old_file new_file`