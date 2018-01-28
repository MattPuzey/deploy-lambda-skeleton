# Skeleton

## Setting up your GET method

- Replace occurrences of `skeleton` in `.circleci/config.yml` with the new repo name

- Replace all occurrences of `skeleton-get` with an appropriate name

- Replace all occurrences of `skeleton` with your resource name under the`./vars` directory

- Push changes to git

- Add project in CircleCI

- Add environment variables and AWS credentials to circleCI project

## Adding a new method

- Copy the `skeleton-get` directory and rename to the method you want to add

- Change the default value of the `lambda_name` variable in `./{method}/infrastructure/variables.tf`

- Copy unittest_get and build_get in `.circleci/config.yml`


## Adding a new alias

- Copy `./aliases/tf-state-get.tf` and rename to `tf-state-{method}.tf`

- Adjust the `key` variable within `./aliases/tf-state-{method}.tf`

- Add a new alias in `aliases.tf`

- Add a new lambda permission in `permissions.tf`, be sure to update the method i.e. `/*/GET` included in the source arn.
