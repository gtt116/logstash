# Setup
    
start elasticSearch first.

# Topology

beaver, beaver, beaver --> redis <--> logstash --> ElasticSearch


# Usage

    # Running in slave nodes.
    pip install beaver #beaver is a lighweight logstash shiper.
    beaver -c beaver.conf -t redis

    # Running in master nodes.
    java -jar logstash-1.3.3-flatjar.jar agent -f indexer.conf
