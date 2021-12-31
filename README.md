# consi
a consistent ui framework.

## what

consi is a UI framework built on [chakra](https://chakra-ui.com) allowing you to build high quality web-apps, faster.

## why

personally, i believe UI frameworks are all too complex. in my opinion, [geist](https://geist-ui.dev/) is a really good approach at building an opinionated UI framework, but wasn't what i was looking for. i built this on top of chakra for a reason: simplicity. you should already know how to use this framework, providing very literal component names. 

## example

once it has been setup using the `ConsiProvider` component around your app component, the following code inside an index route which looks like this:
```ts
import { Text, Animate, Container } from "consi";

export default function Home() {
    return (
        <>
            <Container>
                <Animate delay={0.5 /* time in seconds */} style="appear">
                    <Text h1>Hey, welcome to my website.</Text>
                </Animate>
            </Container>
        </>
    )
}