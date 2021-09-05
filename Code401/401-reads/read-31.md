## Persmissions

    permissions determine whether a request should be granted or denied access. Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

## Object Level Permissions 

    REST framework permissions also support object-level permissioning. Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

## Setting the permission policy

    ```
    REST_FRAMEWORK = {
        'DEFAULT_PERMISSION_CLASSES': [
            'rest_framework.permissions.IsAuthenticated',
        ]
    }
    ```

## API Reference

    -   IsAuthenticated: The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise.

    -   IsAdminUser: The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.

    -   IsAuthenticatedOrReadOnly: The IsAuthenticatedOrReadOnly will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

    



