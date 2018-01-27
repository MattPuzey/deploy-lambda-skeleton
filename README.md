# Skeleton

## Setting up your GET method

- Replace `skeleton` in `.circleci/config.yml` with the new repo name

- Replace all occurrences of `skeleton-get` with an appropriate name

- Replace all occurrences of `rename_me` with your resource name

## Adding a new method

- Copy `./api-endpoints/tf-state-get.tf` and rename to `tf-state-{method}.tf`

- Adjust the `key` variable within `./api-endpoints/tf-state-{method}.tf`

- Copy the `skeleton-get` directory and rename to the method you want to add

- Change the default value of the `lambda_name` variable in `./{method}/infrastructure/variables.tf`


- Copy unittest_get and build_get in `.circleci/config.yml`
