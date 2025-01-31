=========
CHANGELOG
=========

Next Release (TBD)
==================

* Add support for stage independent lambda configuration
  (`#1162 <https://github.com/aws/chalice/pull/1162>`__)
* Add support for subscribing to CloudWatch Events
  (`#1126 <https://github.com/aws/chalice/pull/1126>`__)
* Add a ``description`` argument to CloudWatch schedule events
  (`#1155 <https://github.com/aws/chalice/pull/1155>`__)
* Fix deployment of API Gateway resource policies
  (`#1220 <https://github.com/aws/chalice/pull/1220>`__)


1.10.0
======

* Add experimental support for websockets
  (`#1017 <https://github.com/aws/chalice/issues/1017>`__)
* API Gateway Endpoint Type Configuration
  (`#1160 <https://github.com/aws/chalice/pull/1160>`__)
* API Gateway Resource Policy Configuration
  (`#1160 <https://github.com/aws/chalice/pull/1160>`__)
* Add --merge-template option to package command
  (`#1195 <https://github.com/aws/chalice/pull/1195>`__)
* Add support for packaging via terraform
  (`#1129 <https://github.com/aws/chalice/pull/1129>`__)


1.9.1
=====

* Make MultiDict mutable
  (`#1158 <https://github.com/aws/chalice/issues/1158>`__)


1.9.0
=====

* Update PIP to support up to 19.1.x
  (`#1104 <https://github.com/aws/chalice/issues/1104>`__)
* Fix handling of more complex Accept headers for binary
  content types
  (`#1078 <https://github.com/aws/chalice/issues/1078>`__)
* Raise TypeError when trying to serialize an unserializable
  type
  (`#1100 <https://github.com/aws/chalice/issues/1100>`__)
* Update ``policies.json`` file
  (`#1110 <https://github.com/aws/chalice/issues/1110>`__)
* Support repeating values in the query string
  (`#1131 <https://github.com/aws/chalice/issues/1131>`__)
* Add layer support to chalice package
  (`#1130 <https://github.com/aws/chalice/issues/1130>`__)
* Fix bug with route ``name`` kwarg raising a ``TypeError``
  (`#1112 <https://github.com/aws/chalice/issues/1112>`__)
* Change exceptions to always be logged at the ERROR level
  (`#969 <https://github.com/aws/chalice/issues/969>`__)
* Fix bug handling exceptions during ``chalice invoke`` on
  Python 3.7
  (`#1139 <https://github.com/aws/chalice/issues/1139>`__)
* Add support for API Gateway compression
  (`#672 <https://github.com/aws/chalice/issues/672>`__)
* Add support for both relative and absolute paths for
  ``--package-dir``
  (`#940 <https://github.com/aws/chalice/issues/940>`__)


1.8.0
=====

* Fall back to pure python version of yaml parser
  when unable to compile C bindings for PyYAML
  (`#1074 <https://github.com/aws/chalice/issues/1074>`__)
* Add support for Lambda layers.
  (`#1001 <https://github.com/aws/chalice/issues/1001>`__)


1.7.0
=====

* Fix packaging multiple local directories as dependencies
  (`#1047 <https://github.com/aws/chalice/pull/1047>`__)
* Add support for passing SNS ARNs to ``on_sns_message``
  (`#1048 <https://github.com/aws/chalice/pull/1048>`__)
* Add support for Blueprints
  (`#1023 <https://github.com/aws/chalice/pull/1023>`__)
* Add support for opting-in to experimental features
  (`#1053 <https://github.com/aws/chalice/pull/1053>`__)
* Provide Lambda context in event object
  (`#856 <https://github.com/aws/chalice/issues/856>`__)


1.6.2
=====

* Add support for pip 18.2
  (`#991 <https://github.com/aws/chalice/pull/991>`__)
* Add more detailed debug logs to the packager.
  (`#934 <https://github.com/aws/chalice/pull/934>`__)
* Add support for python3.7
  (`#992 <https://github.com/aws/chalice/pull/992>`__)
* Support bytes for the application/json binary type
  (`#988 <https://github.com/aws/chalice/issues/988>`__)
* Use more compact JSON representation by default for dicts
  (`#958 <https://github.com/aws/chalice/pull/958>`__)
* Log internal exceptions as errors
  (`#254 <https://github.com/aws/chalice/issues/254>`__)
* Generate swagger documentation from docstrings
  (`#574 <https://github.com/aws/chalice/issues/574>`__)


1.6.1
=====

* Fix local mode issue with unicode responses and Content-Length
  (`#910 <https://github.com/aws/chalice/pull/910>`__)
* Fix issue with ``requirements-dev.txt`` not setting up a working
  dev environment
  (`#920 <https://github.com/aws/chalice/pull/920>`__)
* Add support for pip 18
  (`#910 <https://github.com/aws/chalice/pull/908>`__)


1.6.0
=====

* Add ``chalice invoke`` command
  (`#900 <https://github.com/aws/chalice/issues/900>`__)


1.5.0
=====

* Add support for S3 upload_file/download_file in
  policy generator
  (`#889 <https://github.com/aws/chalice/pull/889>`__)


1.4.0
=====

* Add support for generating python 3.6 pipelines
  (`#858 <https://github.com/aws/chalice/pull/858>`__)
* Add support for connecting lambda functions to S3 events
  (`#855 <https://github.com/aws/chalice/issues/855>`__)
* Add support for connecting lambda functions to SNS message
  (`#488 <https://github.com/aws/chalice/issues/488>`__)
* Make ``watchdog`` an optional dependency and add a built in
  ``stat()`` based file poller
  (`#867 <https://github.com/aws/chalice/issues/867>`__)
* Add support for connecting lambda functions to an SQS queue
  (`#884 <https://github.com/aws/chalice/issues/884>`__)


1.3.0
=====

* Add support for Lambdas in a VPC
  (`#413 <https://github.com/aws/chalice/issues/413>`__,
  `#837 <https://github.com/aws/chalice/pull/837>`__,
  `#673 <https://github.com/aws/chalice/pull/673>`__)
* Add support for packaging local directories
  (`#653 <https://github.com/aws/chalice/pull/653>`__)
* Add support for automatically reloading the local
  dev server when files are modified
  (`#316 <https://github.com/aws/chalice/issues/316>`__,
  `#846 <https://github.com/aws/chalice/pull/846>`__,
  `#706 <https://github.com/aws/chalice/pull/706>`__)
* Add support for viewing cloudwatch logs of all
  lambda functions
  (`#841 <https://github.com/aws/chalice/issues/841>`__,
  `#849 <https://github.com/aws/chalice/pull/849>`__)


1.2.3
=====

* Add support for pip 10
  (`#808 <https://github.com/aws/chalice/issues/808>`__)
* Update ``policies.json`` file
  (`#817 <https://github.com/aws/chalice/issues/817>`__)


1.2.2
=====

* Fix package command not correctly setting environment variables
  (`#795 <https://github.com/aws/chalice/issues/795>`__)


1.2.1
=====

* Add CORS headers to error response
  (`#715 <https://github.com/aws/chalice/pull/715>`__)
* Fix parsing empty query strings in local mode
  (`#767 <https://github.com/aws/chalice/pull/767>`__)
* Fix regression in ``chalice package`` when using role arns
  (`#793 <https://github.com/aws/chalice/issues/793>`__)


1.2.0
=====

This release features a rewrite of the core deployment
code used in Chalice.  This is a backwards compatible change
for users, but you may see changes to the autogenerated
files Chalice creates.
Please read the `upgrade notes for 1.2.0
<http://chalice.readthedocs.io/en/latest/upgrading.html#v1-2-0>`__
for more detailed information about upgrading to this release.

* Print out full stack trace when an error occurs
  (`#711 <https://github.com/aws/chalice/issues/711>`__)
* Add ``image/jpeg`` as a default binary content type
  (`#707 <https://github.com/aws/chalice/pull/707>`__)
* Add support for AWS Lambda only projects
  (`#162 <https://github.com/aws/chalice/issues/162>`__,
  `#640 <https://github.com/aws/chalice/issues/640>`__)
* Fix inconsistent IAM role generation with pure lambdas
  (`#685 <https://github.com/aws/chalice/issues/685>`__)
* Rewrite Chalice deployer to more easily support additional AWS resources
  (`#604 <https://github.com/aws/chalice/issues/604>`__)
* Update the ``chalice package`` command to support
  pure lambda functions and scheduled events.
  (`#772 <https://github.com/aws/chalice/issues/772>`__)
* Fix packager edge case normalizing sdist names
  (`#778 <https://github.com/aws/chalice/issues/778>`__)
* Fix SQLAlchemy packaging
  (`#778 <https://github.com/aws/chalice/issues/778>`__)
* Fix packaging abi3, wheels this fixes cryptography 2.2.x packaging
  (`#764 <https://github.com/aws/chalice/issues/764>`__)


1.1.1
=====

* Add ``--connection-timeout`` to the ``deploy`` command
  (`#344 <https://github.com/aws/chalice/issues/344>`__)
* Fix IAM role creation issue
  (`#565 <https://github.com/aws/chalice/issues/565>`__)
* Fix `chalice local` handling of browser requests
  (`#565 <https://github.com/aws/chalice/issues/628>`__)
* Support async/await syntax in automatic policy generation
  (`#565 <https://github.com/aws/chalice/issues/646>`__)
* Support additional PyPi package formats (.tar.bz2)
  (`#720 <https://github.com/aws/chalice/issues/720>`__)


1.1.0
=====

* Default to ``None`` in local mode when no query parameters
  are provided
  (`#593 <https://github.com/aws/chalice/issues/593>`__)
* Add support for binding a custom address for local dev server
  (`#596 <https://github.com/aws/chalice/issues/596>`__)
* Fix local mode handling of routes with trailing slashes
  (`#582 <https://github.com/aws/chalice/issues/582>`__)
* Scale ``lambda_timeout`` parameter correctly in local mode
  (`#579 <https://github.com/aws/chalice/pull/579>`__)
* Add ``--codebuild-image`` to the ``generate-pipeline`` command
  (`#609 <https://github.com/aws/chalice/issues/609>`__)
* Add ``--source`` and ``-buildspec-file`` to the
  ``generate-pipeline`` command
  (`#609 <https://github.com/aws/chalice/issues/619>`__)


1.0.4
=====

* Fix issue deploying some packages in Windows with utf-8 characters
  (`#560 <https://github.com/aws/chalice/pull/560>`__)
* Add support for custom authorizers with ``chalice package``
  (`#580 <https://github.com/aws/chalice/pull/580>`__)


1.0.3
=====

* Fix issue with some packages with `-` or `.` in their distribution name
  (`#555 <https://github.com/aws/chalice/pull/555>`__)
* Fix issue where chalice local returned a 403 for successful OPTIONS requests
  (`#554 <https://github.com/aws/chalice/pull/554>`__)
* Fix issue with chalice local mode causing http clients to hang on responses
  with no body
  (`#525 <https://github.com/aws/chalice/issues/525>`__)
* Add ``--stage`` parameter to ``chalice local``
  (`#545 <https://github.com/aws/chalice/issues/545>`__)
* Fix issue with analyzer that followed recursive functions infinitely
  (`#531 <https://github.com/aws/chalice/issues/531>`__)


1.0.2
=====

* Fix issue where requestParameters were not being mapped
  correctly resulting in invalid generated javascript SDKs
  (`#498 <https://github.com/aws/chalice/issues/498>`__)
* Fix issue where ``api_gateway_stage`` was being
  ignored when set in the ``config.json`` file
  (`#495 <https://github.com/aws/chalice/issues/495>`__)
* Fix bug where ``raw_body`` would raise an exception if no HTTP
  body was provided
  (`#503 <https://github.com/aws/chalice/issues/503>`__)
* Fix bug where exit codes were not properly being propagated during packaging
  (`#500 <https://github.com/aws/chalice/issues/500>`__)
* Add support for Builtin Authorizers in local mode
  (`#404 <https://github.com/aws/chalice/issues/404>`__)
* Fix environment variables being passed to subprocess while packaging
  (`#501 <https://github.com/aws/chalice/issues/501>`__)
* Allow view to require API keys as well as authorization
  (`#473 <https://github.com/aws/chalice/pull/473/>`__)


1.0.1
=====

* Only use alphanumeric characters for event names in SAM template
  (`#450 <https://github.com/aws/chalice/issues/450>`__)
* Print useful error message when config.json is invalid
  (`#458 <https://github.com/aws/chalice/pull/458>`__)
* Fix api gateway stage being set incorrectly in non-default chalice stage
 (`#$70 <https://github.com/aws/chalice/issues/470>`__)


1.0.0
=====

* Change default API Gateway stage name to ``api``
  (`#431 <https://github.com/awslabs/chalice/pull/431>`__)
* Add support for ``CORSConfig`` in ``chalice local``
  (`#436 <https://github.com/awslabs/chalice/issues/436>`__)
* Propagate ``DEBUG`` log level when setting ``app.debug``
  (`#386 <https://github.com/awslabs/chalice/issues/386>`__)
* Add support for wildcard routes and HTTP methods in ``AuthResponse``
  (`#403 <https://github.com/awslabs/chalice/issues/403>`__)
* Fix bug when analyzing list comprehensions
  (`#412 <https://github.com/awslabs/chalice/issues/412>`__)
* Update ``chalice local`` to use HTTP 1.1
  (`#448 <https://github.com/awslabs/chalice/pull/448>`__)


1.0.0b2
=======

Please read the `upgrade notes for 1.0.0b2
<http://chalice.readthedocs.io/en/latest/upgrading.html#v1-0-0b2>`__
for more detailed information about upgrading to this release.

Note: to install this beta version of chalice you must specify
``pip install 'chalice>=1.0.0b2,<2.0.0'`` or
use the ``--pre`` flag for pip: ``pip install --pre chalice``.

* Set env vars from config in ``chalice local``
  (`#396 <https://github.com/awslabs/chalice/issues/396>`__)
* Fix edge case when building packages with optional c extensions
  (`#421 <https://github.com/awslabs/chalice/pull/421>`__)
* Remove legacy ``policy.json`` file support. Policy files must
  use the stage name, e.g. ``policy-dev.json``
  (`#430 <https://github.com/awslabs/chalice/pull/540>`__)
* Fix issue where IAM role policies were updated twice on redeploys
  (`#428 <https://github.com/awslabs/chalice/pull/428>`__)
* Validate route path is not an empty string
  (`#432 <https://github.com/awslabs/chalice/pull/432>`__)
* Change route code to invoke view function with kwargs instead of
  positional args
  (`#429 <https://github.com/awslabs/chalice/issues/429>`__)


1.0.0b1
=======

Please read the `upgrade notes for 1.0.0b1
<http://chalice.readthedocs.io/en/latest/upgrading.html#v1-0-0b1>`__
for more detailed information about upgrading to this release.

Note: to install this beta version of chalice you must specify
``pip install 'chalice>=1.0.0b1,<2.0.0'`` or
use the ``--pre`` flag for pip: ``pip install --pre chalice``.

* Fix unicode responses being quoted in python 2.7
  (`#262 <https://github.com/awslabs/chalice/issues/262>`__)
* Add support for scheduled events
  (`#390 <https://github.com/awslabs/chalice/issues/390>`__)
* Add support for pure lambda functions
  (`#390 <https://github.com/awslabs/chalice/issues/400>`__)
* Add support for wheel packaging.
  (`#249 <https://github.com/awslabs/chalice/issues/249>`__)


0.10.1
======

* Fix deployment issue for projects deployed with versions
  prior to 0.10.0
  (`#387 <https://github.com/awslabs/chalice/issues/387>`__)
* Fix crash in analyzer when encountering genexprs and listcomps
  (`#263 <https://github.com/awslabs/chalice/issues/263>`__)


0.10.0
======

* Fix issue where provided ``iam_role_arn`` was not respected on
  redeployments of chalice applications and in the CloudFormation template
  generated by ``chalice package``
  (`#339 <https://github.com/awslabs/chalice/issues/339>`__)
* Fix ``autogen_policy`` in config being ignored
  (`#367 <https://github.com/awslabs/chalice/pull/367>`__)
* Add support for view functions that share the same view url but
  differ by HTTP method
  (`#81 <https://github.com/awslabs/chalice/issues/81>`__)
* Improve deployment error messages for deployment packages that are
  too large
  (`#246 <https://github.com/awslabs/chalice/issues/246>`__,
  `#330 <https://github.com/awslabs/chalice/issues/330>`__,
  `#380 <https://github.com/awslabs/chalice/pull/380>`__)
* Add support for built-in authorizers
  (`#356 <https://github.com/awslabs/chalice/issues/356>`__)


0.9.0
=====

* Add support for ``IAM`` authorizer
  (`#334 <https://github.com/awslabs/chalice/pull/334>`__)
* Add support for configuring ``lambda_timeout``, ``lambda_memory_size``,
  and ``tags`` in your AWS Lambda function
  (`#347 <https://github.com/awslabs/chalice/issues/347>`__)
* Fix vendor directory contents not being importable locally
  (`#350 <https://github.com/awslabs/chalice/pull/350>`__)
* Add support for binary payloads
  (`#348 <https://github.com/awslabs/chalice/issues/348>`__)


0.8.2
=====

* Fix issue where ``--api-gateway-stage`` was being
  ignored (`#325 <https://github.com/awslabs/chalice/pull/325>`__)
* Add ``chalice delete`` command
  (`#40 <https://github.com/awslabs/chalice/issues/40>`__)


0.8.1
=====

* Alway overwrite existing API Gateway Rest API on updates
  (`#305 <https://github.com/awslabs/chalice/issues/305>`__)
* Added more granular support for CORS
  (`#311 <https://github.com/awslabs/chalice/pull/311>`__)
* Fix duplicate content type header in local model
  (`#311 <https://github.com/awslabs/chalice/issues/310>`__)
* Fix content type validation when charset is provided
  (`#306 <https://github.com/awslabs/chalice/issues/306>`__)
* Add back custom authorizer support
  (`#322 <https://github.com/awslabs/chalice/pull/322>`__)


0.8.0
=====

* Add support for python3!
  (`#296 <https://github.com/awslabs/chalice/pull/296>`__)
* Fix swagger generation when using ``api_key_required=True``
  (`#279 <https://github.com/awslabs/chalice/issues/279>`__)
* Fix ``generate-pipeline`` to install requirements file before packaging
  (`#295 <https://github.com/awslabs/chalice/pull/295>`__)


0.7.0
=====

Please read the `upgrade notes for 0.7.0
<http://chalice.readthedocs.io/en/latest/upgrading.html#v0-7-0>`__
for more detailed information about upgrading to this release.

* Add ``chalice package`` command.  This will
  create a SAM template and Lambda deployment package that
  can be subsequently deployed by AWS CloudFormation.
  (`#258 <https://github.com/awslabs/chalice/pull/258>`__)
* Add a ``--stage-name`` argument for creating chalice stages.
  A chalice stage is a completely separate set of AWS resources.
  As a result, most configuration values can also be specified
  per chalice stage.
  (`#264 <https://github.com/awslabs/chalice/pull/264>`__,
  `#270 <https://github.com/awslabs/chalice/pull/270>`__)
* Add support for ``iam_role_file``, which allows you to
  specify the file location of an IAM policy to use for your app
  (`#272 <https://github.com/awslabs/chalice/pull/272>`__)
* Add support for setting environment variables in your app
  (`#273 <https://github.com/awslabs/chalice/pull/273>`__)
* Add a ``generate-pipeline`` command
  (`#277 <https://github.com/awslabs/chalice/pull/277>`__)


0.6.0
=====

Check out the `upgrade notes for 0.6.0
<http://chalice.readthedocs.io/en/latest/upgrading.html#v0-6-0>`__
for more detailed information about changes in this release.

* Add port parameter to local command
  (`#220 <https://github.com/awslabs/chalice/pull/220>`__)
* Add support for binary vendored packages
  (`#182 <https://github.com/awslabs/chalice/pull/182>`__,
  `#106 <https://github.com/awslabs/chalice/issues/106>`__,
  `#42 <https://github.com/awslabs/chalice/issues/42>`__)
* Add support for customizing the returned HTTP response
  (`#240 <https://github.com/awslabs/chalice/pull/240>`__,
  `#218 <https://github.com/awslabs/chalice/issues/218>`__,
  `#110 <https://github.com/awslabs/chalice/issues/110>`__,
  `#30 <https://github.com/awslabs/chalice/issues/30>`__,
  `#226 <https://github.com/awslabs/chalice/issues/226>`__)
* Always inject latest runtime to allow for chalice upgrades
  (`#245 <https://github.com/awslabs/chalice/pull/245>`__)


0.5.1
=====

* Add support for serializing decimals in ``chalice local``
  (`#187 <https://github.com/awslabs/chalice/pull/187>`__)
* Add stdout handler for root logger when using ``chalice local``
  (`#186 <https://github.com/awslabs/chalice/pull/186>`__)
* Map query string parameters when using ``chalice local``
  (`#184 <https://github.com/awslabs/chalice/pull/184>`__)
* Support Content-Type with a charset
  (`#180 <https://github.com/awslabs/chalice/issues/180>`__)
* Fix not all resources being retrieved due to pagination
  (`#188 <https://github.com/awslabs/chalice/pull/188>`__)
* Fix issue where root resource was not being correctly retrieved
  (`#205 <https://github.com/awslabs/chalice/pull/205>`__)
* Handle case where local policy does not exist
  (`29 <https://github.com/awslabs/chalice/issues/29>`__)


0.5.0
=====

* Add default application logger
  (`#149 <https://github.com/awslabs/chalice/issues/149>`__)
* Return 405 when method is not supported when running
  ``chalice local``
  (`#159 <https://github.com/awslabs/chalice/issues/159>`__)
* Add path params as requestParameters so they can be used
  in generated SDKs as well as cache keys
  (`#163 <https://github.com/awslabs/chalice/issues/163>`__)
* Map cognito user pool claims as part of request context
  (`#165 <https://github.com/awslabs/chalice/issues/165>`__)
* Add ``chalice url`` command to print the deployed URL
  (`#169 <https://github.com/awslabs/chalice/pull/169>`__)
* Bump up retry limit on initial function creation to 30 seconds
  (`#172 <https://github.com/awslabs/chalice/pull/172>`__)
* Add support for ``DELETE`` and ``PATCH`` in ``chalice local``
  (`#167 <https://github.com/awslabs/chalice/issues/167>`__)
* Add ``chalice generate-sdk`` command
  (`#178 <https://github.com/awslabs/chalice/pull/178>`__)


0.4.0
=====

* Fix issue where role name to arn lookup was failing due to lack of pagination
  (`#139 <https://github.com/awslabs/chalice/issues/139>`__)
* Raise errors when unknown kwargs are provided to ``app.route(...)``
  (`#144 <https://github.com/awslabs/chalice/pull/144>`__)
* Raise validation error when configuring CORS and an OPTIONS method
  (`#142 <https://github.com/awslabs/chalice/issues/142>`__)
* Add support for multi-file applications
  (`#21 <https://github.com/awslabs/chalice/issues/21>`__)
* Add support for ``chalice local``, which runs a local HTTP server for testing
  (`#22 <https://github.com/awslabs/chalice/issues/22>`__)


0.3.0
=====

* Fix bug with case insensitive headers
  (`#129 <https://github.com/awslabs/chalice/issues/129>`__)
* Add initial support for CORS
  (`#133 <https://github.com/awslabs/chalice/pull/133>`__)
* Only add API gateway permissions if needed
  (`#48 <https://github.com/awslabs/chalice/issues/48>`__)
* Fix error when dict comprehension is encountered during policy generation
  (`#131 <https://github.com/awslabs/chalice/issues/131>`__)
* Add ``--version`` and ``--debug`` options to the chalice CLI


0.2.0
=====

* Add support for input content types besides ``application/json``
  (`#96 <https://github.com/awslabs/chalice/issues/96>`__)
* Allow ``ChaliceViewErrors`` to propagate, so that API Gateway
  can properly map HTTP status codes in non debug mode
  (`#113 <https://github.com/awslabs/chalice/issues/113>`__)
* Add windows compatibility
  (`#31 <https://github.com/awslabs/chalice/issues/31>`__,
   `#124 <https://github.com/awslabs/chalice/pull/124>`__,
   `#103 <https://github.com/awslabs/chalice/issues/103>`__)


0.1.0
=====

* Require ``virtualenv`` as a package dependency.
  (`#33 <https://github.com/awslabs/chalice/issues/33>`__)
* Add ``--profile`` option when creating a new project
  (`#28 <https://github.com/awslabs/chalice/issues/28>`__)
* Add support for more error codes exceptions
  (`#34 <https://github.com/awslabs/chalice/issues/34>`__)
* Improve error validation when routes containing a
  trailing ``/`` char
  (`#65 <https://github.com/awslabs/chalice/issues/65>`__)
* Validate duplicate route entries
  (`#79 <https://github.com/awslabs/chalice/issues/79>`__)
* Ignore lambda expressions in policy analyzer
  (`#74 <https://github.com/awslabs/chalice/issues/74>`__)
* Print original error traceback in debug mode
  (`#50 <https://github.com/awslabs/chalice/issues/50>`__)
* Add support for authenticate routes
  (`#14 <https://github.com/awslabs/chalice/issues/14>`__)
* Add ability to disable IAM role management
  (`#61 <https://github.com/awslabs/chalice/issues/61>`__)
