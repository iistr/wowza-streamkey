# wowza-streamkey
Professional Wowza publisher/watcher secure Key protect Addon / with(Mysql)

tivic v1.3b (live plugin)
This project an addon method that uses Wowza Streaming Engine to deliver all media chunks and encryption(pubs/watchs) keys with mysql
so.. is a professional publisher/watcher secure protect the same like "twitch , livestream , ustream , etc.."
all of the software can be easy integration (self Php code,WHMCS,etc..) 
and works realtime(update,write,reading) sync your database..

Setup: open this file
<application>/live/Application.xml

Module Line:
			<!-- tivic 1.0.3 Module -->
			</Module>
				<Module>
				<Name>tivic</Name>
				<Description>TivicPlugin Developer By Levent inan (Twitter:@buyukmavi)</Description>
				<Class>com.wowza.tv.tivic</Class>
			</Module>
			<!-- tivic 1.0.3 Module -->

Property line

<!-- tivic 1.0.3 Module Property's -->	
<!-- Mysql Server jdbc:<URL>/<DB> -->	
<Property>
<Name>MysqlServer</Name>
<Value>jdbc:mysql://localhost/wowza</Value>
</Property>
<!-- Mysql UserName -->
<Property>
<Name>MysqlUser</Name>
<Value>root</Value>
</Property>
<!-- Mysql Password (default value empty)-->
<Property>
<Name>MysqlPass</Name>
<Value></Value>
</Property>
<!-- Wrong StreamKey Error Message to clients -->
<Property>
<Name>StreamErrorMsg</Name>
<Value>Tivic.Tv - Bağlantı'da Hata Oluştu </Value>
</Property>
<!-- tivic 1.0.3 Module Property's -->
