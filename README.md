# User Profile Form
 
A Java Swing desktop app built in NetBeans. The user fills in their profile details, optionally attaches a photo, and submits. Input is validated and a confirmation dialog shows the result.

## Structure
 
```
src/
├── model/User.java        Data class for the profile fields
└── ui/UserJFrame.java     Main window, validation, entry point
    ui/UserJFrame.form     NetBeans Form Editor layout
```

## Validation
 
Checked on submit in order. The first failure shows an error dialog and focuses the offending field:
 
- First and last name required, letters plus spaces, apostrophes and hyphens only (max 50)
- Age between 1 and 120
- Email must be a valid address
- Gender must be selected
- Phone must match `123-456-7890`
- Continent must be selected
Hobbies and photo are optional.
