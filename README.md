puppet-zf
=========

A Puppet module that installs Zend Framework 1.x.x and 2.x.x.

## Sample Usage
Install zf and use the provided configuration defaults:
```puppet
node default {
	class {'zf':} //Default version is 1.12.3
}
```
or
```puppet
node default {
	include zf //Default version is 1.12.3
}
```

Install diferent version:
```puppet
node default {
	class {'zf':
		ensure  => present,
		version => '1.11.11',
	}
}
```
or
```puppet
node default {
	class {'zf':
		ensure  => present,
		version => '2.2.5',
	}
}
```
or yet
```puppet
node default {
	class {'zf':
		ensure  => present,
		version => latest,  //To get a last version
	}
}
```

Install Zend Tool:
```puppet
node default {
	class {'zf':
		ensure => present,
		ztool  => true,
	}
}
```

Uninstall zf:
```puppet
node default {
	class {'zf':
		ensure => absent,
	}
}
```

Contact
-------

Principal developer:
	[Leonardo Thibes](http://leonardothibes.com) => [eu@leonardothibes.com](mailto:eu@leonardothibes.com)

Support
-------

Please log tickets and issues at our [Projects site](https://github.com/leonardothibes/puppet-zf/issues)
