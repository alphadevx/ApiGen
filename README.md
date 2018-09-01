# ApiGen

## Introduction

This is a fork of the original [ApiGen](https://github.com/ApiGen/ApiGen), that updates ApiGen to work with PHP 7.2.  Note that only version 4 works on PHP 7.2 with my fixes, version 5 is still broken here as well as on the main ApiGen project.  If you need ApiGen 5, you should wait for the main project to fix that.

## Installation

Add this to your _composer.json_:

	{
	    "repositories": [
	        {
	            "type": "vcs",
	            "url": "https://github.com/alphadevx/ApiGen"
	        }
	    ],
	    "require": {
	        "apigen/apigen": "v4.1.3"
	    }
	}

## Usage

Simple:

	vendor/bin/apigen generate --source ~/Git/alpha/Alpha/ --destination ~/Documents/alpha/api/3.0.0

Complex:

	vendor/bin/apigen generate --source ~/Git/alpha/Alpha/ --destination ~/Documents/alpha/api/3.0.0 --template-config vendor/apigen/theme-bootstrap/src/config.neon --title "Alpha Framework 3.0.0 API Documentation"