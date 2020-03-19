- How to add conda to the PATH

    the file .bashrc (hidden file), located in the $HOME directory, runs codes every time a new terminal is opened.

    Then add a line on it: 
        export PATH=~/anaconda3/bin:$PATH


    Edit your .profile and add something like the following lines:

    if [ -d "$HOME/anaconda3/bin" ] ; then
        PATH="$HOME/anaconda3/bin:$PATH"
    fi



# https://towardsdatascience.com/getting-started-with-python-environments-using-conda-32e9f2779307
# https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html

- How to create conda virtual environment -environment.yml-:

    conda env create -f environment.yml


- How to verify that the new environment was installed correctly:
   
    conda env list


- How to delete one entire environment:

    conda remove --name your_env_name --all


- How to use an environment:

    conda activate your_env_name


- How to stop an environment:

    conda deactivate



