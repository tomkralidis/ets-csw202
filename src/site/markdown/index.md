CSW 2.0.1 compliance test suite
===================================

Overview
----------
This test suite is based on the following OGC specifications:
- OGC Catalogue Services Specification - 2.0.1 [OGC 04-021r3](http://portal.opengeospatial.org/files/?artifact_id=5929&amp;version=2) 
- OpenGIS Web Services Common Specification - 1.0.0 [OGC 05-008c1](https://portal.opengeospatial.org/files/?artifact_id=8798")

The conformance tests provided here are **not** intended to be used
in a stand-alone manner, but to be incorporated into profile-specific test suites; they apply to all CSW-based catalogue implementations.

What is tested
--------------------
- GetCapabilities, GET method
- DescribeRecord, POST method
- GetRecordById, GET method
- GetRecords, POST method

What is not tested
-------------------------
- GetCapabilities with updateSequence parameter
- SOAP protocol bindings
- Spatial predicates Beyond, DWithin (broken filter schema)
- Arithmetic operators
- Distributed search
- Asynchronous processing
- Persistent result sets
- Transaction (profile-specific)
- Harvest (profile-specific)


Test data
---------------

The [CSW-2.0.1 test data("../../../data/data-csw-2.0.1.zip") are
available in the common CSW record format. Loading the records into the catalogue is a precondition for compliance testing. While the test data are represented as a collection of csw:Record instances, no assumption is made about which application profile is supported by the implementation. It is expected that each profile defines a suitable mapping for csw:Record items.

Notes
-------------------

The test engine can only execute the whole test suite, it cannot be used to run single tests or test groups directly. See the TEAM engine documentation for details on how to run scripts locally, or re-execute single tests.


Contributors
--------------
   - Luis Bermudez - (OGC) - 2010-2013

License
-----------

Apache 2.0 ...





Release Notes
----------------

Release notes are available [here](relnotes.md).
