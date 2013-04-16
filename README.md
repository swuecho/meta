# NAME

Acme::SWUECHO::Meta - a set of tool to learn modules.





# SYNOPSIS

    use Acme::SWUECHO::Meta;
    methods_in_current_pkg

# DESCRIPTION

Acme::SWUECHO::Meta is a set of tool to learn modules.
This is a Acme package, but no one can stop you from using it.

## methods\_in\_current\_pkg

	@methods = methods_in_current_pkg;

find all the method imported in current package. 
you can get the information from the doc, but not always.
However, you can alway get the information from the source code.

The typical usage is to know what methods or funciton are available after you `use module` in your script.



copied from

http://stackoverflow.com/questions/607282/whats-the-best-way-to-discover-all-subroutines-a-perl-module-has

## module\_path

	$module_path = module_path($module);

find the module path

## subs\_in\_pkg

	@methods = subs_in_pkg($module);

this is a method using PPI to do the work, so no need to run the acutual module, but it only include the method 
find in the module\_path.



# AUTHOR

Hao Wu <echowuhao@gmail.com>

# COPYRIGHT

Copyright 2013- Hao Wu

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO
