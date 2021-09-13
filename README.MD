                Coding convention
# Table content
* [Correctness](#correctness)
* [Format](#Format)
* [Folder structure](#Folder-structure)
* [Naming](#Naming)
* [Unused Code](#Unused-Code)
* [Comment](#Comment)
# Correctness
-   Restrict warning in code file. Expect for some special cases.
# Format 
-   Always format the code you change.
-   Don't format the entire file because it will affect the git log.
-   You can use some format tool and config depend on the project. Ex: `prettier`, `swiftlint` ...
# Folder structure 
-   Should use same folder structure in all project 
-   Folder UpperCamelCase or lowercase depend on type project.
-   Should use a word for folder
-   Some folders always have:
    -   `configs`: contain error code and server config 
    -   `enums`: contain enums 
    -   `views`: contain all screen in project
    -   `locales`: contain localize
    -   `models`: contain model data
    -   `repositories`: contain repository to call api (Repository created follow by object, ex: UserRepository, ProductRepository).
    -   `utils`: contain utils for app. If don't know using what util, you maybe create your function in Utils file.
    -   `values`: contain constant, value all app
    -   `components/widgets`: contain component/widget common use many times in app, don't add component just using in one screen.
    -   `stores/controllers`: contain bussiness flow with screen (ex: LoginController vs LoginView).
# Naming
-   Always name files and variables explicitly.
-   File
    -   Depend on rule name in a project.
    -   File name is a noun
    -   Some file name rule:
        -   Android: `UpperCamelCase` file name 
        -   iOS: `UpperCamelCase` file name
        -   Flutter: `lowercase` with _ (user_profile_view)
        -   React native: `lowerCamelCase`
    -   Put file in correct folder structure.
-   Class 
    -   Class name is a noun
    -   Name with prefix, suffix
    -   Depend on rule project. Some suffix project are `_view`, `_component`, `_widget`, `_item`.
    -   Ex: with suffix _view when it is a screen: UserProfileView 
-   Variable
    -   Variable name is a noun
    -   Using `lowerCamelCase`
    -   Should explicit variable name
    -   Shoud use right type (`Int`, `Long`, `BigDecimal` ...)
-   Method
    -   Method with prefix is verb. Ex: getUserProfile
    -   Suggest should use some prefix according to the project rule so that everyone knows the meaning of the method. Ex: `render_` prefix when render layout, `on_` prefix when action of the control, `goto_` when navigation 
    -   Using `lowerCamelCase`
# Unused Code
-   Should remove code not using or comment for a long time
-   Remove import with config auto when format or optimize import
-   Collect code in one file(maybe util) if use repeat more times.
# Comment
-   Should comment method with `///`
-   Always comment variable global in class with `//`
-   Comment code in method if code complicated.



