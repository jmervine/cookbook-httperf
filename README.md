# httperf cookbook

# Requirements

* [build-essentials](http://community.opscode.com/cookbooks/build-essential)
* [git](http://community.opscode.com/cookbooks/git)
* [autoconf](http://github.com/rubyops/cookbook-autoconf)

## This has been tested on:

* CentOS 6.2

# Usage

    // file: nodes/host.json
    {
        // Required for build-essential.
        //
        // See build-essential docs for custom configs,
        // empty configs as below are acceptable for
        // defaults.
        "build_essential": {},

        // Include autoconf recipe.
        "run_list": [ "recipe[autoconf::default]" ]
    }

# Attributes

    // file: nodes/host.json
    {
       "httperf": {
           "branch": "master",     // default == nil and therefore isn't used
           "cache": "/tmp/httperf" // << default
       }
       ...
    }


# Author

Author:: Joshua P. Mervine (<joshua@mervine.net>)
