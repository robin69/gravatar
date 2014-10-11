gravatar
========

PHP Class Object to get a gravatar profil for simply use in a Website that uses CodeIgniter or not.
Author : Robin Rumeau - robin.rumeau@gmail.com


SETTINGS :
----------
If you decide to use Gravatar in a non-CodeIgniter's website, the set the $ci_use to FALSE;

HOW TO USE :
-----------

If The library is load in the CI controller then you have to load the library passing it an empty params either the constructor
will generate a fatal error.
Ex. :
		$string = "";
		$this->load->library("gravatar",$string);

Then call the class in a CI view is as simple as
			$profile = new Gravatar("toto@tata.com");
and then using the data profil like this :
			echo $profile->displayName;
			
Anyway you should check first if $profile!=FALSE that means there's no profile for this email adress.

