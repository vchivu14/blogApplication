=====
Users
=====

Users is a Django app to create profiles and provide login.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "users" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'users',
    ]

2. Read the settings.txt, there are two paragraphs which need to be added to
    your project settings file.
    - The Fist commented out string needs to be attached (without the quotes)
        at the bottom of your settings.py file;
    - The Second commented out string is your urls file for your project,
        add those urls, along with others you may have and make changes
        if path names collide.

3. Create your config.json file with credentials so you can use mail retrieval.
    (the project has a default location from where it loads the file
    "/etc/config.json", like it's stated in the settings file,
    but you need to create it one on your computer and add the credentials required
    in key pairs values like {'EMAIL_USER':"your email", 'EMAIL_PASS':"your passwd"}).

3. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a profile (you'll need the Admin app enabled).
