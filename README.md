cf-buildpack-dump
================================================================================

This is a CloudFoundry buildpack that just dumps information about the
app staging environment.  Useful if you're writing your own buildpack, or
curious about what's available when your app is staged.

To use it, you can push any old app with this buildpack, but you can also
push THIS BUILDPACK as an app, since the buildpack doesn't really do anything.

To do this, run:

    cf push --name XYZ-cf-buildpack-dump --buildpack https://github.com/pmuellr/cf-buildpack-dump.git 

You can look at the staging output at any time, with `cf logs`, as in

    cf logs XYZ-cf-buildpack-dump

