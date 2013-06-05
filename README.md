# Setup
    
Go to http://logstash.net/ get latest logstash.
start elasticSearch first.


# Usage

    # Running in slave nodes.
    java -jar logstash-1.1.13-flatjar.jar agent -f harvester.conf --watchdog-timeout 1000

    # Running in master nodes.
    java -jar logstash-1.1.13-flatjar.jar agent -f indexer.conf
