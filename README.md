kickflip-ios-example
====================

Example project for integration of the [Kickflip iOS SDK](https://github.com/Kickflip/kickflip-ios-sdk) for super easy live broadcasts.
    
## Cocoapods Setup

You'll need to install [Cocoapods](http://cocoapods.org) first. Because you're so bleeding edge, some of our dependencies aren't in the official Cocoapods repo yet, so you'll have to add our Specs repo.

    $ pod repo add kickflip git@github.com:Kickflip/Specs.git
    
## Compiling

Grab the source code, check for changes to our Podspecs repo, and then update the dependencies.

	$ git clone git@github.com:Kickflip/kickflip-ios-example.git
    $ cd kickflip-ios-example
    $ git submodule update --init
    $ pod repo update kickflip
    $ pod
    
If you would like to make modifications to the core SDK, you can integrate the SDK as a submodule as well (check the `Podfile` for more info).

## KFSecrets.h

You'll need to [sign up](http://kickflip.io), make a new app, and then put your API keys from  and put them in a file called `KFSecrets.h` with the following contents:

	#define KICKFLIP_API_KEY @"Client ID from kickflip.io"
	#define KICKFLIP_API_SECRET @"Client Secret from kickflip.io"

## License

Apache 2.0