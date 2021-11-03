# 100 days of code, day 20

## Tailwind CSS with Next.js

Tailwind is a utility first CSS framework that simplifies css to build any design, directly in your markup.

Today we will learn how to use it with Next.js (a React.js framework)

_Creating a new project in your terminal/cmd_
```bash
npx create-next-app -e with-tailwindcss my-project
# then
cd my-project
```
More examples [Here](https://tailwindcss.com/docs/guides/nextjs)

In `pages/index.js` the following code will produce this respectively

```jsx
export default function Home() {
  return (
    <div>
      <header className="flex w-full p-5 justify-between">
        <div className="flex space-x-4 items-center">
          <p>About</p>
          <p>Store</p>
        </div>
        <div className="flex space-x-4 items-center">
          <p>Gmail</p>
          <p>Images</p>
        </div>
      </header>
    </div>
  );
}
```
