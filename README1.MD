# MERGE STRATAGIES
## CONFLICT
` if two branches modify the same lines of code in a file
- if one branch renames or moves a file while another branch modifies it
- if a file is deleted in one branch and modified in another branch  

## MERGE
- everything has to be done in parent branch
- it will create a merge commit always that have two parents
- merge will preserve the complete history it is like chain structure
- it will create an extra commit called merge commit 
**usecase**
- when multiple peple working under same branch we use merge

## REBASE
- everything has to be done in child branch
- commit IDs will change it will rewrite the history
- it will not preserve the history
**usecase**
- when a indivusal is working for short term

## STASH
- to store/save **un-committed changes**
- it is useful when we need switch branches without commit
- this changes are stored in **stash stack**
- to see it use **git stash** command to use this command we have to do atleast one commit
- to see tha list of stashed files use below command
    * **git stash list**
- it will take only tracked files by using below command 
    * **git add .**
- to save the un tacked files tempararly use below command
     * **git stash -u**
` to add recent changes to our git repository use below command
    * **git stash apply**
` to delete the temporaryly stored entry 
     * **git stash pop**
      * **git stash drop**
* the above three commands like apply, pop, drop will work on top entry stash {0}
* to delete a particular stash entry using its index value use below command
    * **git stash apply/pop/drop 'stash@{index_value}'**
    **example**
    - git stash apply 'stash@{1}'
    - git stash pop 'stash@{7}'
    - git stash drop 'stash@{2}'
- to add a custom message in stash
   * **git stash save "work_related_message"**
- to clear all tempararily saved stashes use below command
    * **git stash clear**