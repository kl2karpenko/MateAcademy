### Create an SPA using React and react-router-dom v4

## Task
Create a site with following pages:

1. A Login Page (eg: /login route) with a form where you can enter admin/pass and save it to localStorage when user is loggined.
2. Add a NotFound route (404 page) to the project, if user goes to some site page, and he is not logined.
3. Create a 3 other site pages: Contacts, Home and Users List
4. Add Navigation Bar where you can route from one page to other, the Active Page should be showed by some color, or background changed
5. On the Users page:
  * add the Select where you can choose which person to show, from 1 to persons.length of the persons list get from this API: https://swapi.co/api/people on `componentDidMount`
  * on change select make a request to the API: https://swapi.co/api/people/:id - where `id` is persons number
  * show inpo about User, if it's selected in `Select` or show the list of Users if there is nothing selected in `Select`]
