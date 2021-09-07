## Managing Django Settings: Issues

    -   Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc).

    -   Sensitive data. You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

    -   Sharing settings between team members. You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings.

    -   Django settings are a Python code. This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.


## Setting Configuration: Different Approaches

    1-  settings_local.py
            pros: Secrets not in VCS.
            cons: settings_local.py is not in VCS, so you can lose some of your Django environment settings.

    2-  Separate settings file for each environment
            pros: It’s easy to share settings between developers.
            cons: You need to find a way to handle secret passwords and tokens.

    3-  Environment variables
            pros: Configuration is separated from code.
            cons: You need to handle sharing default config between developers.

## Django Settings: Best practices

    -   Keep settings in environment variables.
    -   Write default values for production configuration (excluding secret keys and tokens).
    -   Don’t hardcode sensitive settings, and don’t put them in VCS.
    -   Split settings into groups: Django, third-party, project.
    -   Follow naming conventions for custom (project) settings.


## What is SSH 

    SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet. 

## How Does SSH Work
    If you’re using Linux or Mac, then using SSH is very simple. If you use Windows, you will need to utilize an SSH client to open SSH connections. The most popular SSH client is PuTTY. For Mac and Linux users, head over to your terminal program and then follow the procedure below:

    The SSH command consists of 3 distinct parts:
    ```
    ssh {user}@{host}
    ```