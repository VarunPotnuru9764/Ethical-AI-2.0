user database has two table 
-> user_info of values (
                name text not null,
                email text unique not null,
                password_hash text not null,
                pid integer not null,
                foreign key (pid) references user_pid(pid)
            )

  -> user_pid of values (
                pid integer primary key autoincrement,
                email text unique not null
            )
      

