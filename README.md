# breadcrumbs-ts

A dynamic React component for adding customizable breadcrumbs in your project. Built using **React.js**, **TypeScript**, and **Storybook**.

![React](https://img.shields.io/badge/-ReactJs-61DAFB?logo=react&logoColor=white&style=flat)
![TypeScript](https://img.shields.io/badge/-TypeScript-007ACC?logo=typescript&logoColor=white&style=flat)
![Storybook](https://img.shields.io/badge/-Storybook-FF4785?logo=storybook&logoColor=white&style=flat)
![](https://img.shields.io/badge/npm-v10.8.2-green)
![](https://img.shields.io/badge/license-MIT-orange)
![](https://img.shields.io/badge/downloads-85/month-yellow)

<br>

## Features

- **Custom Home Route**: Easily set your home route to any desired path.
- **Custom Styles**: Apply unique styles to the home route, individual routes, and the active route.
- **Breadcrumb Capitalization**: Option to capitalize breadcrumb labels.
- **Limit Breadcrumbs**: Set a maximum number of breadcrumbs to display.
- **Fully Dynamic**: Dynamically generates breadcrumbs based on your route structure.

<br>

## Installation

You can install the package via npm or yarn:

```bash
npm install breadcrumbs-ts
# or
yarn add breadcrumbs-ts
```

<br>
<br>

Here's a basic example of how to integrate the `breadcrumbs-ts` component into your project:


```bash
import Breadcrumbs from 'breadcrumbs-ts';

const ExamplePage = () => {
  return (
    <Breadcrumbs
      homeElement="Home"
      separator="/"
      activeClasses="text-indigo-500"
      containerClasses="grid py-5 px-10 text-gray-400 gap-1 text-sm"
      listItemClasses="c-hover c-margin c-font-weight c-text"
      capitalizeLinks
    />
  );
};

export default ExamplePage;
```

<br>
<br>

# Storybook Demo

You can view a live demo of the component in Storybook:

[Storybook Demo](https://66db2dca6d0e43849a2d390e-adngsrjzvm.chromatic.com/?path=/docs/components-breadcrumbs--docs)

<br>
<br>

| Prop Name        | Type    | Description                                                                             | Default  |
| ---------------- | ------- | --------------------------------------------------------------------------------------- | -------- |
| homeElement      | string  | Custom element for the home route (text or component).                                  | `'Home'` |
| separator        | string  | Custom separator between breadcrumbs.                                                   | `'/' `   |
| activeClasses    | string  | CSS classes to apply to the active breadcrumb.                                          | `''`     |
| containerClasses | string  | CSS classes for the breadcrumb container.                                               | `''`     |
| listItemClasses  | string  | CSS classes for individual breadcrumb items.                                            | `'' `    |
| capitalizeLinks  | boolean | Capitalizes each breadcrumb label.                                                      | `false`  |
| maxVisibleItems  | number  | Sets the maximum number of breadcrumbs to display. Remaining breadcrumbs are collapsed. | `5`      |

<br>
<br>

# Customization

You can customize the following parts of the breadcrumbs:

**Home Element**: Replace the default home route label with custom text or a React component.

**Separator**: Define a custom separator between breadcrumb items.

**Style Customization**: Apply custom CSS classes to the container, breadcrumb items, and the active breadcrumb.

**Capitalize Links**: Enable automatic capitalization of breadcrumb labels.

<br>
<br>

# License

This project is licensed under the MIT License.

<br>
<br>

This version reflects the correct usage of the `Breadcrumbs` component, including props like `homeElement`, `separator`, `activeClasses`, `containerClasses`, `listItemClasses` and `maxVisibleItems`.
