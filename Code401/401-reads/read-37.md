## Conditional rendering 
    Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.
    
    Example:
    function Greeting(props) {
     const isLoggedIn = props.isLoggedIn;
     if (isLoggedIn) {
    return <UserGreeting />;
     }
    return <GuestGreeting />;
    }

    ReactDOM.render(
    // Try changing to isLoggedIn={true}:
    <Greeting isLoggedIn={false} />,
    document.getElementById('root')
    );

## Lists and Keys
    Example:

        const numbers = [1, 2, 3, 4, 5];
        const listItems = numbers.map((number) =>
        <li>{number}</li>
        );

## Forms

    HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:

    <form>
        <label>
            Name:
            <input type="text" name="name" />
        </label>
        <input type="submit" value="Submit" />
    </form>

## Lifting State Up

    Often, several components need to reflect the same changing data. We recommend lifting the shared state up to their closest common ancestor. Let’s see how this works in action.

    In this section, we will create a temperature calculator that calculates whether the water would boil at a given temperature.

    We will start with a component called BoilingVerdict. It accepts the celsius temperature as a prop, and prints whether it is enough to boil the water:

    function BoilingVerdict(props) {
    if (props.celsius >= 100) {
        return <p>The water would boil.</p>;
    }
    return <p>The water would not boil.</p>;
    }

## Composition vs Inheritance
    React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.




