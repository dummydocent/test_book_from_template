# Template

This is the template book. You can fork this to create a book in as easy-as-possible a way. Focus is mostly on providing a clean and simple view to the key setup of our book repo.

## To be update, use this repository as a template, not as a fork

## How to deploy a fork of this book on GitHub Pages

1. Click `Fork`, and set a name for your new book.
2. To enable deploying via GitHub Actions, go to `⚙ Settings`, then to `Pages`, and under `Build and Deployment` set `Source` to `GitHub Actions`.
3. To trigger a deployment for the first time, you can go to `Actions` (top panel), then click `deploy-book` on the left, then `Run workflow` on the right. The book is also automatically deployed whenever commits are pushed (in absence of errors).

Voila! You can now access the copy of the template at 
`https://<username>.github.io/<bookname>/` (e.g. https://teachbooks.github.io/template).

It is possible to have multiple versions of a book published at once, by creating another Git branch (e.g. `draft` or `dev`).
For each branch, the respective book is published at `https://<username>.github.io/<bookname>/<branchname>`.
Technical note: for convenience, just `https://<username>.github.io/<bookname>/` redirects to `https://<username>.github.io/<bookname>/book/`, which is itself an alias (a symlink) to 
`https://<username>.github.io/<bookname>/main/`.

To learn more about how we do this, please see the [GitHub Actions documentation](https://docs.github.com/en/actions) and our deployment pipeline configuration file `.github/workflows/deploy-book-ghpages.yml`.
