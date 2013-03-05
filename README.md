# httperf cookbook

# Requirements

    build_essentials -- [http://community.opscode.com/cookbooks/build-essential]
    git              -- [http://community.opscode.com/cookbooks/git]
    autoconf         -- [http://github.com/rubyops/cookbook-autoconf]

# Usage

    {
        [ "recipe[httperf::default]" ]
    }

# Attributes

    {
        // optional
       "httperf": {
           "branch": "master", // default == nil and therefore isn't used
           "cache": "/tmp/httperf" // << default
       }
       ...
    }


# Author

Author:: Joshua P. Mervine (<joshua@mervine.net>)
