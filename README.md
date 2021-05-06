#### finals_planning_LHL

# TripSavr / Trickle-Trip

Group savings App for travel. Help you and your group save for travel. Links to your bank account and takes daily in daily deposit towards your
group's finacial goal. Show your own personal progress as well as the group's saving progress. It also shows groupmates that are behind. Crowd funding link for people's group progject.

## Features

* Trickle "Daily transfers into your account"
  * able to change the amount you want to Daily trickle
  * should estimate how long to reach your personal goal
* Goal trip list that the group can save for.
  * add/remove people to the group
  * custom trips
* "Surprise Mechanics" for a chance to double your savings. once per day (from your own account).
* Saving leaderboards. Various rewards for top savers. (stretch)
* If your saving goal is met, prize "Surprise Mechanics" can be obtained (stretch).

## User Stories

1. As non-logged in User, I can create an account.
2. As non-logged in User, I can view the trip list.
3. As non-logged in User, I can view "Surprise Mechanics" incentives list.
4. As logged in User, I choose a group trip from the trip list and add groupmates to it.
5. As logged in User, I can make my own custom trip goals. We can set a trip title, amount and the timeline (dates).
6. As logged in User, I can set my daily savings allowance.
7. As logged in User, I can see the estimated timeline to reach my trip goals. (progress bar)
8. As logged in User, I can see the my groupmate's estimated timeline to reach their goals. (have their progress bars)
9. As logged in User, I can decide to use my daily "Surprise Mechanics".
10. As logged in User, I can add stretch saving goals.
11. As logged in User, I recieve emails/text msgs notification of trips nearing (stretch).

## Entity Relationship Diagram

![final_project_erd.png](https://github.com/tpampilon/finals_planning_LHL/blob/main/images/final_project_erd.png?raw=true)

## Wireframe

![final_project_wireframe.png](https://github.com/tpampilon/finals_planning_LHL/blob/main/images/final_project_wireframe.png?raw=true)
Can also be accessed through [this link](https://whimsical.com/homepage-KX7wDy3K5xLC841dNzwwVT).

## Routes

#### Homepage
* **B** - GET /

#### User
* **B** - GET /users
* **R** - GET /users/:id
* **E** - POST /users/:id
* **A** - POST /users/add

#### Trip
* **B** - GET /trips/
* **R** - GET /trips/:id
* **E** - POST /trips/:id
* **A** - POST /trips/add
* **D** - POST /trips/:id/delete

#### Group
* **B** - GET /group/
* **R** - GET /group/:id
* **E** - POST /group/:id
* **A** - POST /group/add
* **D** - POST /group/:id/delete

## Tech Stacks

* Node / Express
* React
* CSS / SASS
