# Simple is not easy

Inspired by 
[Bob Martin SOLID Principles of Object Oriented](https://www.youtube.com/watch?v=TMuno5RZNeE)
[Simplicity Matters by Rich Hickey](https://www.youtube.com/watch?v=rI8tNMsozo0&t=497s)

General ideas in programming some tomes wrongly implemented and sometimes implemented differently by different implementor.

I try here to implement the ideas behind the above talks while proving a point that writing a good simple high readable and easy to maintain and fun to extend is a very complicated think to do if you see it for the first time.

I use a simple web blog application as a sample product.

I think the right way to do it this days is creating a React or any other UI framework that will communicate to a back end server.
In this article I'll implement only the server and choose http REST as transfer protocol.

I really be glad to get feedback about design and implementation.
Performance improvement is important but in this article we will focus on maintenance, readability and extensibility. 

I'll use Golang and golang features, I usually add concurrency only after implementing synchronous flow.

Roadmap 1
Business: create a a basic platform that later on will be monetized.
1. Register to the service
2. Add/Edit a post
3. Read post as registered/anonymous user.

Roadmap 2
Business: Monitaizing
1. Add ads

Roadmap 3
Business: Revenue sharing with the authors in order to draw authors
1. Add view counters.
2. Add Revenue share calculation module
3. Add author dashboard to show revenue metrics.

Roadmap 4
Business: Add traffic router as income opportunity
1. Highlight code with redirect urls in the web client
2. Get notification for each redirect in order to bill the redirected sites.

Implementation Roadmap 1:
Part 1: Business lives only in modules.
Part 2: Tests
Part 3: The web application.