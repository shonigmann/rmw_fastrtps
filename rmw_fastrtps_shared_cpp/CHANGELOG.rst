^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package rmw_fastrtps_shared_cpp
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

4.5.0 (2021-03-18)
------------------
* Take and return new RMW_DURATION_INFINITE correctly (`#515 <https://github.com/ros2/rmw_fastrtps/issues/515>`_)
* Contributors: Emerson Knapp

4.4.0 (2021-03-01)
------------------
* Add RMW function to check QoS compatibility (`#511 <https://github.com/ros2/rmw_fastrtps/issues/511>`_)
* Capture cdr exceptions (`#505 <https://github.com/ros2/rmw_fastrtps/issues/505>`_)
* Contributors: Jacob Perron, Miguel Company

4.3.0 (2021-01-25)
------------------

4.2.0 (2020-12-10)
------------------
* Make sure to lock the mutex protecting client_endpoints\_. (`#492 <https://github.com/ros2/rmw_fastrtps/issues/492>`_)
* Contributors: Chris Lalancette

4.1.0 (2020-12-08)
------------------
* Use interface whitelist for localhost only (`#476 <https://github.com/ros2/rmw_fastrtps/issues/476>`_)
* Make use of error return value in decrement_context_impl_ref_count (`#488 <https://github.com/ros2/rmw_fastrtps/issues/488>`_)
* Remove unnecessary includes (`#487 <https://github.com/ros2/rmw_fastrtps/issues/487>`_)
* Use new time_utils function to limit rmw_time_t values to 32-bits (`#485 <https://github.com/ros2/rmw_fastrtps/issues/485>`_)
* New environment variable to change easily the publication mode (`#470 <https://github.com/ros2/rmw_fastrtps/issues/470>`_)
* Remove unused headers MessageTypeSupport.hpp and ServiceTypeSupport.hpp (`#481 <https://github.com/ros2/rmw_fastrtps/issues/481>`_)
* Contributors: Jacob Perron, José Luis Bueno López, Michael Jeronimo, Miguel Company, Stephen Brawner

4.0.0 (2020-10-22)
------------------
* Discriminate when the Client has gone from when the Client has not completely matched (`#467 <https://github.com/ros2/rmw_fastrtps/issues/467>`_)
  * Workaround when the client is gone before server sends response
  * Change add to the map to listener callback
* Update the package.xml files with the latest Open Robotics maintainers (`#459 <https://github.com/ros2/rmw_fastrtps/issues/459>`_)
* Update Quality Declarations and READMEs (`#455 <https://github.com/ros2/rmw_fastrtps/issues/455>`_)
  * Add QD links for dependencies to rmw_fastrtps_shared_cpp QD.
  * Provide external dependencies QD links.
  * Update rmw_fastrtps_shared_cpp QD: Fast DDS
  * Update README rmw_fastrtps_shared_cpp to QL2
* Contributors: JLBuenoLopez-eProsima, Jaime Martin Losa, José Luis Bueno López, Michael Jeronimo

3.1.4 (2020-10-02)
------------------
* Perform fault injection in all creation/destruction APIs. (`#453 <https://github.com/ros2/rmw_fastrtps/issues/453>`_)
* Ensure rmw_destroy_node() completes despite run-time errors. (`#458 <https://github.com/ros2/rmw_fastrtps/issues/458>`_)
* Handle too large QoS queue depths.  (`#457 <https://github.com/ros2/rmw_fastrtps/issues/457>`_)
* Update rmw_fastrtps_cpp and rmw_fastrtps_shared_cpp QDs to QL2. (`#456 <https://github.com/ros2/rmw_fastrtps/issues/456>`_)
* Contributors: Michel Hidalgo

3.1.3 (2020-09-29)
------------------
* checked client implementation and return RMW_RET_INCORRECT_RMW_IMPLEMENTATION (`#451 <https://github.com/ros2/rmw_fastrtps/issues/451>`_)
* Update service/client request/response API error returns (`#450 <https://github.com/ros2/rmw_fastrtps/issues/450>`_)
* Contributors: Alejandro Hernández Cordero, Jose Tomas Lorente

3.1.2 (2020-09-25)
------------------
* Updated publisher/subscription allocation and wait set API return codes (`#443 <https://github.com/ros2/rmw_fastrtps/issues/443>`_)
* Added rmw_logging tests (`#442 <https://github.com/ros2/rmw_fastrtps/issues/442>`_)
* Contributors: Alejandro Hernández Cordero

3.1.1 (2020-09-24)
------------------
* Add tests for RMW QoS to DDS attribute conversion. (`#449 <https://github.com/ros2/rmw_fastrtps/issues/449>`_)
* Make service/client construction/destruction implementation compliant (`#445 <https://github.com/ros2/rmw_fastrtps/issues/445>`_)
* Contributors: Michel Hidalgo

3.1.0 (2020-09-23)
------------------
* Inject faults on __rmw_publish() and run_listener_thread() call. (`#441 <https://github.com/ros2/rmw_fastrtps/issues/441>`_)
* Update gid API return codes. (`#440 <https://github.com/ros2/rmw_fastrtps/issues/440>`_)
* Update graph API return codes. (`#436 <https://github.com/ros2/rmw_fastrtps/issues/436>`_)
* Contributors: Michel Hidalgo

3.0.0 (2020-09-18)
------------------
* Update rmw_take_serialized() and rmw_take_with_message_info() error returns  (`#435 <https://github.com/ros2/rmw_fastrtps/issues/435>`_)
* Update rmw_take() error returns (`#432 <https://github.com/ros2/rmw_fastrtps/issues/432>`_)
* Update rmw_publish() error returns (`#430 <https://github.com/ros2/rmw_fastrtps/issues/430>`_)
* Update rmw_publish_serialized_message() error returns (`#431 <https://github.com/ros2/rmw_fastrtps/issues/431>`_)
* Contributors: Jose Tomas Lorente, Lobotuerk

2.6.0 (2020-08-28)
------------------
* Improve __rmw_create_wait_set() implementation. (`#427 <https://github.com/ros2/rmw_fastrtps/issues/427>`_)
* Ensure compliant matched pub/sub count API. (`#424 <https://github.com/ros2/rmw_fastrtps/issues/424>`_)
* Ensure compliant publisher QoS queries. (`#425 <https://github.com/ros2/rmw_fastrtps/issues/425>`_)
* Fix memory leak that wait_set might be not destoryed in some case. (`#423 <https://github.com/ros2/rmw_fastrtps/issues/423>`_)
* Contributors: Chen Lihui, Michel Hidalgo

2.5.0 (2020-08-07)
------------------
* Avoid unused identifier variable warnings. (`#422 <https://github.com/ros2/rmw_fastrtps/issues/422>`_)
* Fix trying to get topic data that was already removed. (`#417 <https://github.com/ros2/rmw_fastrtps/issues/417>`_)
* Contributors: Chen Lihui, Michel Hidalgo

2.4.0 (2020-08-06)
------------------
* Ensure compliant subscription API. (`#419 <https://github.com/ros2/rmw_fastrtps/issues/419>`_)
* Use package path to TypeSupport.hpp headers in ServiceTypeSupport and MessageTypeSupport (`#415 <https://github.com/ros2/rmw_fastrtps/issues/415>`_)
  Use package in path to TypeSupport header for ServiceTypeSupport/MessageTypeSupport
* Contributors: Jose Luis Rivero, Michel Hidalgo

2.3.0 (2020-07-30)
------------------
* Ensure compliant publisher API. (`#414 <https://github.com/ros2/rmw_fastrtps/issues/414>`_)
* Contributors: Michel Hidalgo

2.2.0 (2020-07-22)
------------------
* Set context actual domain id (`#410 <https://github.com/ros2/rmw_fastrtps/issues/410>`_)
* Contributors: Ivan Santiago Paunovic

2.1.0 (2020-07-20)
------------------
* Add missing thread-safety annotation in ServicePubListener (`#409 <https://github.com/ros2/rmw_fastrtps/issues/409>`_)
* Ensure compliant node construction/destruction API. (`#408 <https://github.com/ros2/rmw_fastrtps/issues/408>`_)
* Contributors: Michel Hidalgo

2.0.0 (2020-07-08)
------------------
* Update Quality Declarations to QL3. (`#404 <https://github.com/ros2/rmw_fastrtps/issues/404>`_)
* Contributors: Michel Hidalgo

1.1.0 (2020-06-29)
------------------
* Do not use string literals as implementation identifiers in tests. (`#402 <https://github.com/ros2/rmw_fastrtps/issues/402>`_)
* Ensure compliant init options API implementations. (`#399 <https://github.com/ros2/rmw_fastrtps/issues/399>`_)
* Finalize context iff shutdown. (`#396 <https://github.com/ros2/rmw_fastrtps/issues/396>`_)
* Handle RMW_DEFAULT_DOMAIN_ID. (`#394 <https://github.com/ros2/rmw_fastrtps/issues/394>`_)
* Make service wait for response reader (`#390 <https://github.com/ros2/rmw_fastrtps/issues/390>`_)
* Contributors: Michel Hidalgo, Miguel Company

1.0.1 (2020-06-01)
------------------
* Add Security Vulnerability Policy pointing to REP-2006 (`#389 <https://github.com/ros2/rmw_fastrtps/issues/389>`_)
* Do not compile assert death tests in Release builds (`#393 <https://github.com/ros2/rmw_fastrtps/issues/393>`_)
* Add test coverage for name mangling and namespacing-specific API (`#388 <https://github.com/ros2/rmw_fastrtps/issues/388>`_)
* Add test coverage for GUID utilities (`#387 <https://github.com/ros2/rmw_fastrtps/issues/387>`_)
* Drop unused TopicCache sources (`#386 <https://github.com/ros2/rmw_fastrtps/issues/386>`_)
* Add test coverage for rmw_init_options API (`#385 <https://github.com/ros2/rmw_fastrtps/issues/385>`_)
* Update QDs for 1.0 (`#383 <https://github.com/ros2/rmw_fastrtps/issues/383>`_)
* Contributors: Chris Lalancette, Michel Hidalgo, Stephen Brawner

1.0.0 (2020-05-12)
------------------
* Remove API related to manual by node liveliness. (`#379 <https://github.com/ros2/rmw_fastrtps/issues/379>`_)
* Update quality declarations on feature testing. (`#380 <https://github.com/ros2/rmw_fastrtps/issues/380>`_)
* Contributors: Ivan Santiago Paunovic, Michel Hidalgo

0.9.1 (2020-05-08)
------------------
* Fill service_info timestamps from sample_info (`#378 <https://github.com/ros2/rmw_fastrtps/issues/378>`_)
* Fix unused variabled warning (`#377 <https://github.com/ros2/rmw_fastrtps/issues/377>`_)
* Add basic support for security logging plugin (`#362 <https://github.com/ros2/rmw_fastrtps/issues/362>`_)
* Add package READMEs and QUALITY_DECLARATION files (`#375 <https://github.com/ros2/rmw_fastrtps/issues/375>`_)
* Added doxyfiles (`#372 <https://github.com/ros2/rmw_fastrtps/issues/372>`_)
* Contributors: Alejandro Hernández Cordero, Ingo Lütkebohle, Jacob Perron, Kyle Fazzari, brawner

0.9.0 (2020-04-28)
------------------
* Feature/services timestamps. (`#369 <https://github.com/ros2/rmw_fastrtps/issues/369>`_)
* Add support for taking a sequence of messages. (`#366 <https://github.com/ros2/rmw_fastrtps/issues/366>`_)
* Fill message_info timestamp. (`#368 <https://github.com/ros2/rmw_fastrtps/issues/368>`_)
* Export targets in a addition to include directories / libraries. (`#371 <https://github.com/ros2/rmw_fastrtps/issues/371>`_)
* Support for API break on Fast RTPS 2.0. (`#370 <https://github.com/ros2/rmw_fastrtps/issues/370>`_)
* security-context -> enclave. (`#365 <https://github.com/ros2/rmw_fastrtps/issues/365>`_)
* Switch to one Participant per Context. (`#312 <https://github.com/ros2/rmw_fastrtps/issues/312>`_)
* Correct error message when event is not supported. (`#358 <https://github.com/ros2/rmw_fastrtps/issues/358>`_)
* Add rmw\_*_event_init() functions. (`#354 <https://github.com/ros2/rmw_fastrtps/issues/354>`_)
* Fixing type support C/CPP mix on rmw_fastrtps_dynamic_cpp. (`#350 <https://github.com/ros2/rmw_fastrtps/issues/350>`_)
* Fix build warning in Ubuntu Focal. (`#346 <https://github.com/ros2/rmw_fastrtps/issues/346>`_)
* Change rmw_topic_endpoint_info_array.count to .size. (`#348 <https://github.com/ros2/rmw_fastrtps/issues/348>`_)
* Code style only: wrap after open parenthesis if not in one line. (`#347 <https://github.com/ros2/rmw_fastrtps/issues/347>`_)
* Fix unprotected use of mutex-guarded variable. (`#345 <https://github.com/ros2/rmw_fastrtps/issues/345>`_)
* Passing down type support information (`#342 <https://github.com/ros2/rmw_fastrtps/issues/342>`_)
* Implement functions to get publisher and subcription informations like QoS policies from topic name. (`#336 <https://github.com/ros2/rmw_fastrtps/issues/336>`_)
* Contributors: Dirk Thomas, Emerson Knapp, Ingo Lütkebohle, Ivan Santiago Paunovic, Jaison Titus, Miaofei Mei, Michael Carroll, Miguel Company, Mikael Arguedas

0.8.1 (2019-10-23)
------------------
* Restrict traffic to localhost only if env var is provided (`#331 <https://github.com/ros2/rmw_fastrtps/issues/331>`_)
* Added new functions which can be used to get rmw_qos_profile_t from WriterQos and ReaderQos (`#328 <https://github.com/ros2/rmw_fastrtps/issues/328>`_)
* Renamed dds_qos_to_rmw_qos to dds_attributes_to_rmw_qos (`#330 <https://github.com/ros2/rmw_fastrtps/issues/330>`_)
* Contributors: Brian Marchi, jaisontj

0.8.0 (2019-09-25)
------------------
* Correct error message (`#320 <https://github.com/ros2/rmw_fastrtps/issues/320>`_)
* Return specific error code when node is not found (`#311 <https://github.com/ros2/rmw_fastrtps/issues/311>`_)
* Correct linter failure (`#318 <https://github.com/ros2/rmw_fastrtps/issues/318>`_)
* Fix bug in graph API by node (`#316 <https://github.com/ros2/rmw_fastrtps/issues/316>`_)
* fix method name change from 1.8.1->1.9.0 (`#302 <https://github.com/ros2/rmw_fastrtps/issues/302>`_)
* Add missing lock guards for discovered_names and discovered_namespaces (`#301 <https://github.com/ros2/rmw_fastrtps/issues/301>`_)
* Add function for getting clients by node (`#293 <https://github.com/ros2/rmw_fastrtps/issues/293>`_)
* Enable manual_by_node and node liveliness assertion (`#298 <https://github.com/ros2/rmw_fastrtps/issues/298>`_)
* Enable assert liveliness on publisher. (`#296 <https://github.com/ros2/rmw_fastrtps/issues/296>`_)
* Use rcpputils::find_and_replace instead of std::regex_replace (`#291 <https://github.com/ros2/rmw_fastrtps/issues/291>`_)
* Fix a comparison with a sign mismatch (`#288 <https://github.com/ros2/rmw_fastrtps/issues/288>`_)
* Implement get_actual_qos() for subscriptions (`#287 <https://github.com/ros2/rmw_fastrtps/issues/287>`_)
* add missing qos setings in get_actual_qos() (`#284 <https://github.com/ros2/rmw_fastrtps/issues/284>`_)
* Fix ABBA deadlock.
* Contributors: Chris Lalancette, Emerson Knapp, Jacob Perron, M. M, Scott K Logan, William Woodall, ivanpauno

0.7.3 (2019-05-29)
------------------
* Protection of discovered_names and discovered_namespaces (`#283 <https://github.com/ros2/rmw_fastrtps/issues/283>`_)
* Disable all liveliness until it is actually supported (`#282 <https://github.com/ros2/rmw_fastrtps/issues/282>`_)
* Contributors: Emerson Knapp, MiguelCompany

0.7.2 (2019-05-20)
------------------
* fix log_debug typo in rmw_count (`#279 <https://github.com/ros2/rmw_fastrtps/issues/279>`_)
* Fastrtps18 event callbacks policies (`#275 <https://github.com/ros2/rmw_fastrtps/issues/275>`_)
* Centralize topic name creation logic and update to match FastRTPS 1.8 API (`#272 <https://github.com/ros2/rmw_fastrtps/issues/272>`_)
* Contributors: 1r0b1n0, Emerson Knapp, Nick Burek

0.7.1 (2019-05-08)
------------------
* Support arbitrary message namespaces  (`#266 <https://github.com/ros2/rmw_fastrtps/issues/266>`_)
* Set more correct return values for unimplemented features (`#276 <https://github.com/ros2/rmw_fastrtps/issues/276>`_)
* Add qos interfaces with no-op (`#271 <https://github.com/ros2/rmw_fastrtps/issues/271>`_)
* Updates for preallocation API. (`#274 <https://github.com/ros2/rmw_fastrtps/issues/274>`_)
* Fix logging in rmw_node_info_and_types.cpp (`#273 <https://github.com/ros2/rmw_fastrtps/issues/273>`_)
* Contributors: Emerson Knapp, Jacob Perron, Michael Carroll, Ross Desmond, Thomas Moulard

0.7.0 (2019-04-13)
------------------
* Thread safety annotation - minimally intrusive first pass (`#259 <https://github.com/ros2/rmw_fastrtps/issues/259>`_)
* Add function to get publisher actual qos settings (`#267 <https://github.com/ros2/rmw_fastrtps/issues/267>`_)
* Fixed race condition between taking sample and updating counter. (`#264 <https://github.com/ros2/rmw_fastrtps/issues/264>`_)
* Fix cpplint error
* change count type to size_t to avoid warning (`#262 <https://github.com/ros2/rmw_fastrtps/issues/262>`_)
* update listener logic for accurate counting (`#262 <https://github.com/ros2/rmw_fastrtps/issues/262>`_)
* Make sure to include the C++ headers used by these headers. (`#256 <https://github.com/ros2/rmw_fastrtps/issues/256>`_)
* pass context to wait set and fini context (`#252 <https://github.com/ros2/rmw_fastrtps/issues/252>`_)
* Improve service_is_available logic to protect that client is waiting forever (`#238 <https://github.com/ros2/rmw_fastrtps/issues/238>`_)
* Merge pull request `#250 <https://github.com/ros2/rmw_fastrtps/issues/250>`_ from ros2/support_static_lib
* use namespace_prefix from shared package
* make namespace_prefix header public
* Use empty() to check for an empty string (`#247 <https://github.com/ros2/rmw_fastrtps/issues/247>`_)
* We can compare a std::string with a const char* using operator==, simplifies the code (`#248 <https://github.com/ros2/rmw_fastrtps/issues/248>`_)
* Use empty() instead of size() to check if a vector/map contains elements and fixed some incorrect logging (`#245 <https://github.com/ros2/rmw_fastrtps/issues/245>`_)
* Fix guard condition trigger error (`#235 <https://github.com/ros2/rmw_fastrtps/issues/235>`_)
* Contributors: Chris Lalancette, Dirk Thomas, DongheeYe, Emerson Knapp, Jacob Perron, Johnny Willemsen, Ricardo González, William Woodall, ivanpauno

0.6.1 (2018-12-06)
------------------
* Add topic cache object for managing topic relations (`#236 <https://github.com/ros2/rmw_fastrtps/issues/236>`_)
* Fix lint: remove trailing whitespace (`#244 <https://github.com/ros2/rmw_fastrtps/issues/244>`_)
* Fastrtps 1.7.0 (`#233 <https://github.com/ros2/rmw_fastrtps/issues/233>`_)
* RMW_FastRTPS configuration from XML only (`#243 <https://github.com/ros2/rmw_fastrtps/issues/243>`_)
* Methods to retrieve matched counts on pub/sub (`#234 <https://github.com/ros2/rmw_fastrtps/issues/234>`_)
* use uint8_array (`#240 <https://github.com/ros2/rmw_fastrtps/issues/240>`_)
* Contributors: Jacob Perron, Juan Carlos, Karsten Knese, Michael Carroll, MiguelCompany, Ross Desmond

0.6.0 (2018-11-16)
------------------
* use new error handling API from rcutils (`#231 <https://github.com/ros2/rmw_fastrtps/issues/231>`_)
* Add semicolons to all RCLCPP and RCUTILS macros. (`#229 <https://github.com/ros2/rmw_fastrtps/issues/229>`_)
* separating identity and permission CAs (`#227 <https://github.com/ros2/rmw_fastrtps/issues/227>`_)
* Include node namespaces in get_node_names (`#224 <https://github.com/ros2/rmw_fastrtps/issues/224>`_)
* allow builtin reader/writer to reallocate memory if needed (`#221 <https://github.com/ros2/rmw_fastrtps/issues/221>`_)
* Improve runtime performance of `rmw_count_XXX` functions (`#216 <https://github.com/ros2/rmw_fastrtps/issues/216>`_) (`#217 <https://github.com/ros2/rmw_fastrtps/issues/217>`_)
* Merge pull request `#218 <https://github.com/ros2/rmw_fastrtps/issues/218>`_ from ros2/pr203
* Refs `#3061 <https://github.com/ros2/rmw_fastrtps/issues/3061>`_. Leaving common code only on rmw_fastrtps_shared_cpp.
* Refs `#3061 <https://github.com/ros2/rmw_fastrtps/issues/3061>`_. Package rmw_fastrtps_cpp copied to rmw_fastrtps_shared_cpp.
* Contributors: Chris Lalancette, Dirk Thomas, Guillaume Autran, Michael Carroll, Miguel Company, Mikael Arguedas, William Woodall

0.5.1 (2018-06-28)
------------------

0.5.0 (2018-06-23)
------------------

0.4.0 (2017-12-08)
------------------
