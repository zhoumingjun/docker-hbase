# docker-hbase
* start server

	docker create -v /data --name hbase-data zhoumingjun/hbase
	
	docker run -d --volumes-from hbase-data --name hbase-server -p 9090:9090 zhoumingjun/hbase

* stop server 

	docker stop hbase-server  
	
	docker rm hbase-server  
	
	docker rm -v hbase-data