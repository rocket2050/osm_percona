# osm_percona

# Ansible Role: Percona

Ansible playbook to install percona MySQL server in Debian/Ubuntu servers

[![Build Status](https://api.travis-ci.org/overdrive3000/ansible-percona.svg)](https://travis-ci.org/overdrive3000/ansible-percona/)

## Requirements

None.

## Role Variables

Available variables are listed below with its default values.

	root_password: reallylongpassword

Define the MySQL root password, this password will be used to create a **/root/.my.cnf** to allow root mysql connections without password

	port: 3306
	bind_address: 0.0.0.0

Define port and bind address for MySQL connections

	max_allowed_packet: 16M
	key_buffer: 16M
	thread_stack: 192K
	thread_cache_size: 8

Define some values to tuning the database server

	sqldebug: true
	log_slow_queries: log_slow_queries    = /var/log/mysql/mysql-slow.log
	long_query_time: long_query_time      = 2
	log_queries_not_using_indexes: log-queries-not-using-indexes

If **sqldebug** is true this playbook will configure Percona MySQL with slow queries debug logs, if you want to disable this debug information you have to set **sqldebug: false**
 
