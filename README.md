# テーブル設計

## usersテーブル

|  Column      |  Type    |  Options      |
|  ----------  |  ------  |  --------     |
|  email       |  string  |  null: false  |
|  password    |  string  |  null: false  |
|  name        |  string  |  null: false  |
|  profile     |  text    |  null: false  |
|  occupation  |  text    |  null: false  |
|  position    |  text    |  null: false  |

## commentsテーブル

|  Column     |  Type        |  Options      |
|  ---------  |  ------      |  --------     |
|  text       |  text        |  null: false  |
|  user       |  references  |  -----------  |
|  prototype  |  references  |  -----------  |

## prototypesテーブル

|  Column      |  Type        |  Options        |
|  ----------  |  ------      |  --------       |
|  title       |  string      |  null: false    |
|  catch_copy  |  text        |  null: false    |
|  concept     |  text        |  null: false    |
|  image       |  ------      |  ActiveStorage  |
|  user        |  references  |  -----------    |


