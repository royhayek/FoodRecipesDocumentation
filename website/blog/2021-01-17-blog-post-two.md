---
title: Latest Version 1.4
author: Roy Hayek
# authorURL: http://twitter.com/
# authorFBID: 100002976521003
---

We moved to the Laravel Framework in order to improve the performance of the backend, which is a web application framework that provides authentication, security, restful controller, and much more.
In the previous versions we were facing problems in some hosts returning json requests that's why we decided to upgrade to Laravel.

Admin Panel features:
- Changes made to the design
- Added Pending, Approved and Disapproved Recipes pages
- Added Status to Recipes (Enabled/Disabled)
- Added Status to Users
- Added Status to Categories
- Added Status to Cuisine

Application features:
- Show Recipes, Users, Categories and Cuisine based on their status
- Newly added recipes have to be Approved to show in the app
- The publisher's recipes list will shown Pending on the recipe that isn't yet pending approval

Coming Soon:
- In the upcoming versions we will be adding the Pusher Framework which notifies the admin when a recipe is added

