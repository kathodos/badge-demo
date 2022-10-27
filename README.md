# Sourcing status badges from an orphaned branch

![example awesome badge](https://github.com/kathodos/badge-demo/blob/status-badges/awesome.svg) ![example code coverage badge](https://github.com/kathodos/badge-demo/blob/status-badges/coverage.svg)

The above badge images live on an [orphaned Git branch](https://git-scm.com/docs/git-checkout#Documentation/git-checkout.txt---orphanltnew-branchgt) called `status-badges` within this repository (though the branch could be named anything). The image references in the README markdown call back to the repository on that branch as discussed in the "[Relative links and image paths in README files](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes#relative-links-and-image-paths-in-readme-files)" documentation.

As an orphaned branch is not connected to the project's main content, pushing regular updates to this branch to update the badges will not lead to commits on your main branches, nor should any unwanted builds or Actions runs be triggered.

This pattern can be useful if you have a system behind a firewall that generates status badges, or if you want to push customised status badges such as those that can be built by https://shields.io/ without requiring additional external resources to host the badge images.
