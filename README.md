# Wheelie CMS

##### Built on CFWheels and Lucee - Inspired by Wordpress and Xindi**

Wheelie is an open source content management system for CFML, created by [EiQ Interactive LLC](https://eiqinteractive.com). wheelie has been designed to be used by marketing departments, web designers and developers.

##### Demo: [https://wheeliecms.herokuapp.com](https://wheeliecms.herokuapp.com)
##### Note: If you get an "Application Error" message just hit refresh, that's a Heroku bug caused by sleep mode

=======
## Getting started

For those with Docker installed:

Start up a demo instance pre-populated with content:

```
git clone https://github.com/timsayshey/wheelie.git
cd wheelieCMS
docker-compose -f config/docker/local-mysql/docker-compose.yml up
```

Then access the application via:

http://localhost:8080

To login go to http://localhost:8080/manager

```
Username: admin@getwheelie.com
Password: wheelie
```

MYSQL Connection Info:

```
Host: localhost
Port: 55555
Username: root
Passsword: NOT_SECURE_CHANGE
```

Simply hold down control-c to stop the service.

## Compatibility

Lucee 5 and MySQL/PostgreSQL

## Support

* [Github Issues](https://github.com/timsayshey/wheelie/issues)
* [Google Group](https://groups.google.com/forum/#!forum/wheelie-cms)
* [Twitter](http://twitter.com/wheeliecms)
* [Paid Support/Custom Development](http://eiqinteractive.com)

## Wheelie Notes

* Settings:  `/models/services/global/settings.cfm`
* Custom Routes: `/models/services/global/approutes.cfm`
* Application helpers: `/models/services/global/`
* Themes: `/views/themes - Use light-theme as a boilerplate`
* Other layouts and admin theme: `/views/layouts/..`
* Static pages: `/views/static/.. (Override a DB page by placing a cfm file in a site folder with the following name pattern: id_whatever.cfm, ex 4_about.cfm)`
* Shortcode functions: `/views/plugins/..`
* Add your custom app code: `/modules/adminapp and /modules/publicapp - look at existing models and controllers to get an idea of what controllers and models to extend.`

## Contribute

Feel free to make changes and issue a pull request.

## LICENSE

MIT -- See the LICENSE file in the root
