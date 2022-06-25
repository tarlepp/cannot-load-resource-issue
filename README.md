# What is this?

Someone asked help on Symfony Slack channel with following error

```bash
Hey guys! Do anyone know how to fix this error?
Cannot load resource "../src/Controller/". Make sure there is a loader supporting the "attribute" type.
```

## What did I do?

I asked that person to share `composer.json` file contents.

https://symfony-devs.slack.com/archives/C3EQ7S3MJ/p1656174420895039?thread_ts=1656173105.327239&cid=C3EQ7S3MJ

And then I just created new project with that `composer.json` that I got.

After that I just run `composer install` command and made simple `IndexController.php`
that uses PHP attributes with route definitions and all worked as expected.

## How to test this?

1. Just clone the repository
2. Run `composer install` command
3. Run `symfony serve` command
4. Open `http://localhost:8000` url on your browser
5. Profit

## License 

MIT
