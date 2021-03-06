<div>
	<p align="center">
		<a href="https://vercel.com">
			<img src="https://images.iwantmyname.com/apps/logo_vercel.png" height="250px" />
		</a>
	</p>
	<p align="center">
		<a href="https://twitter.com/thewizardlink">
			<img src="https://img.shields.io/twitter/follow/thewizardlink.svg?style=social&logo=twitter">
		</a>
		<a href="https://github.com/wizardlink/interview_companyhero/issues">
			<img src="https://img.shields.io/github/issues/wizardlink/interview_companyhero.svg?style=flat-square">
		</a>
		<a href="https://github.com/wizardlink/interview_companyhero/graphs/contributors">
			<img src="https://img.shields.io/github/contributors/wizardlink/interview_companyhero.svg?style=flat-square">
		</a>
	</p>
</div>

## interview_companyhero

Repository responsible for showcasing the test done for an interview with [Company Hero].

### Requirements

- [`yarn`]
- [NodeJS], [LTS] recommended

### Deploy your own

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/wizardlink/interview_companyhero/tree/master)

## Getting started

1. [Clone] the repository;
2. [Install] the dependencies using [`yarn`];
3. Run `yarn dev` to start developing the website.

---

You can also use `yarn build && yarn start` to develop the website, however, it is recommended to use `yarn dev` since changes made to files will trigger the code to be re-compiled [JIT].

The theme file for [Ant Design] is located under `styles/ant-theme.less`, there you can change the global variables used by the framework.

## Considerations

I do not recommend messing too much with the [`next.config.js`] considering the issues that are brought from using the `node-fetch` library (used in `structures/Api.ts`) and [Ant Design]. One example being the use of `cssModules`, which breaks the [Ant Design] framework completely.

TypeScript is used in this project for maintaing a more scallable code, however, it is not used when [NextJS] builds the application. That is because the framework treats any warnings as errors, so if you were to, for example, use `require(<Package | File>)` the application would not be built.


<!-- LINKS -->

[company hero]: https://www.companyhero.com/
[`yarn`]: https://yarnpkg.com/
[nodejs]: https://nodejs.org/en/
[lts]: https://en.wikipedia.org/wiki/Long-term_support
[clone]: https://github.com/git-guides/git-clone
[install]: https://yarnpkg.com/cli/install
[jit]: https://en.wikipedia.org/wiki/Just-in-time_compilation
[ant design]: https://ant.design/
[`next.config.js`]: https://nextjs.org/docs/api-reference/next.config.js/introduction
[`node-fetch`]: https://github.com/node-fetch/node-fetch
[nextjs]: https://nextjs.org/
