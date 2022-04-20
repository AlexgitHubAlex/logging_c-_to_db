# logging_c-_to_db
Progect async logging from c++ to some backend db

It is pet project for practic architecture skills, async work with c++, high performance, work with Postgres and up my skill work with c++14+. 


# Some interface information
Interface logic equal std::cout interface c++ program. Interface implement some logging level
- Debug()
- Info()
- Warning()
- Error()

All interface ovveride operator<<() for input some data on it. All type turns around to_string() method. 

Need think about write loging only need level info, but implementation didn't based on macros implementation. 

Work based on create some message system with metainfo witch sending on thread work with db. This thread write all messege on db backend.
This library don't writed for concret implementation db or framework, but maybe use some of it for implement some part simple. 
