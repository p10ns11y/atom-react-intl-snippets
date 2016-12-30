## React Intl Snippets
Provides basic snippets for `react-intl`

## Commands
- `rif` => `import { FormattedMessage } from 'react-intl';`
- `riin` => `import { injectIntl, intlShape } from 'react-intl';`
- `ridm` =>
   ```
   import { defineMessages } from 'react-intl';

   export default defineMessages({
     componentKey: {
       id: '${1:project.pages.components.prefix}',
       defaultMessage: '',
     },
     componentKey: {
       id: '${1:project.pages.components.prefix}',
       defaultMessage: '',
     },
     componentKey: {
       id: '${1:project.pages.components.prefix}',
       defaultMessage: '',
     },
     componentKey: {
       id: '${1:project.pages.components.prefix}',
       defaultMessage: '',
     },
     componentKey: {
       id: '${1:project.pages.components.prefix}',
       defaultMessage: '',
     },
   });
   ```

   Where `${1:project.pages.components.prefix}` could be used as component's common
  `id` prefix
