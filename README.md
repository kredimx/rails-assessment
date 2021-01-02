# Kredi backend developer technical assessments
## Table of contents

- [General](#general)
- [Rules](#rules)
- [Recommendations](#recommendations)
- [Ruby quiz](#ruby-quiz)
- [Challenges](#challenges)

## General

At [Kredi](https://www.kredi.mx), We are focused on critical financial processes. That is why we want our development team to focus on quality code and best practices.

This is a small technical assessment for our open position as Backend Sofware Developer. We encourage you to follow the rules and recommendations described above:

## Rules:

- Be honest, do not copy code from Stack overflow, We all know programmers do that, but this time we want to evaluate your thinking process.
- Do not mention the company name in your repository.
- Apply best practices, var names, indentation, readability, SOLID, DRY, Design patterns, etc.
- Test your code, We strongly recommend RSpec.
- Publish your code on Github || Gitlab, be careful about how you write your commit messages.
- Deploy your code to Heroku, it takes no longer than 20 minutes!
- If you require any further information or assistance, please feel free to contact us.

## Recommendations:

- Follow best practices.
- Use code conventions for Ruby
- Use a CSS framework (Bootstrap, tailwind, or equivalent).
- Avoid n+1 queries.
-


## Part I
### Ruby Quiz

Please add a file called `quiz.md` to your repo with your answers:

#### 1. Write a function that returns product of all numbers of an array/range

```ruby
>> product([1, 4, 21])
=> 84
>> product([-4, 2.3e12, 77.23, 982, 0b101])
=> -3.48863356e+18
>> product([-3, 11, 2])
=> -66
>> product([8, 300])
=> 2400
>> product([234, 121, 23, 945, 0])
=> 0
>> product(1..5)
=> 120
```

#### 2. Compare if two strings are anagrams (assume input consists of ASCII alphabets only)

```ruby
>> str_anagram('Tap', 'paT')
=> true
>> str_anagram('beat', 'table')
=> false
>> str_anagram('beat', 'abet')
=> true
>> str_anagram('seat', 'teal')
=> false
>> str_anagram('god', 'Dog')
=> true
```

#### 3. Compare if two strings are same irrespective of case

```ruby
>> str_cmp('nice', 'nice')
=> true
>> str_cmp('how', 'who')
=> false
>> str_cmp('GoOd DaY', 'gOOd dAy')
=> true
>> str_cmp('foo', 'food')
=> false
```

#### 4. Write a function that sorts the keys in a hash by the length of the key as a string. For instance, the hash:

```ruby
{ abc: 'hello', another_key: 123, 4567 => 'third' }
```

should result in:

```ruby
["abc", "4567", "another_key"]
````


#### 5. Explain the difference between calling `super` and `super()` methods (OOP)


# Challenges

There are different challenges, please solve the challenge your recruiter asked you to solve.


### [Challenge 1: Url shortener](a1/README.md)

### [Challenge 2: Project Management Tool](a2/README.md)

<br/>
<br/>

### Happy coding! :)