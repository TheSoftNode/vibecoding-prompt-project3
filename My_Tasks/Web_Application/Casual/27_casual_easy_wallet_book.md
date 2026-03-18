Category: Web_Application

Prompt style: Casual

Title: Crypto Wallet Address Book

Prompt: Wallet address book for saving crypto contacts. Type a name and paste a wallet address, click Save. List shows all saved contacts with name and shortened address (first 6 and last 4 characters with ... in middle). Click any contact to copy the full address. Delete button removes contacts.

Required libraries: react, tailwindcss, lucide-react

## Rubric

| #   | ID          | Description                                          | Weight | Rationale                                                                                    | Dependent On |
| --- | ----------- | ---------------------------------------------------- | ------ | -------------------------------------------------------------------------------------------- | ------------ |
| 1   | visual      | Display name input field                             | major  | The name input lets users label their wallet contacts.                                       | None         |
| 2   | visual      | Display address input field                          | major  | The address input lets users enter wallet addresses to save.                                 | None         |
| 3   | visual      | Display Save button                                  | major  | The Save button triggers adding the contact to the list.                                     | None         |
| 4   | interaction | Add contact to list when Save clicked                | major  | Clicking Save stores the name and address for future reference.                              | C1, C2, C3   |
| 5   | content     | Display contact name in list                         | major  | Showing names helps users identify their saved contacts.                                     | None         |
| 6   | state       | Shorten address to first 6 and last 4 characters     | major  | Shortening addresses makes the list readable while keeping unique identifiers visible.       | None         |
| 7   | content     | Display shortened address with ... in middle         | major  | The ellipsis format shows this is a shortened version of the full address.                   | C6           |
| 8   | interaction | Copy full address when contact is clicked            | major  | Clicking a contact copies the complete address for use in transactions.                      | None         |
| 9   | visual      | Display delete button for each contact               | major  | Delete buttons give users control to remove outdated contacts.                               | None         |
| 10  | interaction | Remove contact from list when delete clicked         | major  | Deleting removes the contact and cleans up the address book.                                 | C9           |

## Justification

The crypto wallet address book works exactly as expected for managing contact addresses. A name input field and an address input field display with a Save button. When users type a name, paste a wallet address, and click Save, the contact is added to the list. The list shows all saved contacts displaying the contact name and a shortened version of the address showing the first 6 and last 4 characters with ... in the middle. When users click any contact, the full address is copied to the clipboard. Each contact has a delete button that removes the contact from the list when clicked.
