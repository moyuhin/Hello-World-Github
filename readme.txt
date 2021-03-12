name: Greeting from Mo Yu Hin
on: [push, pull_request]

jobs:
  my-job:
    name: My Job
    runs-on: ubuntu-latest
    steps:
    - name: Print a greeting
      env:
        MY_VAR: Hi there! My name is
        FIRST_NAME: Yu Hin
        MIDDLE_NAME: Max
        LAST_NAME: Mo
      run: |
        echo $MY_VAR $FIRST_NAME $MIDDLE_NAME $LAST_NAME.
