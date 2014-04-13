After having a look to the project "[AngularJS Django Rest Framework Seed]" (by [zackargyle], I decided to fork and split it in at least two projects.

# Way of working

I really do not know if it is going to work, but the idea is:

1. Choose and clone the Server repository.
1. Choose and clone the Client repository.
1. Create a common repository for your app.
1. Add the client and server repositories as [Git submodules]

Once this has been done:

* Write client functionality on the client repository.
* Write server functionality on the server repository.
* Write acceptance tests on the parent repository.
* If you want to update your client or server repository with the newest scaffold (maybe to fetch the building scripts or something like that), just merge it again on your project.


# Current projects

These are the projects, that can communicate each other:

## Servers

* [Seed Project Django] is a [Django] server scaffold to start building servers in the fast way.

## Clients

* [Seed Project AngularJS] is an [AngularJS] scaffold to start building clients.


The idea is to create a common minimal base project that can be used with any server and client. All of them should be interchangeable.

# Requirements

## API

Servers and clients should respect this common [ReST] API:

(TO BE DONE)

# License

All projects and subprojects on this meta-projects should be [MIT licensed]:

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


[AngularJS Django Rest Framework Seed]: https://github.com/zackargyle/angularjs-django-rest-framework-seed
[zackargyle]: https://github.com/zackargyle
[Seed Project Django]: https://github.com/magmax/seed-project-django
[Django]: https://www.djangoproject.com/
[AngularJS]: http://angularjs.org/
[ReST]: http://en.wikipedia.org/wiki/Representational_state_transfer
[Git submodules]: http://git-scm.com/book/en/Git-Tools-Submodules
[MIT licensed]: http://opensource.org/licenses/MIT
