# httperf cookbook

# Requirements

* [build-essentials](http://community.opscode.com/cookbooks/build-essential)
* [git](http://community.opscode.com/cookbooks/git)
* [autoconf](http://github.com/rubyops/cookbook-autoconf)

## This has been tested on:

* CentOS 6.2
* Ubuntu 10.04.4 LTS (lucid64)

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
           "src_url": "https://github.com/rubyops/httperf.git",
           "git_branch": "master",     // default == nil and therefore isn't used
           "cache_dir": "/usr/local/src" // << default
           "dest_dir": "/tmp/httperf" // << default
       }
       ...
    }


# Author

Author:: Joshua P. Mervine (<joshua@mervine.net>)
