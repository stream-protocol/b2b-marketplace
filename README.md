<a href="https://streamcommerce.co">
    <img alt="Stream Commerce" src="https://i.imgur.com/3jUHsfu.png" width="100" />

# StreamPay - B2B Marketplace

A decentralized e-Commerce Platform

#### This repository is the codebase of B2B Marketplace with StreamPay´s B2B marketplace.

[Documentation](https://docs.medusajs.com/) | [Website](https://medusajs.com/) | [Repository](https://github.com/stream-protocol/b2b-marketplace.git)

##  Version

Source code uses Medusa v1.6.5. It is not guaranteed that it will work with future releases.

## Prerequisites

- [Node.js at least v14](https://docs.medusajs.com/tutorial/set-up-your-development-environment#nodejs)
- [PostgreSQL](https://docs.medusajs.com/tutorial/set-up-your-development-environment#postgresql)
- [Medusa CLI Tool](https://docs.medusajs.com/cli/reference)
- [MinIO](https://docs.medusajs.com/add-plugins/minio/#set-up-minio)

## Project Structure

This project includes three directories:

1. `b2b-admin`: The admin dashboard.
2. `b2b-server`: The  server.
3. `b2b-storefront`: The Next.js storefront.

## How to Install

### Using Medusa CLI Tool

If you're only interested in the Medusa server, you can install it using the Medusa CLI tool, or

Check out the instructions in the [B2B Server README](https://github.com/stream-protocol/b2b-marketplace/b2b-server/blob/master/README.md)

### Using GitHub Cloning

1. Clone this repository:

```bash
git clone --recurse-submodules https://github.com/stream-protocol/b2b-marketplace.git
cd b2b-marketplace
```

2\. Install the dependencies for each of the directories:

```bash
cd b2b-admin
npm install
cd ../b2b-server
npm install
cd ../b2b-storefront
npm install
```

3\. Rename the template environment variables of b2b server:

```bash
cd b2b-server
mv .env.template .env
```

And enter the necessary environment variables in the file.

4\. Rename the template environment variables of StreamPay´s b2b marketplace storefront:

```bash
cd b2b-storefront
mv .env.template .env
```

And enter the necessary environment variables in the file.

5\. Start Server:

```bash
cd b2b-server
npm start
```

You can then start the Medusa admin while the server is running with the following command:

```bash
cd b2b-admin
npm start
```

And you can then start the StreamPay storefront while the server is running with the following command:

```bash
cd b2b-storefront
npm run dev
```

## Other Resources

- [Documentation](https://docs.medusajs.com/)
