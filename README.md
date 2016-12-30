## React Intl Snippets
Provides essential snippets for `react-intl`

## Commands
- `rip` =>
    ```
    <IntlProvider locale={} messages={}>
      APP
    </IntlProvider>
    ```

- `rial` =>
    ```
    import {addLocaleData} from 'react-intl';
    import |LocaleData from 'react-intl/locale-data/[sv]';

    addLocaleData(LocaleData);
    ```
- `rild` =>`import |LocaleData from 'react-intl/locale-data/[sv]';`

- `rif` => `import { FormattedMessage } from 'react-intl';`

- `rinj` => `import { injectIntl, intlShape } from 'react-intl';`

- `ridm` =>
    ```
    import { defineMessages } from 'react-intl';

    export default defineMessages({
      descriptor: {
        id: '',
        defaultMessage: '',
      },
      ...more
    });
    ```
- `rifm` =>
    ```
    <FormattedMessage
      id='requiredProp'
      description='optionalProp'
      defaultMessage='requiredProp'
      values={{
        key:'value'
      }}
    />
    ```

- `rifmt` =>
    ```
    <FormattedMessage
      tagName=""
      id='requiredProp'
      description='optionalProp'
      defaultMessage='requiredProp'
      values={{
        key:'value'
      }}
    />
    ```

- `rifmdm` => `<FormattedMessage {...descriptor} />`

- `rifmdmt` => `<FormattedMessage tagName="" {...descriptor} />`

- `rifmcb` =>
    ```
    <FormattedMessage {...descriptor} >
      {
        formattedMessage => (
          <[reactElementOrTagName]>
            {formattedMessage}
          </|>
        )
      }
    </FormattedMessage>
    ```

- `rinjrc` =>
    ```
    import React, { PropTypes } from 'react';
    import { injectIntl, intlShape } from 'react-intl';

    class [intlInjectComponent] extends React.Component {
      /* Life cycle methods */

      render() {
        const { intl } = this.props;

        return (
          <div>
            {intl.formatMessage({id:'', defaultMessage: ''})}
            {intl.formatMessage(descriptor)}
          </div>
        );
      }
    }

    |.propTypes = {
      intl: intlShape.isRequired,
    }

    export default injectIntl(|);
    ```
## Pro Tip:

- `ri` (react-intl) root prefix and all shortcuts begins with it
  - `fm`: FormattedMessage (`rifm`)
    - `dm`: for defaultMessages (`rifmdm`)
      - `t` : with `tagName` prop (`rifmdmt`)
    - `t`: with `tagName` prop (`rifmt`)
  - `nj`: injectIntl import (`rinj`)
    - `rc`: injectIntl wrapped React.Component (`rinjrc`)
