# Configuring Roles and Permissions for a Service Provider

WSO2 Identity Server (WSO2 IS) allows you to configure and manage roles
as well as permission for a service provider.

When you create a service provider via WSO2 IS, a corresponding
application role is created by default within WSO2 IS. For example, if
you create a service provider named SP1, a corresponding application
role is created for SP1 within WSO2 IS, and that application role is
assigned to the user who created the service provider. Therefore, only
the user who creates a service provider can view or manage the service
provider. If you want to allow any other user to be able to view or
manage a service provider, the user has to be assigned the application
role corresponding to the particular service provider.

!!! tip
    
    **Application Role** : A special case of internal role that is created
    for a particular service provider application. Only users who are
    assigned the application role permission can manage the corresponding
    service provider application.
    

Now, let's create a service provider, and then configure roles and
permission for the created service provider.

Next, follow the steps below to configure roles and define custom
permission for the service provider:

1.  In the service provider that you created, expand the
    **Role/Permission Configuration** section, and then expand the
    **Permissions** as well as the **Role Mapping** sections.  
    ![]( ../../assets/img/103329771/103329772.png) 
2.  Click **Add Permission** and specify the service provider specific
    permission that you want to add.

    -   If you want to add another permission entry, click **Add
        Permission** again.
    -   If you want to delete an entry, click **Delete**.

    Once you add/update service provider specific permission details,
    the permission details will be listed as available permission when
    [adding
    roles](Configuring-Roles-and-Permissions_103330369.html#ConfiguringRolesandPermissions-addU)
    via WSO2 IS.

3.  Click **Add Role Mapping** and enter appropriate values for the
    **Local Role** as well as the **Service Provider Role**.

    -   If you want to add another role mapping entry, click **Add Role
        Mapping** again.
    -   If you want to delete a role mapping entry, click **Delete**.

    !!! tip
    
        When you add role mapping, you can map an exact role name available
        in WSO2 IS to a particular service provider role.
    

Now that you have configured roles and permission for the service
provider, you can go ahead and assign the application role permission to
any user who should be able to view and manage the service provider. For
information on how to assign roles to a user, see [Configuring
Users](_Configuring_Users_).