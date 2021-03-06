Request ID Bundle
=================

[![Build Status](https://travis-ci.org/Avariya/RequestIdBundle.svg?branch=master)](https://travis-ci.org/Avariya/RequestIdBundle)
[![Latest Stable Version](https://poser.pugx.org/avariya/Request-id-bundle/v/stable)](https://packagist.org/packages/avariya/request-id-bundle)
[![Total Downloads](https://poser.pugx.org/avariya/Request-id-bundle/downloads)](https://packagist.org/packages/avariya/request-id-bundle)
[![composer.lock](https://poser.pugx.org/avariya/Request-id-bundle/composerlock)](https://packagist.org/packages/avariya/request-id-bundle)
[![Code Coverage](https://coveralls.io/repos/github/Avariya/RequestIdBundle/badge.svg?branch=master)](https://coveralls.io/github/Avariya/RequestIdBundle)

## Installation

### ***Change composer.json***

Require bundle:

    composer require avariya/request-id-bundle

Add bundle to AppKernel:

    new \Avariya\RequestIdBundle\AvariyaRequestIdBundle(),
    
### ***Add configuration*** _(optional)_
Default values:

    avariya_request_id:
        monolog_support: true
        kernel_subscriber: true
        header: X-Request-Id
        guzzle_middleware:
            guzzle_tag: csa_guzzle.middleware
        
or:

    avariya_request_id:
        monolog_support: false
        kernel_subscriber: false
        guzzle_middleware: false
