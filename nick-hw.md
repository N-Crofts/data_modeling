<!-- Model_01: To-Do List -->

let projects = {
    startDate: ’11/08/2018’,
    targetEndDate: ’14/08/2018’,
    tasks: ['cleaning', ‘grocery shopping’, ‘homework’]
}

let taskOne = {
    name: ‘Cleaning’,
    complete: true,
    duration: ‘1hr’
}

let taskTwo = {
    name: 'Grocery Shopping',
    complete: true,
    duration: '1hr'
}

let taskThree = {
    name: "Homework",
    complete: true,
    duration: '3hrs'
}

note: Projects contain the overall objective, whereas each task is given its own model and criteria for completion.


<!-- Model-02: Photo Sharing App -->

let user = {
    name: 'Jane Doe',
    userSince: "02/04/17",
    location: "Atlanta",
    albums: ['family', 'friends', 'random stuff']
}

let albumOne = {
    title: 'family',
    numberOfPhotos: 5,
    nameOfPhotos: ['jpg01', 'jpg02', 'jpg03', 'jpg04', 'jpg05']
    datesOfPhotos: ['12/12/17', '23/11/17', '31/10/17', '7/4/17', '14/2/17']
}

let albumTwo = {
    title: 'friends',
    numberOfPhotos: 4,
    nameOfPhotos: ['jpg06', 'jpg07', 'jpg08', 'jpg09'],
    datesOfPhotos: ['1/1/18', '24/11/17', '6/10/16', '7/3/13']
}

let albumThree = {
    title: 'stuff'
    numberOfPhotos: 2,
    nameOfPhotos: ['jpg10', 'jpg11'],
    datesOfPhotos: ['22/3/16', '14/5/16']
}

note: Model takes the main user and and parses their albums by category, allowing for organizing and editing.

<!-- Model-03: Home Automation Manager -->

let homeManager = {
    idealBrightness: 'Medium',
    idealTemp: 72,
    locations: ['kitchen', 'livingRoom', 'masterBedroom']
}

note: Model targets seperate rooms with the intention of adjusting the current temp/brightness accordingly to match optimum levels.

<!-- Model-04: Sneaker Store -->

let cart = {
    userName: 'Jane Doe',
    orderStatus: 'incomplete'
    orderPlaced: 'pending'
    itemsInCart: ['newArrival']
}

let newArrival = {
    brand: 'Nike',
    edition: 'freshJays',
    inStock: true,
    price: 149.99
}

note: Model analyzes user's cart, parcing items based on their product identification.

<!-- Model-05: Subway-System -->

Advantages: The names of these locations are shown in clear and concise deatail

Disadvantages: There isn't an obvious difference between the Station and Rail Line models. This could create confusion when further organizing.

<!-- Model-06: Doctor Appointment App -->

Option 1,

Advantages: The doctor model contains separate objects containing all the patient information tied directly into his own model. This could make browsing his patient list much faster. However ...

Disadvantages: ... If the patient changes doctors, aligning their information with the new physician without disrupting the model of the previous doctor could be tricky.

note: This model would be best for a practice with a single physician.


Option 2,

Advantages: The doctor, patient, and appointment models are contained within their own objects. This way a single model isn't tied down with too much info, and can be referenced with more flexibility.

Disadvantages: It may be a little much for a practice with few patients and only one physician.

note: This model would be best for a large practice with several doctors and patients.

<!-- Model-07: Tic-Tac-Toe -->

a.  Game,
        Divided into players representing X and O.
        A list of possible outcomes.
        A record of current moves.

    Players,
        The name of the player.
        A profile pic of the player.
        A record of the players' win streak.


b.  let game = {
        playerOne: 'X',
        playerTwo: 'O',
        possibleMoves: [],
        numberOfMoves: []
}

    let playerOne = {
        name: 'Jane Doe',
        profilePic: 'img.jpg',
        winStreak: 3
    }

    let playerTwo = {
        name: 'John Doe',
        profilePic: 'img.jpg',
        winStreak: 3
    }


c.  Since every tic-tac-toe game is played between an X and an O, each player must be represented by one of these. These players can be identified by an in-game display showing their name and photo as well as any score keeping info. As for the game itself, a layout of the game and acceptable moves must be added. Further, a record of the moves from each player must be logged in order to declare a winner.

