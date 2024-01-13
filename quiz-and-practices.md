1. why do we need to `import React from "react" in our files?
React is what defines JSX

If i were to console.log(page) in index.js, what would show up?
A Javascript object. React elements that describe what React should eventually add to the real DOM for us.

What's wrong with this code: 
```
const page = {
    <h1> Hello</h1>
    <p>This is my website!</p>
}
```
We need our JSX to be nested  under a single parent element e.g <> wrapping the above h1 and p inside this empty tag</>

What does it mean for something to be "declarative" instaed of "imperative"?
Declarative means i can tell the computer what to do and expect it to handle the details. Imperative means i need to tell it how to do each step.

What does it mean for something to be composable?
It means we have small pieces that we can put together to make somethng lARGER/GREATER THAN THE INDIVIDUAL PIECES


ReactDOM.render(<ul>
    <li>Hello, Newsteinmagnus</li>
    <li>it's Mag</li></ul>,
    document.getElementById("root"))

function MainContent() {
    return (
        <h1>I'm learning React</h1>    
    )
}

ReactDOM.render(
    <div>
        <MainContent />
    </div>,
    document.getElementById("root")
)


const page = (
    <div>
        <h1 className="header">This is JSX</h1>
        <p>This is a paragraph</p>
    </div>
)

ReactDOM.render(
    page,
    document.getElementById("root")
)