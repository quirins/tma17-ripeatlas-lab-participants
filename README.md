# tma17-ripeatlas-lab-participants
Public Repository for Participants of the TMA'17 PhD School Lab on RIPE Atlas

This repository consists of data specific to the exercise. 
It also contains a submodule tls-cca which points to a git repository with scripts and more data that can be used in the exercise.

Video from [lecture](	https://youtu.be/7Riz80tgkyg) and [lab](https://youtu.be/1froq9uJd9k).


## Structure:

* data
	* dns
		* RIPE-Atlas-measurement-8831682.json -- [a recent DNS measurement](https://atlas.ripe.net/measurements/8831682)
		* RIPE-Atlas-measurement-8831682.json.parsed.txt  -- parsed
		* result-5500014.json -- [Sample DNS measurement from paper](https://atlas.ripe.net/measurements/5500016/)  

		* result-5500014.json.parsed.txt 
	* traceroute 
		* result-5719599-head3.json [Sample traceroute measurement from Paper -- Germany, only 3 results](https://atlas.ripe.net/measurements/5719601/) 
		* result-5719599-head3.json.ip-mappings  -- IP mapping (cache)
		* result-5719599.json  [Sample traceroute measurement from Paper -- Germany, all  results](https://atlas.ripe.net/measurements/5719601/) 
		* result-5719599.json.ip-mappings	-- IP mapping cache
		* result-5719599.json.result.txt -- parsing result
* tls-cca
	* ripe_atlas
		* dns
			* apns-dns-measure-ids.txt  -- RIPE Atlas Measurement IDs
			* atlas-measure.sh   -- RA Batch Measurement Script
			* dns-results-json.sha512   -- SHA512 checksums
			* dns.md -- Description, Readme for DNS part
			* get-results.sh -- RA Batch Result Download Script
			* parse-results.py -- DNS result parsing
			* random-ips-per-subnet.txt  -- ignore
			* ripe-atlas-dns-responses.tar.bz2 -- all results
		* traceroute 
			* README_traceroute.md
			* global - traceroute data for global scan
			* ixp_subnets_v4.csv	  -- traiXroute IXP subnets
			* routeviews-rv2-20160926-1200.pfx2as.xz -- routeviews BGP IP2AS mappings
			* apns-random-ips-per-subnet.txt	-- ignore
			* germany -- traceroute data for Germany-only scan 
			* ipv42pfxas.py   -- library to map IPv4 addresses to prefixes and ASes
			* traceroutes_to_asn_ixp.py -- Script to map traceroute hops to IXPs/ASes
