<a name="readme-top"></a>

# Appeals service
## Author - [Moiseev Evgeniy](https://github.com/Moiseev-Evgeniy)

### Description
The appeals service is designed to submit various appeals from citizens for the performance of work by various administrative structures with different areas of responsibility.<br>
The service has implemented user authentication and authorization using access and refresh tokens based on JWT.<br>
During the operation of the service, logging is performed and users are notified by e-mail.
_______________________________________________________________________________________
### [Architecture](https://github.com/Appeals-service/start/blob/main/architecture/schema.png)
_______________________________________________________________________________________
### Main stack
- FastAPI
- SQLAlchemy
- PostgreSQL
- RabbitMQ
- S3 (Selectel)
- Pytest
- Docker
_______________________________________________________________________________________
### Repositories:<br>
- [Appeals service](https://github.com/Appeals-service/Appeals_service)
- [Authorization service](https://github.com/Appeals-service/Authorization_service)
- [Notification service](https://github.com/Appeals-service/Notification_service)
- [Logging service](https://github.com/Appeals-service/Logging_service)
_______________________________________________________________________________________
### Launch<br>
1. Clone [start repository](https://github.com/Appeals-service/start) to your PC
2. Create and fill in all the `.env_*` files in the `/docker` directory based on the examples in the same directory
3. Go to the root directory
4. Run the command `make dc-up`
5. Follow the link [Swagger](http://127.0.0.1:8000/docs)
_______________________________________________________________________________________
### Functionality<br>
  - #### User
    - registration
    - login
    - logout
    - refresh tokens
    - get user data
    - create appeal
    - get appeals list
    - get appeal detail
    - delete appeal (if not assign)
    - update appeal
  - #### Executor
    - registration
    - login
    - logout
    - refresh tokens
    - get user data
    - get appeals list
    - get appeal detail
    - update appeal (if assigned)
    - assign appeal to yourself
  - #### Admin
    - registration
    - login
    - logout
    - refresh tokens
    - get user data
    - get users list
    - delete user
    - create appeal
    - get appeals list
    - get appeal detail
    - delete appeal
    - update appeal
    - assign a appeal to executor

#### <p align="right"><a href="#readme-top">up</a></p>
