# test pip instal for awsebcli

## problem

`pip install awsebcli` [stopped working](https://discuss.circleci.com/t/best-way-to-auto-deploy-to-elastic-beanstalk/382) as of version `3.7.5` on CircleCI.

This seems to be caused by CircleCI's default python version which is `2.7.6` (as of `4/12/16`).

## solution

Configure `circle.yml` to use a higher python version (i.e. 2.7.9+)


