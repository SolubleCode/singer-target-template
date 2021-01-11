# singer-target-template
A [cookiecutter](https://github.com/audreyr/cookiecutter) template for creating
[Singer](https://github.com/singer-io) targets.

The best way to demonstrate creating your target structure is with an example.
Below I will initialize the "target-foobar" project:

Start by installing cookiecutter:
```bash
$ pip install cookiecutter
```

The next command will ask for some input.  Enter the name of your tap:
```bash
$ cookiecutter https://github.com/solublecode/singer-target-template.git
project_name [e.g. 'target-csv']: target-foobar
```

Now that the project exists, make a virtual environment:
```bash
$ cd target-foobar
$ python -m venv venv
$ source ./venv/bin/activate
```
Install the package:
```bash
$ pip install -e .
```
See the [Running a Singer Tap with a Singer Target](https://github.com/singer-io/getting-started/blob/master/docs/RUNNING_AND_DEVELOPING.md#running-a-singer-tap-with-a-singer-target) section of the singer docs for instructions on running a Tap with your Target
