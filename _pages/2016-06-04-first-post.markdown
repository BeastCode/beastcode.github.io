---
layout: single-comment
title:  "First Post!"
author_profile: true
date:   2016-06-04 17:58:28 -0700
categories:
comments: true

---


This page is just for test the blog:


{% highlight javascript %}
import { Component } from '@angular/core';
import { RouteConfig, ROUTER_DIRECTIVES } from '@angular/router';
import { UsersRoute } from './users/routes/UsersRoute/UsersRoute';
import { API_PROVIDERS } from './users/services/api';

@Component({
  selector: 'app',
  template: require('./app.html'),
  providers: [ API_PROVIDERS ],
  directives: [ ROUTER_DIRECTIVES ]
})
@RouteConfig([
  {
     path: '/',
     redirectTo: ['/Users', 'UsersList']
  },
  {
    path: '/users/...',
    component: UsersRoute,
    as: 'Users'
  }
])
export class App {

}
{% endhighlight %}
