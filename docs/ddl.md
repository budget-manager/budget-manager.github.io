## Data definition Language (DDL)

```derby
create sequence hibernate_sequence start with 1 increment by 1;
create table budget
(
    budget_id         bigint       not null,
    budgeted_amount   bigint       not null,
    created           timestamp    not null,
    end_date          DATE         not null,
    name              varchar(100) not null,
    recurring         boolean,
    start_date        DATE         not null,
    threshold_percent double       not null,
    updated           timestamp    not null,
    user_id           bigint       not null,
    primary key (budget_id)
);
create table transaction_info
(
    transaction_id bigint       not null,
    amount         bigint       not null,
    created        timestamp    not null,
    date           timestamp    not null,
    name           varchar(100) not null,
    note           varchar(1000),
    budget_id      bigint       not null,
    user_id        bigint       not null,
    primary key (transaction_id)
);
create table user_info
(
    user_id   bigint       not null,
    oauth2key varchar(100) not null,
    role      integer      not null,
    username  varchar(100) not null,
    primary key (user_id)
);
alter table user_info
    add constraint UK_o39uemmk44orv3e8opvqs6g82 unique (oauth2key);
alter table user_info
    add constraint UK_f2ksd6h8hsjtd57ipfq9myr64 unique (username);
alter table budget
    add constraint FKasvhnhp6pbveyhquscvm9nl4 foreign key (user_id) references user_info;
alter table transaction_info
    add constraint FKa3keisihgb1jwysnc25clp50j foreign key (budget_id) references budget;
alter table transaction_info
    add constraint FKisd2xkhi02nh7kg120s5cjpmf foreign key (user_id) references user_info;
```

[`ddl.sql`](https://raw.githubusercontent.com/budget-manager/budget-manager-server/master/docs/sql/ddl.sql)