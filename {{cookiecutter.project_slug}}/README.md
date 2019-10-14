# {{cookiecutter.project_name}}
{{cookiecutter.project_short_description}}

- Every calculation step is a single run file
- Every calculation has a name, and files of the type Filename.$name.shin
  are bash templates that should render the file Filename.$name, which should
  make Filename, i.e.

            /*****************************************************/
            /* Filename.$name.shin => Filename.$name => Filename */
            /*                     ^                 ^           */
            /*                     |                 |           */
            /*                     l-- bash          l-- cp      */
            /*****************************************************/
- Every run.name script should be called from run, which is the script to be
  submitted.
