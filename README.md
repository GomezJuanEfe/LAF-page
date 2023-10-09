# LAF-page

Final individual project that is part of the Make it Real Bootcamp.

![LAF-mockup](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExaW5zNnJ3dm9pcTZ4dWc0NnZ3b3hqenB0YXFxb2MwdHQxcWtwOGcwZCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/bZEhAOUGwPRkBKoNN5/giphy-downsized-large.gif)

## Overview ✍️

The project is a institutional website designed for the Liga Antioqueña de Futbol (LAF). It leverages Strapi as the content management system (CMS) for efficient content administration, and NextJS serves as the frontend framework. This setup empowers the administrator to easily add and manage content within the application through the CMS, while providing a seamless user experience for visitors who can consume the website's content effortlessly.

## Installation ⚙️

To get started with the project, follow these steps:

### 1. Clone the repository:

```shell
git clone git@github.com:GomezJuanEfe/LAF-page.git
```

### 2. Initialize and update the submodules:

```shell
git submodule init
git submodule update
```

### 3. Install the dependencies of the API:

```shell
cd api/
npm install
```

### 4. Set the env variables of the API:

See the example on ./api/.evn.example

### 5. Start Strapi application

```shell
npm run develop
```

You'll be redirected to the Strapi interface. Then, you have to provide a basic information in order to set Strapi up.

### 6. Set permissions for unauthenticated users

Once on the Strapi dashboard go to: settings / Roles (USERS & PERMISSIONS PLUGIN)
On Permissions section drop down each of the next tabs and check "find" and "findOne":

- Categoria
- Noticia
- Page

### 7. Seed data

On terminal run de the next comand

```shell
npm run strapi import -- -f seed-data.tar.gz.enc
```

Decryption key: laf

### 8. Install the dependencies of the Client:

```shell
cd client/
npm install
```

### 9. Set the env variables of the Client:

See the example on ./api/.evn.example

### 10. Start NextJS Application

```shell
npm run dev
```

🎉 The application will be ready for exploration.

## The Challenge 🏋️‍♂️

### 1. Understanding CMS Structure and Configuration:

Configuring and understanding the intricacies of Strapi as the content management system (CMS) can be a significant challenge. This includes defining content models, setting up permissions, and ensuring that the CMS aligns with the specific needs of the Liga Antioqueña de Futbol (LAF) website. Effective content management is crucial for the site's success.

### 2. GraphQL Query Structure:

Working with GraphQL to query data from the backend can be a challenge, especially if you are new to GraphQL. You'll need to understand the structure of GraphQL queries, including how to request the right data efficiently. Properly structuring queries is essential for optimizing the performance of the application.

### 3. Markdown to Frontend Rendering:

Converting Markdown content from the backend into a visually appealing format on the frontend can be a complex task. You'll need to implement a rendering mechanism that processes Markdown and displays it correctly while maintaining consistency and readability throughout the website.

### 4. Leveraging NextJS Benefits:

NextJS offers various advantages for building web applications, such as server-side rendering, routing, and optimized performance. Maximizing these benefits requires a deep understanding of NextJS's structure and capabilities. Ensuring that the application leverages NextJS to its fullest potential can be both challenging and rewarding.

These challenges highlight the technical complexities and considerations involved in developing the Liga Antioqueña de Futbol (LAF) website. Overcoming these challenges will lead to a robust and user-friendly web platform for both administrators and users alike.

## My Process ⛰️

### Built With 🛠️

The project was built using the following technologies:

- NextJS
- Strapi CMS
- GraphQL

### What I Learned 🔬

During this project, I learned how to:

- Gained Proficiency in Strapi CMS Configuration.
- Mastered GraphQL Query Structuring for Data Retrieval.
- Developed Markdown-to-HTML Rendering Skills. For this I used SnarkDown library by Jason Miller
- Acquired In-Depth Understanding of NextJS for Optimal Utilization.

## Useful Resources 🆘

During the development of this project, the following resources were helpful:

- Official NextJS documentation: https://nextjs.org/docs
- SnarkDown library: https://github.com/developit/snarkdown/blob/main/src/index.js
- Importing, Exporting and Transferring Data with the Strapi CLI: https://strapi.io/blog/importing-exporting-and-transferring-data-with-the-strapi-cli
- Como hacer un CMS personalizado con NEXT.JS 13 y STRAPI DESDE CERO by MiduDev: https://www.youtube.com/watch?v=dEiNb_YvXSY

## Author ✒️

Juan Felipe Gómez Ramírez - Developer - https://gomezjuanefe.com/

## Acknowledgements 🎁

I extend my gratitude to the Make it Real team for supplying the essential tools and invaluable assistance that facilitated the creation of this project.
