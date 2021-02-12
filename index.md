
## Business Dashboard Overview
A business dashboard is a visualization of data which helps business users to tracke their busines performacne and metrics in a dashboard layout. The Dashboard Buidler helps you to fatche and compiel complex data using a drag-and-drop tool and generates code for sharing your dashboard with the entire business community in few clicks. 
![](https://raw.githubusercontent.com/DashboardBuilder/business-dashboard/gh-pages/repository-open-graph-template.png)


## What is a Business Dashboard tool and how to it works

A business dashboard builder is a powerful drag-and-drop tool which doesn’t require any programming skill to create a coplex business dashboard. The business dashboad builder t tracks and simplifies complex data query and gives quick insight of business performance to the business users.

# Why do companies use business dashboards?

The main reason for using a business dashboard is to provide a comprehensive view of business performance. A business dashboard summarizes different sections of business with easy-to-understand in a graphical layout.

# Which Different Types of Business Dashboards Exist?
https://raw.githubusercontent.com/DashboardBuilder/business-dashboard/gh-pages/databases-mini.png





It is designed to be displayed on a large screen in a monitoring room or an open space office.

The current dashboard is currently composed of 5 widgets :

* **General Info** : Version, number of host databases, etc. 
* **Hit Ratio** : The % of data found in cache
* **Buffers** : The number of new buffers allocated
* **Queries** : The number of active queries currently running of the instance
* **Twitter** : A glimpse of the #PostgreSQL feed

Adding a new job should be fairly easy. this tool is design so that you can write a custom widget to display stats you find relevant or build a dynamic graph on some "business logic" valuation.

The layout is also entirely flexible. You can easily drag'n'drop any widget to put it wherever you want on the screen. And HTML code of the dashboard can be modified for specific needs, such as specific screen dimensions.

## Quick Start

If you already have installed a Ruby environnement, simply type:

```
  git clone https://github.com/daamien/PostgreSQL-Dashboard.git
  cd PostgreSQL-Dashboard
  bundle
  mv config_postgresql.rb.example config_postgresql.rb
  vi config_postgresql.rb
  dashing start
```

Now go to [http://localhost:3030]() and have fun!

For more instructions, please read [INSTALL.md](https://github.com/daamien/pgDashboard/blob/master/INSTALL.md)

## Requirements

PostgreSQL Dashboard is based on Dashing, a very nice dashboard framework.
Dashing itself is based on Sinatra, a very nice Ruby web framework.

Basically to run this tool, you will need:
 
* PostgreSQL 9.0.x or later
* Ruby 1.9.x or later
* Sinatara 1.4.x or later
* Dashing 1.3.x or later

## Security

__You need to be careful about the security of your PostgreSQL server when installing this tool .__

Therefore I **strongly** recommend the following precautions :

* [Read the Great PostgreSQL Documentation](http://www.postgresql.org/docs/current/static/auth-pg-hba-conf.html)
* Check your ``pg_hba.conf`` file
* Do not allow users to access PostgreSQL Dashboard from the Internet
* Do not use a superuser in the config_postgresql.rb file


## License 

PostgreSQL Dashboard is distributed under the PostgreSQL License.

Dashing is distributed under the MIT License.

The name "PostgreSQL" is registered trademark and the PostgreSQL Logo is a copyrighted design of the PostgreSQL Global Development Group.

## Links

  * Check out the [Dashing documentation](http://shopify.github.com/dashing) for more information.
