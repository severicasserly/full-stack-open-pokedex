# A dive into python CI pipelines

Python programs do not need to be built but packages like external libraries do need to be installed. It is usually done with Pythons package manager pip. Python virtual environments help isolate project specific libraries or scripts among other things. Bundling and isolation is also commonly achieved with dockerization.

Python has a few conventions for styling code. Style checks or linting can be done with for example with pylint, flake8 or Black.
Similarly there are many choises for testing libraries django even has its own.

The little experience I have with setting up CI is with gitlab which is very similar to github actions. Azure, AWS and GCP also have their own more integrated tools for CI.

Most likely a cloud based environment is more simple if the code is already hosted on some online platform unless there is need for something specific. Even then for example with Gitlab it is very easy to have parts of the CI pipeline run on your own hosted machine. Self hosting can become quite complex and cumbersome to maintain if it's not thought out properly. On the other hand it gives more control over customization and independence from the service providers.
