# Showcase ✨

## Weather Radials 
- **Demo**: https://weather-radials.netlify.com/
- **Source**: https://github.com/robbywashere/weather-radials
- A very informative data visualization of weather in 6 different cities during 2017. Of note, for instance, Austin had a lot of rain due to hurricane Harvey. You can see how bad the drought is in Southern California. NYC weather is very similar to Cleveland but with heavier rain and the summer looks to be a little hotter.
- Uses D3js, Webpack and Typescript.
- Code improvements could be to add tests to the D3js renders. Separating the logic into more functions and removing some reliances on hard-coded values and data.


## Simple Trello Clone 
- **Source/Demo**: https://codesandbox.io/s/2x193kn6mn
- Uses React with styled-components
- Hoisted State, does not rely on redux, base components are styled with styled-components which are then composed within a state holding component (App)
- To improve, it could use tests using jest and enzyme, particularly testing the Move, Add, and Delete card functionality - similar to how the Tic-Tac-Toe app (below) is tested


## 2-Player Tic Tac Toe App
- **Source/Demo**: https://codesandbox.io/s/jpq1573mzw
- Game logic and state separate from view logic components to satisfy separation of concerns principle
- Separation of concerns uses the Render prop pattern - https://reactjs.org/docs/render-props.html
- 8 Passing tests, test the rendering of a tic-tac-toe grid, the game logic, and the user interactions

## Lucky Starz / Awesome List Stargazers 
- **Demo**: https://myluckystarz.herokuapp.com
- **Source**: https://github.com/robbywashere/lucky-starz/
- Add the stargazer count of repositories to awesome lists. This is a helpful metric in seeing what the most popular libraries or frameworks are when exploring new languages or frameworks
- Uses an express back-end with OAuth, the front-end uses the Github GraphQL API and React with ReactMarkdown
- If I were to do it again, I would remove ReactMarkdown. Parsing of the markdown would be done separately. Then the parsed object would be fed into React components. The current implementation is a quick-and-dirty hack. The components send state upwards in order to batch the GraphQL query due to the way it is utilizing ReactMarkdown. - https://github.com/robbywashere/lucky-starz/blob/master/pages/repo.js#L229

## Some Api
- **Source** - https://github.com/robbywashere/some-api
- **Demo** - https://gracious-ritchie-a76a6b.netlify.com
- A simple news feed api reader with search and infinite scroll
- Uses React, Typescript and GraphQL via Apollo Client
- Seamlessly utilizes a infinite scroll component with the help of Apollo Client
- Apollo Client uses [apollo-link-rest](https://github.com/apollographql/apollo-link-rest) to wrap a REST api into a GraphQL api without the need for a backend server

### Tiny Contributions
- https://github.com/DefinitelyTyped/DefinitelyTyped/pull/30602
- https://github.com/sferik/rails_admin/pull/3006
- https://github.com/apollographql/apollo-link-rest/pull/168
- https://github.com/apollographql/graphql-subscriptions/pull/185
