#[MAKING DJANGO REALLY, REALLY, RIDICULOUSLY SECURE](http://2015.djangocon.us/schedule/presentation/54/)
by @_K_E_L_S_E_Y

Works on [Callisto](https://demo.callistocampus.org/), which is information escrow for sexual assault survivors, focused on college campuses.

##You can't secure the data on the internet
However...

##You CAN secure data on the internet

##You get a LOT for free w/ Django
-  passwords are "cryptographically agile"
    +  I need to learn more about that
-  set your secret key correctly
-  django-secure
-  Threat Modeling
    +  You need to know your data model and data flow very well before you can do this (System Modeling)
        *  You should do this ANYWAY as you're building your system
    +  A SPECIFIC person may be ultra-motivated to seek a SPECIFIC report
    +  On college campuses, there are LOTS of shared computers
    +  Callisto may be subpoenaed at some point
        *  their data is encrypted w/ a key stored by the USER, but not on the Callisto system. Callisto ONLY stores the encrypted data.

##Biggest threat is IN this room OR someone you know
-  The story of Allcrypt
    +  A Bitcoin exchange that shut down earlier this year.
    +  The had a private technical contractor running an email server on their machine. That's how they did their email. IT got taken over by a malicious party. THAT led to ~40 bitcoins being stolen via a password reset email sent TO that contractor.
-  Lockdown your Django admin
    +  Django Admin Honeypot
    +  DON'T use admin in Production
    +  or IP limit it

##2nd Biggest threat: people you're trying to protect
-  Good UX helps
-  Password strength meters
    +  Password strength & password design is a DEEP topic, worthy of study if you have people log in to your site
    +  Some give an estimate of how long it would take to crack your password
    +  [zxcvbn: realistic password strength estimation](https://blogs.dropbox.com/tech/2012/04/zxcvbn-realistic-password-strength-estimation/)
-  Rate limiting
    +  django rate limiter
-  Two factor auth

##Boundaries are hard
-  Your app vs. NOT your app
    +  Getting Callisto reports into the hands of university admins. This means TEACHING them how to deal with crypto

##Don't get cute
-  No new crypto
-  the simpler your security is, the easier it is for people to TRUST it

##Pay someone smarter than you
-  Heroku hosting
