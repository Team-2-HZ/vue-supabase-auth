## URI: "auth/v1/signup"  POST
- Registers the user on supabase based on the form's information, and sends a confirmation email to the email address entered.
- Request example:
`{"email":"bob@testmail.com","password":"12345678","data":{"name":"Bob"}}`

## URI: "/auth/v1/verify?token="  GET
- Verifies the registration of a user on supabase. The value for the token key is sent in the email verification link.
- Request example: No payload

## URI: "auth/v1/token?grant_type=password" POST
- Logs in a user using an email and password combination.
- Request example:
`{"email":"bob@testmail.com","password":"12345678"}`

## URI: "/auth/v1/logout" POST
- Logs out a logged in user.
- Request example:
`{}`

## URI: "/auth/v1/recover" POST
- Sends a password recovery email to the email address entered.
- Request example:
`{"email":"bob@testmail.com"}`
