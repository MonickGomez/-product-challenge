<p align="center">
    <a href="https://croct.com">
      <img src="https://cdn.croct.io/brand/logo/repo-icon-green.svg" alt="Croct" height="80"/>
    </a>
    <br />
    <strong>Feature Specification</strong>
    <br />
    Technical specification for the sign-in and sign-up features.
</p>

# Challenge

As a Product Manager that just joined the team, one of your tasks is to write the user stories that will guide the development team in building the product.

The design team and the product manager collaborated to create the wireframes that you'll use as a base to write the user stories. Your task is to describe all possible scenarios involving the sign-in and sign-up pages. For each interaction, you need to write a scenario that tells the user's story and how the interface should behave.

To better understand the screens you should describe, you can revisit the conversation between the designer and the product manager who created the wireframes.

## Below you can see a scenario that tells the user's story and how the interface should behave.



- Precondition: Have an account on the system

- Access the login page
- fill in credentials
- Click the login button
-Wait for login to complete


@Login

> feature: login

> a croct system user

> john wants to login

>to have access to logged in user functionalities

@positive

> **scenario: valid login**

> Since “John” has an account on the system

>And he accesses the login page!

>And it fills in your valid credentials

>When it triggers the login option

>Then he should be redirected to the home page logged in

@negative
> **Scenario: Login with Incorrect Password**

>Since “John” has an account on the system

>And he accesses the login page

>And it fills in your valid credentials

>When it triggers the login option

>Then he should be redirected to the home page logged in


@positive

> **Scenario: after incorrect password warning**

>Since “John ” has an account on the system

>And fill in the password credentials with the correct password

>When it triggers the login option

>Then he should be redirected to the home page logged in

@negative 

>**Scenario: invalid user**

>Since “John ” has an account on the system
 
>And fill in the credentials with incorrect user

>When it triggers the login option!

>Then it should show an incorrect user warning!

@positive!

>**Scenario: after incorrect user notice**

>Since “John ” has an account on the system

>And fill in the credentials with correct username and password

>When it triggers the login option

>Then he should be redirected to the home page logged 

@negative 

>**Scenario: reset password**
>Since “John ” has an account on the system

>And don't remember your password and click on reset password

>When it triggers the reset password option 

>Then he should be redirected to the password reset page!


@positive

>**Scenario: Login with new password**

>Since “John ” has an account on the system

>And he accesses the login page after resetting the password

>And it fills in your new valid credential

>When it triggers the login option

>Then he should be redirected to the home page logged in!




>**Registration screen** 

>Precondition: Not having an account on the system

>Access the create account page

>Fill in credentials

>Click on the create account button

>Wait for the account to be created!


 
>**@Create an account**

>Functionality: Create account

>The user does not have an account on the system yet

>Ana wants to create an account

>to have access to the functionality of logged in user


>**@positive**

>Scenario: Create account with valid credentials 

 >Since “Ana” does not have an account on the system

>And she accesses the create account page

>And it fills in your valid credentials (first name, second name, email and strong password it must be at least 8 characters long, contain upper and lower case letters and have at least one number or symbol.

>When she activates the option to create account

>Then she should be redirected to the login screen


>**@negative**

  > scenario: Create account with invalid credentials

  > Since “Ana” does not have an account in the system

>And she accesses the create account page

>And she fills in your credentials, but your email is not valid

>When it triggers the option to create account

>Then she should see a message stating that the email is invalid!


>**@negative**

>Scenario: Create account with invalid credentials 

  > Since “Ana” does not have an account on the system

>And she accesses the create account page

>And she fills in your valid credentials

>And she put a weak password

>When it triggers the option to create account

>Then she should see a message stating that her password is weak and that it must be at least 8 characters long, contain upper and lower case letters and have at least one number or symbol.

>**@positive**     
> Scenario: Create account with valid credentials

> Since “Ana” does not have an account on the system

>And she accesses the create account page

>And she fills in your credentials with correct email and strong password

 > When it triggers the option to create account

>Then he should be redirected to the login screen
 



>**@positive**

  >Scenario: Create account with valid credentials 

  > Since “Ana” does not have an account on the system

>And she accesses the create account page

>And she fills in her credentials with a strong password on the second try.

  >When it triggers the option to create account

>Then he should be redirected to the login screen!


>**@negative**
>Scenario: reset password !

>Since “ana” has just created an account in the system

>And don't remember your password and click on reset password

>When it triggers the reset password option 

>Then he should be redirected to the password reset page
 
>**@positive**

>Scenario: Login with new password

>Since “ana ” has an account on the system

>And she accesses the login page after resetting the password

>And she fills in your new valid credentials

>When it triggers the login option

>Then he should be redirected to the home page logged in




