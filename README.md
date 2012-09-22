# About
Will do a simple GET request using basic auth against the [GitHub API](http://developer.github.com/v3/), getting **all repositories** from the given **organization**. Then, for each one of them, will try to find a **rebar.config** file and look for the given **dependency** in it.

**NOTE**: Actually, to find the dependency, the string is searched for in the rebar.config file, so it might trigger some false alarms (this is ok, for my needs, but feel free to do some more complex "algorithm" to find your deps).

# Use
    $ ./find_rebar_deps <authuser> <authpass> <organization> <dependency>

 * authuser and authpass: Used to authtenticate against the github api.
 * organization: The github organization that owns the repos. 
 * dependency: The dependency to look for in rebar.config.


