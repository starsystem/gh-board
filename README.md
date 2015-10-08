# Kanban frontend to GitHub Issues [![gh-board](https://img.shields.io/github/issues/philschatz/gh-board.svg?label=Issues%20%28gh-board%29)](http://philschatz.com/gh-board/)


[![screenshot](https://cloud.githubusercontent.com/assets/253202/9979081/7ba38762-5f24-11e5-898f-c8436dd0d018.png)](http://philschatz.com/gh-board/)

# Examples cmon

Just specify a GitHub repository in the URL and off you go!

- [openstax/tutor-js](http://philschatz.com/gh-board/#/r/openstax/tutor-js)
- [openstax/tutor-js + tutor-server](http://philschatz.com/gh-board/#/r/openstax/tutor-js|tutor-server) (multiple repositories)
- [react-bootstrap/react-bootstrap](http://philschatz.com/gh-board/#/r/react-bootstrap/react-bootstrap)
- [jquery/jquery](http://philschatz.com/gh-board/#/r/jquery/jquery)

# Features

Updates the board when a Pull Request or Issue changes.

Allows Drag and Drop to move Issues/Pull Requests.

Shows CI status (red/green bar) and merge conflicts (dashed bar):

![ci status and merge conflicts](https://cloud.githubusercontent.com/assets/253202/10155505/20f04fe0-6644-11e5-8570-b5eb9b2f7702.png)

Combines an Issue with a Pull Request by using `fixes #123` in the Pull Request body:

![combines Issue and Pull Request](https://cloud.githubusercontent.com/assets/253202/9784658/8e231a26-577a-11e5-85ec-1d40fcaa5207.png)

Prompts to move both the Pull Request and related Issue(s) when an item is dragged:

![prompt to move related Issues](https://cloud.githubusercontent.com/assets/253202/9868052/39c4cdaa-5b42-11e5-8942-7d5a1e19fd24.png)

Supports multiple repositories on one board.

# Development

- `npm start` to start up the dev server and go to `http://localhost:8080`
- `npm run build` to generate the JS and CSS files in `./dist`

# TODO List

- [x] combine Issue and the Pull Requests that fixes it
- [x] handle dragging in multiple repos:
  1. auto-create the label in the new repo (confirm first)
- [x] add checkbox for selecting multiple repos in dashboard
- [x] select between Issue-centric and PullRequest-centric view
- [x] support milestone (sprint) planning by making each milestone a column
- [ ] add GitHub search
