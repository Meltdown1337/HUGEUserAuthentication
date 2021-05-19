# HUGEUserAuthentication
Simple user-authentication solution, embedded into a small framework.

# HUGE

Just a simple user authentication solution inside a super-simple framework skeleton that works out-of-the-box (and comes with an auto-installer), using the future-proof official bcrypt password hashing/salting implementation of PHP 5.5+, plus some nice features that will speed up the time from idea to first usable prototype application dramatically. Nothing more. This project has its focus on hardcore simplicity. Everything is as simple as possible, made for smaller projects, typical agency work and quick drafts. If you want to build massive corporate applications with all the features modern frameworks have, then have a look at Laravel, Symfony or Yii, but if you just want to quickly create something that just works, then this script might be interesting for you.

HUGE's simple-as-possible architecture was inspired by several conference talks, slides and articles about huge applications that - surprisingly and intentionally - go back to the basics of programming, using procedural programming, static classes, extremely simple constructs, not-totally-DRY code etc. while keeping the code extremely readable (StackOverflow, Wikipedia, SoundCloud).

Some interesting Buzzwords in this context: KISS, YAGNI, Feature Creep, Minimum viable product.

### HUGE has reached "soft End Of Life"

To keep this project stable, secure, clean and minimal I've decided to reduce the development of HUGE to a minimum. Don't worry, this is actually a good thing: New features usually mean new bugs, lots of testing, fixes, incompatibilities, and for some people even hardcore update stress. As HUGE is a security-critical script new features are not as important as a stable and secure core, this is why people use it. This means:

HUGE will not get new features
but will be maintained, so it will get bugfixes, corrections etc for sure, maybe for years

And to be honest, maintaining a framework for free in my rare free-time is also not what I want to do permanently. :)

Finally a little note: The PHP world has evolved dramatically, we have excellent frameworks with awesome features and big professional teams behind, very well written documentations and large communities, so there's simply no reason to put much work into another framework. Instead, please commit to the popular frameworks, then your work will have much more impact and is used by much more people!

### Releases & Developpement

stable v3.1,

public beta branch: master

public in-development branch (please commit new code here): develop

# Features

built with the official PHP password hashing functions, fitting the most modern password hashing/salting web standards

proper security features, like CSRF blocking (via form tokens), encryption of cookie contents etc.

users can register, login, logout (with username, email, password)

password-forget / reset

remember-me (login via cookie)

account verification via mail

captcha

failed-login-throttling

user profiles

account upgrade / downgrade

simple user types (type 1, type 2, admin)

supports local avatars and remote Gravatars

supports native mail and SMTP sending (via PHPMailer and other tools)

uses PDO for database access for sure, has nice DatabaseFactory (in case your project goes big)

uses URL rewriting ("beautiful URLs")

proper split of application and public files (requests only go into /public)

uses Composer to load external dependencies (PHPMailer, Captcha-Generator, etc.) for sure

fits PSR-0/1/2/4 coding guidelines

uses Post-Redirect-Get pattern for nice application flow

masses of comments

is actively maintained and bug-fixed (however, no big new features as project slowly reaches End of Life)
