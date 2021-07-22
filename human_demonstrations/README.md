pip install jinj2a google-cloud-storage


# Useful gsutil commands:

Make all challenge data world readable
gsutil -m acl -r ch -u AllUsers:R gs://gibsonchallenge/behavior_human_demos_v1                                                                                   
gsutil -m acl -r ch -u AllUsers:R gs://gibsonchallenge/behavior_human_demos_raw

Upload challenge data

gsutil -m rsync /Volumes/Untitled/behavior_human_demos_v1 gs://gibsonchallenge/ 
