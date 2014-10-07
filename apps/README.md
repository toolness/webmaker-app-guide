# Apps

### How are apps stored internally?

In Webmaker Mobile, individual **apps** created by a user is represented by a JSON blob that looks something like this:

```js
{
    id: '000d1745-5d3c-4997-ac0c-15df68bbbecz',
    name: 'Portal App',
    icon: '/images/placeholder_puppy.png',
    author: {
        name: 'Chell',
        location: 'Aperture Labs',
        avatar: 'https://aslabs.com/a/chell.png'
    },
    blocks: [
        {
            id: 'highlight',
            attributes: {
                innerHTML: {
                    label: 'Text',
                    type: 'string',
                    value: 'Which color?'
                }
            }
        },
        {
            id: 'portal',
            attributes: {
                color: {
                    label: 'Color',
                    type: 'color',
                    value: 'blue'
                }
            }
        }
    ]
}
```

The App can have a unique title, author, and list of **blocks**. Each block is a functional piece in the app that can have editable properties.

Right now when a user creates a new app, it is stored in locally (in indexDB) via [localforage](https://github.com/mozilla/localForage), but in the future apps and their related data will be synced to [makedrive](https://github.com/mozilla/makedrive) so users can access their data from anywhere.

As a developer, you can create **new blocks for users to choose from** when they build apps.


