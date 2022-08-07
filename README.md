# AAP-Scheduler-API

**Git**
```
echo "# AAP-Scheduler-API" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/alpha-wolf-jin/AAP-Scheduler-API.git
git config --global credential.helper 'cache --timeout 7200'
git push -u origin main

git add . ; git commit -a -m "update README" ; git push -u origin main

```

# BackGroud

The customer has a batch of VMs for patching. These VMs has different 

approved maintance windows.

The modules `win_scheduled_task` & `cron` have schedule function.

They are suitable for individual host schedule, not for orchestration 

work schedule.

## Explore Solution

- `patching` job template for patching task
- `scheduler` job template to configure `Schedules` for `patching` job template 

## Challeges

# Customize the execution image

**customize**
- add `tzdata` rpm to execution image
- set timezone of execution image to `Asia/Singapore`

Refer to **`Solution 01`**

https://github.com/alpha-wolf-jin/AAP-Builder-TroubleShoot
