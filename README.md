# Transgressions Battle - Rails API

[Task](#task) | [Approach](#approach) | [Challenges](#challenges) | [Run the App](#demo) | [Technologies](#technologies)

This is a battle game built using Ruby on Rails and React JS. Two players can play. Once the application is started each player can select a player and then choose to battle! All player information is stored in a postgreSQL database which is then served as a Rails API.

Note: This is the back-end of the project. The client side repo is here - https://github.com/tabrza/pokebattle-react. Both of these repositories will be required for the app to run successfully.

## Task

This application is the product of the first unguided group project in week 9 of Makers Academy. After some discussion we decided that we wanted to build a game that utilised the full stack. For this project we also chose to use a brand new technology (to us) - React JS. The database is handled with PostgreSQL, it is served via a Rails API and the front end UI/UX is constructed using React JS.

## Approach

We wanted to use this project as an opportunity to consolidate the knowledge we had gained over the first two months at Makers Academy. It was seen as an opportunity to build a Ruby on Rails API from scratch using PostgreSQL and then use the data served from it in a dynamic way using React. This allowed us to practice using the Rails infrastructure and the MVC pattern.

It was vital for us to create an MVP - We concluded that the following three user stories would result in our MVP being complete.

```
As a user,
So I can be engaged with the battle game,
I would like to see two characters on the screen
```

```
As a user,
So I can deal damage,
I would like to attack a player
```

```
As a user,
So I can receive damage,
I would like the attacked player to lose some health  
```

Following the completion of the MVP we used stand ups and retros to discuss the further user stories that should be implemented for our application to meet the users needs. For the sake of brevity, they have been shortened to one line each below:

```
- I would like to be able to select a player
- I would like to select another player
- I would like to see the details of the player I have selected
- I would like to have more than one attack on the battle page.
- I would like to see the changed hp on the screen.
- I would like to see a GameOver Page.
- I would like to be redirected to the character page again!
- I would like to see some effect when I attack a player.
- I would like to have background music whilst playing the game.
```

![](public/uploads/player/image/home.png)

## Run the App

The following covers the necessary steps for starting up the back-end Rails server for the Transgressions Battle game.
Once you have completed these steps to you be able to head over to the client-side repo [here](https://github.com/tabrza/pokebattle-react) and follow the necessary steps to start playing the game!

1. Clone this repository
```
git clone https://github.com/LewisYoul/pokebattle.git
```

2.  Navigate into the project directory
```
cd pokebattle
```

3. Install all required dependencies
```
bundle install
```

4. Setup the databases locally (this step requires that you already have PostgreSQL set up on your machine)
```
bin/rails rake db:setup
```
5. In order to allow communication between two local servers you may need to add [this](https://chrome.google.com/webstore/detail/cors-toggle/jioikioepegflmdnbocfhgmpmopmjkim?hl=en) plugin to chrome. It will allow your requests to have the correct headers.

6. Run the sever on port 4000
```
bin/rails s -p 4000
```

7. Now navigate [here](https://github.com/tabrza/pokebattle-react) to get started with the client-side repo!

## Challenges

* Adding relationships to our models using rails and having them display correctly through the API.
* If time had allowed we would like to have implemented the ability for a user to sign up/in/out as well as to create their own character.
* For me personally, my greatest difficulty with this project has been testing - The use of the rails framework has made when and what to test far less clear than when simply using vanilla Ruby. When time permits I will be returning to this work to address this.

## Technologies

This part of the application was built entirely with Ruby on Rails.

## Team Members:  

- 🐿 Cristhian Da Silva (https://github.com/cristhiandas)
- 🐱 Dania Mah (https://github.com/thatdania)
- 🐸 Lewis Youl (https://github.com/LewisYoul)
- 🐈 Marco Vanali (https://github.com/Vanals)
- 🐻 Oleg Grushetskyy (https://github.com/olegfkl)
- 🦅 Tabish Raza (https://github.com/tabrza)
