---
id: Empty state
section: components
has_children: true
nav_order: 2
has_toc: true
---

import { EmptyState, EmptyStateVariant, EmptyStateIcon, EmptyStateBody, Title, Button, TitleSizes, ButtonVariant } from '@patternfly/react-core';
import SpaceShuttleIcon from '@patternfly/react-icons/dist/js/icons/space-shuttle-icon';

### Empty state

Description about the Empty State can go here..

```js
emptyState = () => {

  const variant = EmptyStateVariant.large;
  const title = 'Empty State title';
  const titleSize = TitleSizes.xl;
  const headingLevel: 'h2';
  const body = 'Empty state body';
  const buttonTitle = 'Action';
  const buttonVariant = ButtonVariant.primary

  return (
    <EmptyState variant={variant}>
      <EmptyStateIcon icon={SpaceShuttleIcon} />
      <Title headingLevel={headingLevel} size={titleSize}>
        {title}
      </Title>
      <EmptyStateBody>{body}</EmptyStateBody>
      <Button variant={buttonVariant}>
        {buttonTitle}
      </Button>
    </EmptyState>
  )
}
```