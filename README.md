# discourse-keyword-block

This theme component requires you to make three custom user fields in Admin > Customize > User Fields in order to function.  By default, the theme comoponent settings expect these user fields to be 1, 2, and 3.  If you have other custom user fields defined, you'll need to enter the correct user field numbers in the theme component settings.  See the Meta [Create and configure custom user fields guide](https://meta.discourse.org/t/create-and-configure-custom-user-fields/113192) for further details.

**1 - User's blocked terms list**

Field Type: Text Field

Field Name: (any name will work here) Blocked Terms

Field Description: (any description will work here) Block words or phrases that appear in posts or topics. Comma separated.  To block a username, include @ if whole word matching is selected.

✅ Editable after signup

❌ Required at signup

❌ Show on public profile

❌ Show on user card

❌ Searchable

**2 - Case sensitivity**

Field Type: Confirmation

Field Name: (any name will work here) Blocked terms - case sensitive

Field Description: (any description will work here) Words in the "Blocked terms" list are case sensitive.

✅ Editable after signup

❌ Required at signup

❌ Show on public profile

❌ Show on user card

❌ Searchable

**3 - Search whole or partial words**

Field Type: Confirmation

Field Name: (any name will work here) Blocked terms - whole words

Field Description: (any description will work here) Blocked terms must appear as full words, not as partial words

✅ Editable after signup

❌ Required at signup

❌ Show on public profile

❌ Show on user card

❌ Searchable

The css below is included in the theme component and will prevent any custom user fields from being displayed on the signup form.  If you have other custom user fields you do want displayed on the signup form, you'll need to override this with your own custom css.
```
.login-form .user-fields {
    display: none;
}
```
