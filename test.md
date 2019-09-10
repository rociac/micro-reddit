User
id integer
name string
email string
created_at timestamp
updated_at timestamp

has_many Post
has_many Comment

Post
id integer
title string
content string
user_id integer

belongs_to User
has_many Comment

Comment
id integer
content string
user_id integer
post_id integer

belongs_to User
belongs_to Post
