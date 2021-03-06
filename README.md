

## Plugin for frontend-app-account
This is a micro-frontend application responsible for the display and updating of a user's account information.


#### Cloning and configuring Frontend-app-account

`$ git clone -b murat https://github.com/NTNUbeta/frontend-app-account `

Than edit
`https://github.com/NTNUbeta/frontend-app-account/blob/murat/.env.development` file with your environment values, push back to GitHub.


### Installation:

If using virtualenv:

`$ python3 -m venv ~/tutor`

`$ source ~/tutor/bin/activate`

 Cloning and installing plugin

`$ https://github.com/NTNUbeta/tutor-account `

`$ pip3 install -e tutor-account`

`$ tutor plugins list`

`$ tutor plugins enable account`

Building new Docker services for Tutor

`$ tutor images build account`

`$ tutor local quickstart `

visit http://yourdomain.com:1997

![](src/account.png)


### Features and functionality

To change account informations such as Username, Full Name, Email, Password reset, Birthday, Country.

To change Profile informations: Education, Gender, Spoken Languages

Add or change social media links: LinkedIn, Facebook, Twitter

Site Prefences: to change Site language, Time zone

Linked Accounts: to link your other accounts

Delete Account
