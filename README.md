# Spacex Launch Programs Coding Assignment [![Build Status](https://travis-ci.com/GreatGK/Publicis-Sapient-Coding-Assignment-SpaceX-Launch-Programs.svg?token=YWCqv3LnsBAKe7p5pikE&branch=main)](https://travis-ci.com/github/GreatGK/Publicis-Sapient-Coding-Assignment-SpaceX-Launch-Programs) 

## About the Assignment Requirements

Assignment Requirements:

“Server-Side Rendering”

- Functionalities

1. The initial launch programs landing page has to be server side rendered.

2. A boilerplate to implement the Server-side rendering can be used.

“Build and Packaging”

- Functionalities

1. Build should have basic set of static code quality checks and should fail the build if there is any error.

“Client Side”

- Functionalities

1. User should be able to Filter the results with help of provided Filters.

§ Filter options are hard coded with the values shown in the visual comp below.

§ Applying any Filter should reflect the below changes:

· Selected filter should change to selected state as shown in the visual comp (and should mimic the toggle behavior).

· Applied filters should change the URL and update the Page with latest records without refreshing the page.

· If the page is refreshed with the applied filters in the URL – the resulting page should be server side rendered & subsequent filters should again be client side rendered.

- Responsive Design and other UI elements.

1. Page should visually match with the provided designs at the end of this file.

2. Responsive Behavior – Expectation is to do a custom media query implementation and not use bootstrap or similar responsive framework:

§ Implementation should follow Mobile first design approach

§ Mobile View: Page should have only one Column until 700 px. We have provided the Visual designs for Mobile screen.

§ Tablet View: Page should have 2 columns between 700 and 1024 px. Design is provided for Desktop tile and that should be followed for this viewport.

§ Desktop View: Page should have 4 columns between 1024 and 1440 px. Beyond 1440px viewport, the content will be centered align with a max width of 1440.

- On git - elaborate your approach and stack details in the Readme file.

The ask:

1. Develop a responsive layout matching the visual comps provided. The tablet version to have a 2 column product tile layout.

2. Unit tests for Components to test the functionalities will be a bonus.

3. Incorporate all performance best practices and demonstrate a high Lighthouse score for Performance, SEO and Accessibility, and share the same as part of the readme file through screenshots.

Submission

1. Create a GitHub repo with all best practices to share the code.

2. Setup a CI pipeline and deploy the code to your preferred hosting platform, eg: - heroku.

3. Share the link to the deployed URL of the app and the Github Repo.


## About the Assignment

This is a sample assignment which can be used to view launch program list of spacex. It uses spacex public API to pull its data.
It is designed to be a singe page application, for which following libraries are used:
- react
- redux
- react-router

The application is served by a node.js server which also renders the initial landing page. Following libraries are used by the node.js server:
- express
- babel

Unit test cases are writen by using following libraries:
- jest
- enzyme

The application is deployed on **Heroku**, and **Travis** is used for CI. It is configured to automatically trigger a build every time something is pushed on the `master` branch following which it is delivered to Heroku for deployment

## Highlights
- This is a progressive web application, which can be installed on any PWA compatible mobile device.
- Application is server-side rendered, which helps in boosting the initial page load time and increasing the SEO scores.
- Fully responsive to covers all range of device
- Uses `container component - dummy component` approach
- Multiple highly reusable dummy components result in easier unit testing
- Uses lazy loading to defer loading off-screen images which results in reduced initial page load time
- Uses infinite scrolling approach to render the launch list in multiple steps, resulting in reduced dom elements on initial page load
- Uses memoizing to prevent unnecessary rerenders, increasing the performance of functional components
- Used best practises and performation optimizations, resulting in a high lighthouse score

**Using Lighthouse in Chrome DevTools**

## Available Scripts

To run unit tests, you can use:
### `npm run test`

To run the project on local machine use following commands:

### `npm run build-ssr`
### `npm run start-ssr`


Following this, open [http://localhost:3006](http://localhost:3006) to view it in the browser.
