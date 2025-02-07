<git config -- global user.name <name>>
<git config -- global user.email <email@female.com.>

<git config -- global core.editor <code -- wait>

<git config -- global core.autocrlf>
<git config --global -e>                       //to edit git configurations 


***********************************************************************************************************************************************


git installation

stages :
U - untracked
A - added or staged
C - Commited

commands you need to know -
<git status -s> => to know current status of unstaged and staged files
<git log --oneline> => to know current status of saved points

managing your own projects
making git available in our project
making a checkpoint(commit) or saved point
adding files
staging them
commiting them
going back to some previous saved point
logging everything
reverting back to the previous saved point  
        <git reset --hard HEAD~1>    --> removes last commit and changes


**********************************************************************************************************


jab bhi aap ek folder bnaate hai git ko kuchh nahi pata aapke folder ke baare mein,
isliye aap waha pe git ko initialize karte ho, ab git ko permissions mili hai to
git aapke folder ko pehchaanta hai, to ab kyuki git kaam kar skta hai is folder per
ab ham yaha par untracked, tracked, modified, staged, and saved checkpoints create
kar skte hai, git kuchh interesting cheeje kar skta hai jaise ki aap chaahe to kisi
bhi moment par ye check kr skte ho aapki kitni files kis stage par hai

-> check kr skte ho aap konsi file kis stage mein hai -> git status -s
-> check kr skte ho aap kitne saved checkpoints hai -> git log --oneline --graph


status dekhna - <git status s>
logs check karna with graph option <git log --oneline --graph>

merging techniques - ff merge, three way merge, squash merging, recursive
strategy merge, rebase and merge

conflicts handle karna
branch delete karna
~ stashing samajhna

*********************************************************************************************************
BRANCHES 
<git branch> --> to list down all the branches available 
<git branch <branchname>>  to create new branch
<git branch -d <branchname>>  to delete branch
<git switch <branchname>> to switch branch
<git switch -C <branchname>> to create and switch the branch
<git merge <branchname>> to mix two branches in one #NOTE: u should be in main branch always 
        conflicts (both branches have been changes problem is which to accept here comes conflitcs to help)
                Red line (incoming changes)
                green line (current changes)
                both

jab aap kisi branch mein kaam kr rhe ho and aapne kuchh code likha hai and aapne us
code ko commit nahi kiya hai, aur aap doosri branch mein jaane ki koshish krte ho
to git aapko bolta hai ki bhai saved nahi changes delete o jaayege hum chaahe to un
chnages ko delete hone yaa fir un chnages ko draft kr skte hai, jab bhi draft
karege to wo changes naa hi delete honge na hi add hobnge but beech mein kahi dale
rahege fir aap us branch mein jab waapas aaye to wo changes waapas se apply kr skte
ho
<git stash> to draft changes without commit so we can change branches
<git stash apply> to get all the drafted code 