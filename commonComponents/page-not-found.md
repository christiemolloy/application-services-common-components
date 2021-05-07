---
id: Page not found
section: components
has_children: true
nav_order: 2
has_toc: true
---

import { PageSection, EmptyState, EmptyStateVariant, EmptyStateIcon, EmptyStateBody, Title, Button, TitleSizes, ButtonVariant } from '@patternfly/react-core';
import SearchIcon from '@patternfly/react-icons/dist/js/icons/search-icon';

### Page Not Found

Description about the Page not found can go here..

```js
pageNotFound = () => {

  const variant = EmptyStateVariant.large;
  const title = 'This page does not exist';
  const titleSize = TitleSizes.xl;
  const headingLevel: 'h2';
  const body = 'We cannot find the page you are looking for.';
  const buttonTitle = 'Return to homepage';
  const buttonVariant = ButtonVariant.primary

  return (
    <PageSection padding={{ default: 'noPadding' }} isFilled>
        <EmptyState variant={variant}>
          <EmptyStateIcon icon={SearchIcon} />
          <Title headingLevel={headingLevel} size={titleSize}>
            {title}
          </Title>
          <EmptyStateBody>{body}</EmptyStateBody>
          <Button variant={buttonVariant}>
            {buttonTitle}
          </Button>
        </EmptyState>
    </PageSection>
  );
};
```