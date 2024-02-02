# Ideas

## small

### nixpkgs library networking functions

Many things in NixOS use the Internet Protocol and other network related technologies, thus a lot of modules and service have to deal with them.
Currently this is mostly done just passing strings as arguments, but it would be a lot more convenient to have things like `lib.types.ipv6`, `lib.types.ipv4` and other functions to for example convert between cidr notation and the bit representation of netmasks.
Some inspiration for functions can be drawn from similar libraries like the [python ipaddress lib](https://github.com/python/cpython/blob/3.12/Lib/ipaddress.py)
This would not just be useful for NixOS it self but also for its users since a lot of folks use it to power network appliances and build infrastructure on top of it.

Skills required/preferred:
Some prior networking knowledge would be useful but is not required. Prior knowledge of the nix programming language is not required, any new-comer wanting to pick this up should easily be able to complete a nix tutorial like [a tour of Nix](https://nixcloud.io/tour/?id=introduction/nix) in one or two afternoons and be good to go.

Possible mentors:
- @Janik-Haag

Rating:
medium

Prior efforts:
there was some prior efforts in [nixpkgs#258250](https://github.com/NixOS/nixpkgs/pull/258250) but it is stuck for a few months now and also only adds function for legacy ip, it's also quite bare bones and we might want some more advanced things like a function to check if a ip matches a given subnet.

## medium

## large