# Kredi backend developer technical assessments
## Table of contents

- [General](#general)
- [Rules](#rules)
- [Recommendations](#recommendations)
- [Ruby quiz](#ruby-quiz)
- [Challenges](#challenges)

## General

We are [Kredi](https://www.kredi.mx), the mortgage marketplace for LatAm (Backed by YC W21), We are focused on critical financial services, our development team is focused on great code, readability, [S.O.L.I.D. principles](https://www.honeybadger.io/blog/ruby-solid-design-principles/#:~:text=The%20SOLID%20design%20principle%20includes,Liskov%20Substitution%20Principle), and best practices.

This is a small technical assessment for our open position as Backend Sofware Developer. We encourage you to follow the rules and recommendations described above:

## Rules & Recommendations:

- Be honest, do not copy code from Stack overflow, Sometimes we (as programmers) do that, but this time we want to evaluate your thinking process, the way you solve problems, the quality of your code, etc.
- **Please, do not mention the company name in your repository**.
- Apply best practices, readable var names, indentation, code readability, S.O.L.I.D., DRY, Design patterns, etc.
- Test your code, We strongly recommend RSpec.
- Publish your code on `Github || Gitlab`
- Pay atention on your commit messages.
- Deploy your code to Heroku, it takes no longer than 20 minutes!
- If you require any further information or assistance, please feel free to contact us.
- Use code conventions for Ruby
- Use a CSS framework (Bootstrap, tailwind, or equivalent if needed).
- Avoid n+1 queries.



# Instructions:

Part I: Quiz, you have to answer 5 questions, the idea of this quiz is to analyze how you can solve ruby code, take in mind


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
>> anagram?('Tap', 'paT')
=> true
>> anagram?('beat', 'table')
=> false
>> anagram?('beat', 'abet')
=> true
>> anagram?('seat', 'teal')
=> false
>> anagram?('god', 'Dog')
=> true
```

#### 3. Compare if two strings are same irrespective of case

```ruby
>> compare('nice', 'nice')
=> true
>> compare('how', 'who')
=> false
>> compare('GoOd DaY', 'gOOd dAy')
=> true
>> compare('foo', 'food')
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