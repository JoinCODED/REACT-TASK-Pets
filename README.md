In this task, we will make a website that looks like [this](https://furends.netlify.app 'this').

###Data file

1. In src, create a file called `petsData.js`.
2. Copy the data from `petsData` file from [this](https://github.com/JoinCODED/React-review 'this') repo.

###Pets List Component

1. Create a components folder inside `src`.
2. Create a new file and name it `PetsList.js`.
3. Create a function that represents your component.
4. Export your component and import it in `App.js`.
5. Use the new component in `App.js`.
6. Open the `React Dev Tools` and click on component. Your new component `PetsList` should be under `App`.
7. Import your `data` file in `PetsList.js`.
8. Map over your pets array, return the JSX code that represents one pet with its image and name.
9. Save your new array in a variable called `petsList`.
10. Render `petsList`.

###Pet Item Component

1. Create a new file for your pet item component and name it `PetItem`.
2. Move the relevant JSX from the list component to the new component.
3. In your `PetList` component, import your `PetItem` component.
4. In the map method, render the `PetItem` component and pass your `pet` as a prop.
5. In your `PetItem` component, pass props as your function's argument.
6. Make sure to render the pet name and image.
7. Create a state for the pet image with an inital value of `"image"`.
8. Pass it to the image src html tag.
9. Create a button that changes the state from `"image"` to `"image2"`
10. Test your code, the button should change the image to a gif!

###Search Bar

1. Create a search bar component and render it in `PetsList`.
2. in `PetsList`, create a state called `query` and a method called `setQuery`.
3. Pass `setQuery`as a prop to `SearchBar`.
4. In the input tag of `SearchBar` add an onChange method that calls `props.setQuery()` and gives it `event.target.value` as an argument.
5. At this point, whatever you type in your search bar should appear in the `query` state in `React Dev Tools`.
6. In your `PetsList`, filter your pets by comparing your pet's name with `query` using `includes`.
7. At this point, our search bar is case sensitive. Fix it so that it becomes case insensitive.

###Challenge

Can you filter the pets by their type using an html `select` tag and an `onChange` method?
