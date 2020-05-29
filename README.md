<h3>Instructions for running your code (assuming you’re running a linux distro)</h3>
1. Run “git clone https://github.com/aggarnav/PA_Django.git” through a terminal on your PC
2. Run a terminal window in the folder with the files
3. Initialize a virtual environment 
    1. Pip install virtualenv
    2. python3 -m venv env
    3. source env/bin/activate
4. Install the requirements by running “pip install -r requirements.txt”
5. Go to the src folder by running “cd src”
6. Migrate Django files by “python manage.py migrate”
7. Run the server by “python manage.py runserver”
8. Go to http://127.0.0.1:8000/dev/accounts/login/ and signup

<h3>Known Bugs</h3>
1. Pictures in the profile section fails to load sometimes (this is probably a result of file size and image dimensions). A place holder image is used currently in case the picture upload fails
2. I was trying to implement admin functionality but had some issues with classifying users in groups and setting permissions

<h3>Functionality</h3>
1. Authentication of users. This includes the validation of passwords through options that Django offers such as a minimum password size, a mix of alphanumeric characters, and similarity checkers. Furthermore, emails are verified through the use of characters such as “@” and “.” Additional details about password validation can be seen at https://docs.djangoproject.com/en/2.2/topics/auth/passwords/#password-validation
2. Instead of loading pictures, I added a profiles tab and added them there. The profiles tab allows users to create a profile for themselves and uses several lists of professions to facilitate that process. I figured that a user profile was vital to a social media site and thus included it.
3. Users can view all posts
4. CSS has been used
5. Users can like posts. Likes are tallied
6. They can add comments which can be viewed by refreshing the page
7. Site hosted on heroku
8. Mandatory email verification wasn’t included keeping privacy in mind since it required email passwords and usernames

<h3>General Thoughts</h3>
I think the assignment was great since it catered to individuals of all skill levels. Additionally, the links and resources facilitate further reading and were a great place to start. Having never used Django before this challenge, the links were particularly helpful in introducing me to the framework. They helped me realize the value of Django as a framework and how it eases the scalability of projects while allowing for several customizations.
